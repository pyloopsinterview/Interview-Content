# Interview Questions & Answers – MDM Python (AWS) Developer  
**Candidate: Amritpal Singh**

---

## 1. Give me a brief introduction about yourself.

**Answer:**  
Hi, my name is Amritpal Singh. I have a little over **12 years of experience in data engineering, ETL development, and MDM solutions**, with strong hands-on expertise in **Python, AWS, and modern data warehousing platforms like Snowflake**.  

In my current role at **AmerisourceBergen**, I design and build **scalable, cloud-native data pipelines** using **AWS Lambda, Glue, S3, SNS, SQS, and CloudWatch**. I recently led an **MDM data onboarding and synchronization initiative** where multiple OLTP systems were sending inconsistent product and customer master data. I designed a **serverless AWS pipeline** to standardize, match, and merge records before loading them into Snowflake.  

I’m also deeply involved in **performance tuning, monitoring, documentation, and mentoring junior developers**, and I work closely with product and analytics teams in an agile environment.

---

## 2. They are building a lot from the ground up. Someone with natural curiosity and AI exposure is a good cultural fit. How do you relate?

**Answer:**  
I’m naturally curious and enjoy exploring new technologies, especially **AI and automation**. Even outside of work, I experiment with **Python-based ML models and LLM-driven data enrichment**, and I think about how AI can improve **MDM matching, deduplication, and data quality workflows**. This mindset fits well with teams building platforms from scratch and evolving them over time.

---

## 3. Creating one source of truth instead of doing things the old way — what’s your approach?

**Answer:**  
My approach is to challenge legacy assumptions and focus on **MDM fundamentals** like **standardization, matching, survivorship, and governance**. I make sure all downstream systems consume a **certified golden record**, not raw source data, and I work closely with business and governance teams to enforce data quality at the source.

---

## 4. Can you describe a scalable data pipeline you designed using AWS services, and why?

**Answer:**  
I designed a **serverless MDM pipeline** using **S3, Lambda, SQS, Glue, and Snowflake**. Data landed in S3, Lambda handled validation and routing, SQS decoupled ingestion, and Glue performed distributed transformations, matching, and survivorship logic.  

This design allowed us to **scale automatically, reduce cost, improve resilience**, and support both operational and analytical use cases.

---

## 5. How do you ensure data quality, security, and compliance in your data architectures?

**Answer:**  
I enforce **data quality checks** at multiple stages, including schema validation, null checks, and business rules. For security, I use **IAM least-privilege access**, **encryption at rest and in transit**, and **audit logging**. For compliance, I align with governance teams to meet **PII, retention, and regulatory requirements**.

---

## 6. How comfortable are you with developing and debugging AWS Lambda and Glue using Python?

**Answer:**  
I’m **very comfortable and hands-on** with both. Lambda is central to my real-time validation and orchestration logic, while Glue handles **distributed ETL, matching, and survivorship**. I regularly debug and optimize both using **CloudWatch, Spark UI, and structured logging**.

---

## 7. Can you give a real example of Lambda and Glue working together?

**Answer:**  
In one MDM pipeline, an S3 upload triggered a **Lambda function** that validated schema and business rules. Valid data was pushed to **SQS**, which triggered a **Glue PySpark job** to standardize records, apply deterministic and fuzzy matching, calculate confidence scores, and generate golden records loaded into Snowflake.

---

## 8. Does it go to Glue or Lambda based on your design?

**Answer:**  
Everything goes to **Lambda first**. Lambda acts as the gatekeeper for validation and routing. If the data needs heavy processing, Lambda pushes it to **SQS**, which triggers **Glue**. Lambda stays lightweight, and Glue handles the heavy lifting.

---

## 9. What does distributed processing have to do with a single Lambda?

**Answer:**  
A single Lambda has **nothing to do with distributed processing**. Lambda is not a distributed compute engine. **Glue provides distributed processing**, which is why I separate responsibilities between Lambda and Glue in the architecture.

---

## 10. If you had to process a million records using Lambda, how would you design it?

**Answer:**  
I would design a **fan-out architecture**. The file would be split into smaller chunks in S3, each chunk sent to **SQS**, and multiple Lambdas would process chunks in parallel. Each Lambda would be **idempotent**, with retries and DLQs. A final aggregation step — usually using Glue — would consolidate results.

---

## 11. How are you doing matching in your MDM process?

**Answer:**  
We use a **hybrid matching approach**. First, deterministic matching on strong identifiers like product codes or emails. Then, **probabilistic fuzzy matching** on names and addresses. The results are combined into a weighted confidence score.

---

## 12. How do you calculate high-confidence matches?

**Answer:**  
We assign weights to deterministic and fuzzy signals and compute a **final confidence score** between 0 and 1. Matches above a defined threshold are treated as high confidence, while mid-range scores are flagged for review.

---

## 13. What happens to suspected matches and address comparisons?

**Answer:**  
Suspected matches are flagged and stored for review or enrichment. Addresses are standardized and compared using **token-based fuzzy matching** to catch near-duplicates and formatting differences.

---

## 14. How much data were you processing?

**Answer:**  
Typically **50,000 to 100,000 records per day**, with the system designed to handle spikes smoothly.

---

## 15. How do you optimize scripts for large volumes of data?

**Answer:**  
I optimize using **S3 partitioning, Glue worker tuning, column pruning, broadcast joins**, and by minimizing expensive operations. For Pandas, I rely on **vectorized operations**.

---

## 16. Do you optimize SQL as well?

**Answer:**  
Yes. In Snowflake, I optimize queries using **clustering, micro-partition pruning, materialized views**, and by avoiding unnecessary full-table scans.

---

## 17. What logging and observability improvements did you implement?

**Answer:**  
I implemented **structured logging, correlation IDs, CloudWatch dashboards, alerts, and DLQs** so failures could be detected and resolved quickly.

---

## 18. Do you have experience with AWS X-Ray?

**Answer:**  
Yes. I used X-Ray to trace **Lambda execution paths**, identify latency issues, and analyze downstream dependencies.

---

## 19. What is the timeout limit for AWS Lambda?

**Answer:**  
The maximum timeout for an AWS Lambda function is **15 minutes**.

---

## 20. Is 100k data processed by a single Lambda?

**Answer:**  
No. Lambda handles validation and orchestration only. **Glue handles bulk processing** because it is distributed.

---

## 21. Do you support batch or real-time processing?

**Answer:**  
Both. **Batch processing** is handled through Glue, and **real-time validation** is handled through Lambda.

---

## 22. What is the next step after fuzzy matching?

**Answer:**  
We calculate confidence scores, apply **survivorship rules**, and generate the **golden record**.

---

## 23. How are survivorship rules authored and validated?

**Answer:**  
They are authored by **business SMEs and governance teams**, validated using **Pandas prototypes**, and confirmed through **UAT cycles**.

---

## 24. What happens after a CSV file lands in S3?

**Answer:**  
S3 triggers Lambda → Lambda validates → routes to SQS → Glue processes → Snowflake loads → data is consumed by BI and downstream systems.

---

## 25. Do you have guardrails before ingestion?

**Answer:**  
Yes. We enforce **schema validation, mandatory fields, null thresholds, pattern checks, and duplicate detection** before data enters the pipeline.

---

## **Final Summary**

These questions and answers reflect my hands-on experience designing and delivering **scalable, secure, and governed MDM solutions on AWS**, with strong emphasis on **Python, distributed processing, and clear communication**, aligning well with this role.
