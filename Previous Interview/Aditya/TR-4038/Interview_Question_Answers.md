Here’s a **Markdown (MD)** file version containing all your **interview questions and answers** from this series of Molina-related discussions — written in a **clear, detailed, and conversational style** suitable for review or documentation.

---

````markdown
# Claims & Eligibility Developer Interview — Q&A Summary

## 1. Tell me about your experience around claims and eligibility — especially with PL/SQL and data extraction.

In my recent work, I’ve been deeply involved in the **claims and member eligibility** space — particularly focusing on data integration, validation, and reconciliation between multiple systems.  
I’ve used **PL/SQL** extensively for writing stored procedures, functions, and packages to process and validate large claim datasets. For example, we developed logic to handle **member-claim mismatches**, where eligibility data from external sources didn’t align with claims received.

I also built ETL-like data extraction jobs to identify discrepancies between **enrollment feeds** and **claims processing tables**, helping improve overall data accuracy.  
This required a mix of **complex SQL joins**, **performance tuning**, and **PL/SQL cursors** to efficiently handle millions of records.

---

## 2. What is the core system that Molina uses?

Molina primarily uses **Facets** as its core claims processing system.  
It manages **member eligibility**, **provider data**, **claims adjudication**, and **billing**.  
In our integration layer, we usually interact with Facets through **database procedures**, **flat file interfaces**, or **web services**, depending on the use case.  
For example, in claims automation or reconciliation processes, we extract data from Facets staging tables using **SQL scripts or APIs**, then transform and send it to external vendors or reporting systems.

---

## 3. Tell me about the project you worked on — specifically around claims and member eligibility mismatch.

Sure. I worked on a project focused on resolving **claims vs. eligibility mismatches**.  
Sometimes, claims come in for members whose eligibility isn’t updated or synchronized with the current month’s enrollment data.  
Our goal was to **automate detection and resolution** of those mismatches.

We built a backend PL/SQL module that:

- Validated incoming claims against the latest eligibility data.
- Logged exceptions into a mismatch table.
- Triggered notifications to the enrollment team for resolution.

Once fixed, the corrected eligibility was fed back into the Facets system.  
This improved our **claim processing accuracy** and reduced manual intervention by over 30%.

---

## 4. What’s the difference between `%TYPE` and `%ROWTYPE` in PL/SQL?

- `%TYPE` is used when you want a variable to take **the same data type** as a specific column or another variable.  
  Example:
  ```sql
  emp_salary employees.salary%TYPE;
  ```
````

This ensures that even if the column type changes in the database, your variable automatically adapts.

- `%ROWTYPE` is used when you want to declare a record that represents **an entire row** of a table or cursor.
  Example:

  ```sql
  emp_record employees%ROWTYPE;
  ```

  This lets you access all columns of a table row at once, like `emp_record.emp_id` or `emp_record.emp_name`.

You’d use `%TYPE` for **single column references** and `%ROWTYPE` when you need **a full record structure**, such as fetching or updating complete rows.

---

## 5. What are some key ways to optimize PL/SQL code for performance?

There are several approaches I usually apply:

- **Use bulk operations** (`FORALL`, `BULK COLLECT`) instead of row-by-row loops to minimize context switching between SQL and PL/SQL engines.
- **Avoid unnecessary queries** inside loops — fetch all needed data at once.
- **Use bind variables** to reuse execution plans and prevent hard parsing.
- **Analyze execution plans** and **create proper indexes** for high-selectivity queries.
- **Use pipelined functions** for better performance on large datasets.
- **Limit context switching** by combining SQL and procedural logic efficiently.
- **Profile and tune** using Oracle tools like TKPROF or DBMS_PROFILER.

---

## 6. What is context switching in PL/SQL?

Context switching happens when control moves back and forth between the **PL/SQL engine** and the **SQL engine**.
For example, if your PL/SQL block executes SQL statements repeatedly inside a loop, each statement causes a context switch, which adds overhead.

To minimize it:

- Use **BULK COLLECT** to fetch multiple rows at once.
- Use **FORALL** to perform bulk DML operations.
- Move as much logic as possible into SQL rather than repeatedly calling SQL from PL/SQL.

By reducing context switches, you improve performance significantly — especially in large data processing tasks.

---

## 7. How do you minimize context switching when executing SQL?

When executing SQL dynamically or in transactions, the key is to:

- Batch similar operations together using **bulk binding**.
- Avoid executing one statement per iteration in a loop.
- Use **table joins or inline subqueries** instead of fetching data in multiple PL/SQL loops.
- Push more computation into SQL rather than procedural code, since SQL runs in its own engine.

For example, instead of looping through claim IDs and inserting one-by-one, I’d use:

```sql
FORALL i IN claim_list.FIRST .. claim_list.LAST
    INSERT INTO claim_summary VALUES (claim_list(i));
```

This reduces round-trips and context switches between SQL and PL/SQL engines.

---

## 8. Suppose you need to design an application that processes files for a vendor — fetching data from a database, creating a flat file, and sending it. How would you plan and manage that?

I’d start by breaking the application into **modular stages**:

1. **Requirements & Planning**
   Understand file layout, format (CSV, fixed-width), schedule (daily/weekly), and transmission protocol (SFTP, API).

2. **Data Extraction Layer**
   Build optimized SQL or PL/SQL procedures to extract required claim or eligibility data from source tables.
   Apply filters, joins, and business rules in the query itself to reduce transformation load.

3. **Transformation & File Creation**
   Use Node.js, Python, or PL/SQL’s UTL_FILE to transform the data into the required file structure.
   Apply field formatting, validations, and mapping logic.

4. **File Delivery**
   Automate file transfer to the vendor via **SFTP** or **API integration**, with audit logging and checksum validation.

5. **Error Handling & Logging**
   Implement logging tables or an ELK stack for tracking failures, retries, and performance metrics.

6. **Scheduling & Automation**
   Use **cron jobs**, **Oracle Scheduler**, or a CI/CD pipeline for execution.

7. **Monitoring & Alerts**
   Send email or dashboard alerts on success/failure status.

This approach ensures maintainability, auditability, and scalability of the entire data processing workflow.

---

## 9. How are newborn claims handled?

When a newborn claim is received, typically, the system doesn’t yet have the baby registered as a separate member.
In such cases:

- The claim is initially linked to the **mother’s member ID**.
- A **temporary member record** may be created for the newborn.
- Once eligibility enrollment is updated (usually within a few days), the newborn is assigned a unique member ID.
- The claim is then reprocessed or re-adjudicated under the correct member profile.

The key is ensuring that the newborn is **linked to the correct parent policy**, and eligibility updates are synchronized promptly to avoid denials or delays.

---

## 10. Suppose you completed your JIRA story quickly but notice another teammate is taking longer. What do you do?

If I finish early, my first step is **to communicate with the team**.
I’d let my scrum master or tech lead know that my story is complete and that I’m available to help others.
If a teammate is struggling, I’d offer to **pair program**, review their code, or help debug an issue.

For example, during our claims automation project, I once finished my PL/SQL enhancement early and noticed another developer stuck on a complex eligibility extraction task. I spent time helping optimize their joins and indexes — we resolved it quickly, and the sprint goal stayed on track.

If everyone’s on schedule, I might pick up **technical debt**, write **unit tests**, or improve **query performance** in existing modules.
This proactive approach ensures the team stays productive and cohesive.

---

# ✅ Summary

This interview covered key areas:

- Claims and eligibility processing.
- PL/SQL concepts (`%TYPE`, `%ROWTYPE`, context switching).
- Performance tuning and optimization.
- Application planning for data integration.
- Agile collaboration and teamwork.

These answers demonstrate both **technical expertise** and **collaborative problem-solving**, which are crucial for the claims/eligibility developer role.

---

```

---

Would you like me to **add one section at the top** — like a short **self-introduction summary** (e.g., “About Me: Developer with X years in healthcare/PLSQL/claims domain”) before the questions?
It makes the file more complete for sharing or interview prep.
```
