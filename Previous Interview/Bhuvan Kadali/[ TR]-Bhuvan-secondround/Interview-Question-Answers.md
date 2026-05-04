# Interview Q&A Summary

## 1. Introduction
**Answer:**
Hi, my name is Bhuvan Chandra Kadali, and I bring around 12+ years of experience in Data Engineering, Python development, and cloud-based data platforms. Currently, I work as a Lead Data Engineer at Liberty Mutual, where I design scalable data pipelines and modern data architectures.

---

## 2. End-to-End Pipeline Design (SQL Server → AWS → Snowflake)
**Answer:**
Design involves ingestion using AWS DMS/Glue, landing in S3, transformation via Spark/Glue, loading into Snowflake using Snowpipe/COPY, followed by modeling and orchestration using Airflow or Step Functions.

---

## 3. Schema Management & Loading Strategy
**Answer:**
Handled using schema-on-read in raw layer and schema-on-write in warehouse. Use Type 1 for overwrite and Type 2 for historical tracking using MERGE and effective date fields.

---

## 4. Handling Missing Business Key
**Answer:**
Use derived composite keys or surrogate keys with hash-based change detection for identifying uniqueness and changes.

---

## 5. Data Sources to S3
**Answer:**
From on-prem via AWS DMS (CDC), from APIs via Lambda/Glue, and files via SFTP into S3 as central data lake.

---

## 6. Unstructured Data Handling
**Answer:**
Ingest JSON into S3, process using Spark/Glue, flatten nested structures, and load into Snowflake as structured tables or VARIANT.

---

## 7. Glue Catalog & Athena
**Answer:**
Use Glue Crawlers to create metadata catalog and query data in S3 via Athena for validation and exploration.

---

## 8. SQL Joins
**Answer:**
Inner, Left, Right, Full, Cross, Self, Natural, Semi, Anti joins.

---

## 9. CTE Types
**Answer:**
Single, multiple, chained, recursive, and subquery replacement CTEs.

---

## 10. Data Integrity without Constraints (Snowflake)
**Answer:**
Use pipeline-level validation, MERGE logic, audit tables, and reconciliation checks instead of DB constraints.

---

## 11. Mongo Flattening & Deduplication
**Answer:**
Use document ID, composite keys, controlled unwind, hash validation, and reconciliation checks.

---

## 12. Mongo $out vs $merge
**Answer:**
$out replaces entire collection; $merge supports incremental upsert logic.

---

## 13. Observability Metrics
**Answer:**
Track freshness, completeness, quality, and reliability; expose via dashboards and alerts.

---

## 14. Connectivity & Credentials
**Answer:**
Use AWS Secrets Manager, IAM roles, key-pair authentication, and secure network configurations.

---

## 15. Version Control & Deployment
**Answer:**
Use Git with feature branching, CI/CD pipelines, environment separation, and automated deployments.

---

## 16. Final Role Understanding Question
**Answer:**
Ask about daily responsibilities, collaboration, expectations, and success metrics.

