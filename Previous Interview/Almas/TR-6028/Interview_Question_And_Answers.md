# Data Architect Interview – Q&A (Mohammed Almas Malim)

---

## 1. Tell me about yourself

**Answer:**

Hi, my name is Mohammed Almas Malim.  

I have around 12 years of experience, and over time my role has evolved from backend engineering into data architecture, with a strong focus on PostgreSQL, large-scale data migration, and enterprise integrations.

Currently, I’m working with Bon Secours Mercy Health, where we build and support large healthcare platforms used across multiple hospitals.

One of the key projects I led was a large-scale data migration initiative where we consolidated patient, billing, and operational data from multiple legacy systems, including a mainframe billing system, into a modern PostgreSQL platform.

We also integrated this platform with Salesforce Health Cloud for patient engagement and care coordination.

I was responsible for designing the PostgreSQL architecture, defining migration strategy, building transformation pipelines, and ensuring data consistency across systems.

---

## 2. Have you dealt with huge volume data migration?

**Answer:**

Yes, absolutely.

In my current role, I led a large-scale migration project involving millions to billions of records from legacy systems into PostgreSQL.

My responsibilities included:
- Designing the migration strategy  
- Building data extraction and transformation pipelines  
- Creating a canonical data model  
- Ensuring data quality using validation and reconciliation  

We also handled data inconsistencies and different formats using transformation logic and preprocessing pipelines.

---

## 3. How would you migrate 3 billion records from PostgreSQL to Salesforce?

**Answer:**

For this scale, I would not perform a single bulk push.

Instead, I would:

- Break the data into **smaller batches (chunk-based processing)**
- Use **Salesforce Bulk API 2.0** for asynchronous loading
- Prepare data in a **staging layer** before sending
- Run **parallel jobs with controlled concurrency**
- Implement **checkpointing** to track progress
- Capture and retry **failed records separately**

To ensure success:
- Perform **record count validation**
- Use **checksum or business-level validation**
- Monitor throughput, failures, and API limits

---

## 4. What if performance issues occur after migrating 1 billion records?

**Answer:**

I would not restart the migration.

Instead, I would:

- Resume from the **last successful checkpoint**
- Identify the **root cause**:
  - API issue  
  - Data issue  
  - Performance bottleneck  

Then:
- Adjust **batch size or concurrency**
- Fix **data issues in staging**
- Retry only **failed batches**

I also ensure:
- **Idempotent design (upserts with external IDs)**  
- Proper **monitoring and alerting**  
- Validation of already migrated data  

---

## 5. How strong are you in PostgreSQL transformations?

**Answer:**

I’m very strong in PostgreSQL transformations, especially for large-scale data workloads.

I’ve worked extensively with:
- Complex SQL queries  
- CTEs  
- Window functions  
- JSON/JSONB processing  
- PL/pgSQL procedures  

In my project, I built transformation pipelines to:
- Merge data from multiple systems  
- Deduplicate records  
- Apply business rules  
- Standardize data into canonical models  

For performance:
- I use **set-based operations**
- Apply **partitioning and indexing**
- Break logic into **staged transformations**

I also decide intelligently whether to process data inside PostgreSQL or use external pipelines for semi-structured data.

---

## 6. How do you ensure smooth migration without breakages?

**Answer:**

I ensure smooth migration using:

- **Pre-validation**: Clean and transform data before loading  
- **Controlled execution**: Batch processing + checkpointing  
- **Error handling**: Capture and retry failed records  
- **Monitoring**: Track performance and failures in real-time  
- **Post-validation**:
  - Record count checks  
  - Data reconciliation  
  - Business-level validation  

---

## 7. How do you handle high-pressure environments?

**Answer:**

In high-pressure situations, I focus on:

- Prioritizing critical issues  
- Breaking problems into smaller tasks  
- Maintaining clear communication  

I also ensure:
- Proper fallback strategies  
- Monitoring systems  
- Quick resolution of blockers  

This helps maintain stability even under tight deadlines.

---

## 8. Closing Statement

**Answer:**

Thank you, I really appreciate the opportunity to speak with you today.

It was a great discussion, and the role aligns very well with my experience in PostgreSQL, large-scale migrations, and Salesforce integrations.

I’d definitely be interested in taking this forward and discussing further with the implementation partner and the customer.

Please feel free to reach out if you need anything from my side.

Thanks again, and have a great day.

---
