Below is a clean **Markdown (MD) formatted** list of the key interview questions you asked, along with strong, concise answers aligned to your experience.

---

# 📘 Interview Q&A Summary – Data Engineering

---

## 1. Introduction – Skills & Experience

**Q:** Tell me about your experience and skillset.

**A:**
I am a Lead Data Engineer with over 10 years of experience building scalable, cloud-based data platforms. Currently, I work at Sutter Health where I design and manage large-scale data ingestion and transformation systems on AWS. I work extensively with Python, SQL, AWS services like S3, Glue, Lambda, and Step Functions, and Snowflake as the analytics warehouse. My focus areas include modular pipeline design, data quality, schema enforcement, performance optimization, and secure handling of healthcare data. I also mentor engineers and contribute to architecture decisions.

---

## 2. Cloud Experience Beyond AWS

**Q:** Do you have experience with Databricks or Azure?

**A:**
My primary hands-on experience is with AWS. However, I have worked in environments where Databricks was used for Spark-based large-scale processing and collaborated on data integrations involving Azure services like Data Factory and ADLS. I understand distributed processing concepts and can adapt quickly across cloud ecosystems.

---

## 3. Data Quality During Ingestion

**Q:** What data quality checks do you perform while ingesting data?

**A:**
I implement:

* **Schema validation** (data types, required fields)
* **Null and completeness checks**
* **Duplicate detection** using business keys
* **Business rule validation** (date logic, code sets)
* **Referential integrity checks**
* **Volume anomaly monitoring**
  Invalid records are quarantined, and data lineage is tracked for traceability.

---

## 4. Delayed Event Tracking

**Q:** How do you handle delayed events?

**A:**
I design pipelines around **event time**, not arrival time. I use a **lateness window** (e.g., 24–48 hours) and reprocess recent partitions to capture late data. Upserts (MERGE) ensure late records update historical data instead of duplicating it. Monitoring tracks the gap between event time and ingestion time.

---

## 5. Watermarking – Implementation

**Q:** How do you implement watermarking?

**A:**
In batch systems, I store the last processed event timestamp in a **control table**. Each run processes data newer than `(last_watermark – lateness_window)` and updates the watermark after success. In streaming systems, watermarking is configured in the processing logic using the event-time column and allowed delay threshold.

---

## 6. Referential Checks

**Q:** What are referential integrity checks?

**A:**
These ensure foreign keys match valid master records. For example, every `patient_id` in a claims table must exist in the patient table. Unmatched records are quarantined and monitored.

---

## 7. Handling Sensitive (PII/PHI) Data

**Q:** How do you ensure sensitive data is protected?

**A:**
I apply:

* Data classification
* Field minimization
* Masking and tokenization
* Role-based access control
* Encryption at rest and in transit
* Audit logging
* De-identified data in non-prod environments

---

## 8. Tokenization at Scale

**Q:** What about managing millions of token mappings?

**A:**
We use deterministic tokenization and store mappings in a secure, indexed lookup system. Access is highly restricted. Tokens are generated once during ingestion and reused downstream.

---

## 9. Justification for Big Data Architecture

**Q:** Why is a big data architecture justified?

**A:**
Because of:

* High data volume and growth
* Mixed structured/semi-structured data
* Complex cross-domain transformations
* High concurrency analytics
* Compliance and governance requirements
* Need for scalable, cost-efficient processing

---

## 10. Irreversible Encryption

**Q:** What is irreversible encryption?

**A:**
It refers to **cryptographic hashing**. We use **salted SHA-256 hashing** to de-identify sensitive identifiers. The original value cannot be retrieved, and the hash is used as a safe surrogate key.

---

## 11. Data Masking – Implementation

**Q:** How do you implement masking?

**A:**
Masking is implemented:

* **Dynamically** at the warehouse level using role-based masking policies
* **Statically** during ETL when sharing or moving data
  Sensitive fields are partially hidden or replaced based on user roles.

---

## 12. Role-Based Security (RBAC)

**Q:** How do you implement RBAC?

**A:**
Roles are created based on job functions. Permissions are granted to roles (not users). Users are assigned roles, ensuring least-privilege access to schemas and tables.

---

## 13. Row-Level Security (RLS)

**Q:** How is row-level security implemented?

**A:**
We create row access policies that filter data based on user role or tenant mapping. For example, regional users only see rows where `region = their_region`.

---

## 14. Multi-Tenancy

**Q:** Explain multi-tenancy in patient data systems.

**A:**
Multiple organizations share the same platform, but each record includes a `tenant_id`. Row-level policies ensure users only see data belonging to their tenant. This allows shared infrastructure with strict logical isolation.

---

## 15. SQL Self Join

**Q:** How do you get employee and manager names from the same table?

**A:**
By performing a **self join**:

```sql
SELECT e.emp_name AS employee, m.emp_name AS manager
FROM employees e
LEFT JOIN employees m ON e.manager_id = m.emp_id;
```

The `manager_id` references another employee’s `emp_id`.

---

## 16. Why LEFT JOIN?

**Q:** Why use LEFT JOIN instead of INNER JOIN?

**A:**
Because some employees have no manager. LEFT JOIN ensures all employees appear, with NULL for manager where applicable.

---

## 17. Python – Counting Unique Events

**Q:** Count unique event types per user.

**A:**

```python
from collections import defaultdict

def count_unique_events(events):
    user_events = defaultdict(set)
    for e in events:
        user_events[e["user_id"]].add(e["event_type"])
    return {uid: len(types) for uid, types in user_events.items()}
```

---

## 18. Why `defaultdict`?

**Q:** Why use defaultdict?

**A:**
It automatically creates an empty set for a new user_id, avoiding manual key checks.

---

## 19. What Does `return` Do?

**Q:** Explain `return` in Python.

**A:**
`return` sends a value back from a function and ends its execution. Without it, a function returns `None`.

---

This document summarizes the technical depth, architecture knowledge, and practical implementation skills demonstrated during the discussion.
