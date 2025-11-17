Here is the **complete Markdown file** containing **all questions you asked during the interview + correct senior-level answers**.

---

# ✅ **Interview Q&A – Complete (Markdown Version)**

## **1️⃣ Java Stream Filtering**

### **Q:**

```java
Optional<Employee> result = employees.stream()
        .filter(e -> "Paul".equalsIgnoreCase(e.getFirstName()))
        .findFirst();
```

Explain this.

### **A:**

This stream filters employees whose `firstName` equals `"Paul"` (case-insensitive) and returns the **first match** wrapped in an `Optional`.
Uses:

- `Stream API`
- `filter()`
- `equalsIgnoreCase()`
- `findFirst()` (short-circuits)
- `Optional` for null-safety

---

## **2️⃣ SQL JOIN – Employee + Address**

### **Q:**

```sql
SELECT e.employee_id,
       e.first_name,
       e.last_name,
       a.address_type,
       a.address
FROM employee e
JOIN address a
    ON e.employee_id = a.employee_id;
```

Explain.

### **A:**

This is an **INNER JOIN** returning only employees who have a matching record in the address table.
It retrieves employee details + addresses based on the foreign key relationship.

---

## **3️⃣ SQL – Joining Address Twice**

### **Q:**

```sql
SELECT e.employee_id, e.first_name, e.last_name,
       a1.address_line AS residential_address,
       a2.address_line AS office_address
FROM employee e
JOIN address a1
  ON e.employee_id = a1.employee_id AND a1.address_type = 'RESIDENTIAL'
JOIN address a2
  ON e.employee_id = a2.employee_id AND a2.address_type = 'OFFICE';
```

Explain why you joined the address table twice.

### **A:**

Because each address type (RESIDENTIAL, OFFICE) is stored as a **separate row**, we must join the table twice to convert:

- **Multiple rows → into → multiple columns**

This is a classic **self-join** to fetch different filtered rows.

---

## **4️⃣ Q: Tomorrow if I get a new address type, will I join three times?**

### **A:**

Yes, technically—but not recommended.
The scalable solution is **conditional aggregation (pivoting)**:

```sql
MAX(CASE WHEN address_type='RESIDENTIAL' THEN address_line END)
```

This needs **only one JOIN**, no matter how many address types exist.

---

## **5️⃣ Q: I join 10 times?**

### **A:**

You can, but it is poor design.
Use **one JOIN + CASE expressions** instead of 10 joins.

---

## **6️⃣ SSN Verified Flag**

### **Q:**

What datatype will you use for SSN Verified column?

### **A:**

Use a **BOOLEAN** or **BIT(1)**.

- `TRUE` → SSN Verified
- `FALSE` → SSN Not Verified
  If database doesn’t support Boolean (Oracle), use `CHAR(1)` with `'Y'/'N'`.

---

## **7️⃣ Add SSN Verified result to the query**

### **Q:**

Add a column that shows:

- “SSN Verified” → when true
- “SSN Not Verified” → when false

### **A (with LEFT JOIN):**

```sql
SELECT
    e.employee_id,
    e.first_name,
    e.last_name,
    a1.address_line AS residential_address,
    a2.address_line AS office_address,
    CASE
        WHEN e.ssn_verified = TRUE THEN 'SSN Verified'
        ELSE 'SSN Not Verified'
    END AS ssn_status
FROM employee e
LEFT JOIN address a1
    ON e.employee_id = a1.employee_id AND a1.address_type = 'RESIDENTIAL'
LEFT JOIN address a2
    ON e.employee_id = a2.employee_id AND a2.address_type = 'OFFICE';
```

---

## **8️⃣ Q: How many records will be fetched with LEFT JOIN?**

### **A:**

**LEFT JOIN returns exactly the same number of records as the employee table.**

Because the employee table is the left side of the join.

---

## **9️⃣ Q: How many records will be fetched with INNER JOIN?**

### **A:**

INNER JOIN returns **only employees who have BOTH**:

- A RESIDENTIAL address
- An OFFICE address

Others are excluded.

---

## **🔟 Q: Are we only querying employee table or also joining address table?**

### **A:**

We are joining the address table, so the number of results depends on matching address rows.

---

## **1️⃣1️⃣ Q: As per the description, how many records will be fetched?**

### **A:**

As per your description (each employee has both address types),
**the INNER JOIN returns the same number of records as total employees.**

---

# ✅ End of Interview Q&A (Markdown Ready)

If you want, I can turn this into a PDF, DOCX, or GitHub-ready README.md.
