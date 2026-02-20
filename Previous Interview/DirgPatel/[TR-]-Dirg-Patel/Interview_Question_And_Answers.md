# Senior Data Engineer & Technical Lead – Interview Q&A

---

## 1. Introduction & Data Engineering Experience

**Q:** Could you introduce yourself and describe your experience designing production-grade data pipelines using Python, PySpark, Airflow, and SQL?

**A:** I have 12+ years of software engineering experience, with strong focus on Data Engineering and Technical Leadership. I’ve built production-grade batch and streaming pipelines using Python and PySpark, orchestrated with Airflow, and optimized SQL transformations. My work includes performance tuning, CI/CD automation, secure deployments, and large-scale data processing in enterprise environments.

---

## 2. Pluggable Sync Layer in Python Pipelines

**Q:** How would you design a pluggable sync layer to add new destinations with minimal changes?

**A:** I would use OOP principles with an abstract base class and Strategy pattern. Each destination implements a common interface, and a factory loads it via configuration. This ensures loose coupling, extensibility, and minimal changes when adding new sinks.

---

## 3. SLA Miss During Month-End

**Q:** How would you capacity plan and optimize a pipeline that frequently misses SLA?

**A:** I would analyze Spark UI metrics, data growth, and executor usage. Then optimize partitioning, joins, caching, and incremental loads. I’d scale cluster resources, tune parallelism, and strengthen monitoring with SLA alerts.

---

## 4. Handling Retries from Slow Network Writes

**Q:** How would you design retries, timeouts, and backoffs to avoid duplicate effects?

**A:** I ensure idempotent writes using upserts or MERGE logic. I configure exponential backoff with retry limits and explicit timeouts. For Spark, I batch writes using foreachPartition and enable checkpointing in streaming to avoid duplicates.

---

## 5. Custom Partitioner Causing Skew

**Q:** How would you evaluate and replace a skewed custom partitioner?

**A:** I’d analyze Spark UI metrics to confirm skew, review key distribution, and replace with hash-based partitioning or salting for hot keys. I’d also enable Adaptive Query Execution (AQE) and tune shuffle partitions.

---

## 6. Containerizing Data Pipelines

**Q:** What would you include in a Docker image and how would you manage dependencies?

**A:** I use a lightweight base image, include only required application code, and pin dependencies in requirements.txt. I use multi-stage builds, CI-based image versioning, and inject secrets via environment variables.

---

## 7. DAG Dependency on Unavailable External System

**Q:** How would you implement fallbacks or circuit breakers?

**A:** I’d implement a circuit breaker pattern with retry thresholds and cooldown. I’d design fallback mechanisms like cached snapshots or deferred processing. Airflow retries and alerting ensure graceful degradation.

---

## 8. Event-Time vs Processing-Time Scheduling

**Q:** How do you prevent gaps and overlaps?

**A:** I use Airflow’s logical execution date for deterministic event-time windows. I track last processed timestamps in metadata tables and enforce idempotent writes with backfill support.

---

## 9. KubernetesPodOperator Resource Tuning

**Q:** How would you tune requests, limits, and retries?

**A:** I analyze CPU and memory metrics, set realistic requests, slightly higher limits, and configure controlled retries with timeouts. I may split workloads or adjust Spark configurations for stability.

---

## 10. Schema Evolution in Automated Pipelines

**Q:** How do you handle schema evolution with backward compatibility?

**A:** I enforce explicit schema definitions in version control, allow nullable additive changes, validate schemas in CI, and implement drift detection with alerts. Curated layers enforce strict schema governance.

---

## 11. Unpinned Dependency in CI

**Q:** How would you detect and remediate it?

**A:** I add CI checks to fail builds if dependencies aren’t pinned. I enforce version locking, update requirements with exact versions, and run automated tests before merging.

---

## 12. GCP Service Accounts vs User Accounts

**Q:** What’s the difference and how are they used in CI/CD?

**A:** User accounts are for human access. Service accounts are for automation. In CI/CD, I use service accounts with least-privilege IAM roles and secure authentication like Workload Identity.

---

## 13. VPC Service Controls in GCP

**Q:** How does VPC SC protect data and what challenges arise?

**A:** VPC SC creates a security perimeter to prevent data exfiltration. It enhances security but can restrict cross-project communication and CI/CD integrations, requiring careful network design.

---

## 14. Handling Schema Drift from SFTP CSV Ingestion

**Q:** How would you manage changing source columns?

**A:** I use a layered architecture (Raw → Staging → Curated). Raw layer is flexible; curated layer enforces strict schema. I validate schema changes, use metadata-driven mapping, and add CI-based data quality checks.

---

## 15. Transaction Fact vs Incremental Snapshot Fact

**Q:** What guides your design decision?

**A:** Transaction facts provide event-level granularity and flexibility. Snapshot facts simplify reporting and improve performance. I choose based on business needs, data volume, and query patterns—sometimes using both.

---

## 16. Junior Breaking Production Deployment

**Q:** How would you respond?

**A:** I stabilize production first, then conduct a blameless postmortem. I provide constructive feedback and improve CI/CD guardrails, review processes, and deployment validation checks.

---

## 17. Loosely Defined Project with Delivery Date Request

**Q:** How would you create a credible plan?

**A:** I clarify scope, define success criteria, identify risks, break work into milestones, and provide phased estimates with transparent assumptions. Clear communication ensures realistic commitments.

---
