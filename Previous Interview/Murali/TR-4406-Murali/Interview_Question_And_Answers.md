Below is the full **Markdown (MD) file** containing **all the questions you were asked in the mock interview** along with **clean, experience-based, interview-ready answers** aligned exactly to your architecture and explanations.

---

# **MDM Python AWS Developer – Interview Q&A (Full Set)**

## **1. Give me a brief introduction.**

I have a little over 12 years of experience in Python development, data engineering, and building cloud-native MDM and ETL pipelines on AWS. In my recent role at Bon Secours Mercy Health, I designed and implemented serverless ingestion frameworks, entity-matching engines, survivorship logic, and real-time mastered-data publishing pipelines. I worked extensively with Python, Lambda, Step Functions, Glue, SQS/SNS, and SQL to build scalable MDM workflows for patient, provider, and facility master domains.

---

## **2. What are your source systems?**

Our key sources included Epic for clinical/patient data, Lawson for provider/HR data, credentialing systems for licensing/NPI data, facility management systems, and multiple legacy scheduling/registration systems.

---

## **3. Where are the transformations happening? Which services are used?**

Transformations happen in two layers:

- **Real-time**: In Python-based Lambdas for validation, standardization, matching, and survivorship.
- **Batch**: In AWS Glue for large-volume standardization, DQ checks, and harmonization.
  We use Step Functions for orchestration, SQS/SNS for event flow, and API Gateway when synchronous data access is needed.

---

## **4. How are your Lambdas triggered?**

Most Lambdas are **SQS-triggered** (event-driven ingestion).
We also use triggers from Step Functions, and optionally API Gateway or S3 events depending on the pipeline type.

---

## **5. How do you profile source data before ingestion?**

I first load sample extracts into Pandas or PySpark and compute null ratios, uniqueness, pattern checks, and distribution analysis. I compare data quality across systems (Epic vs Lawson vs legacy), validate identifier consistency, and align attributes to business rules. This helps design matching thresholds and survivorship rules.

---

## **6. Besides SQL, do you use Pandas or other tools?**

Yes, I use **Pandas** and **PySpark** for deeper profiling—null analysis, data type validation, distribution checks, and pattern recognition. Pandas helps with quick, script-driven profiling before onboarding a new source.

---

## **7. How did you use Pandas specifically?**

I load sample datasets into Pandas DataFrames, run automated null-ratio checks, validate attribute formats, and analyze name/address distributions. Pandas was key in comparing attribute reliability across sources and designing survivorship rules.

---

## **8. Were you deeply involved in MDM architecture/implementation?**

Yes. I designed the ingestion framework, harmonization layer, Python-based matching engine, survivorship logic, golden-record creation, and downstream event publishing. I also defined routing logic, DQ rules, and reusable MDM components across domains.

---

## **9. Why build custom MDM instead of using vendor tools?**

The decision was made before I joined, but the key reasons were:

- High customization needs for clinical data.
- Need for full control over matching/survivorship logic.
- Lower long-term cost vs. vendor licensing/customization.
- Faster iteration with a cloud-native, Python-based engine.

---

## **10. Walk me through your MDM pipeline end-to-end.**

1. **File or event lands in S3/SQS**
2. **Step Functions** starts the workflow
3. **Classification Lambda** determines batch vs real-time
4. **Glue or Lambda** runs standardization and DQ
5. **Matching Engine** computes deterministic + fuzzy scores
6. **Survivorship Logic** selects trusted attributes
7. **Golden Record** is generated
8. **Persist** in MDM Hub + ODS
9. **SNS publishes** mastered entity to all downstream consumers

---

## **11. Deep dive: How does your matching engine work?**

- Deterministic checks for MRN, NPI, internal IDs.
- Fuzzy scoring for names, addresses, phones.
- Weighted composite scoring based on profiling results.
- Threshold-based classification into strong match, probable match, or new entity.

---

## **12. How do you calculate confidence scores? Any libraries used?**

I wrote a custom scoring framework in Python.

- Deterministic matches get full weight.
- Fuzzy scores computed using lightweight libraries like **rapidfuzz**.
- Composite score = Σ(weight × attribute score).
- Outcomes driven by thresholds validated with governance.

---

## **13. Do you generate suspected matches?**

Yes. Mid-confidence scores become **suspected matches**. These pass through address-comparison layers and go into a secondary review or auto-resolution path based on future events.

---

## **14. How much data are you processing daily?**

Across Epic, Lawson, and legacy systems, we process **50,000–100,000+ events per day**, and significantly more on batch-refresh days.

---

## **15. How do you optimize your Lambda processing?**

- Avoid large payloads
- Cache reference data
- Precompute lookups
- Use efficient fuzzy algorithms (rapidfuzz)
- Set reserved/provisioned concurrency
- Offload heavy workloads to Glue
- Benchmark Lambda hot paths

---

## **16. Do you optimize SQL queries as well?**

Yes. We optimize lookups using indexing, caching frequent reference data, rewriting inefficient joins, using bulk loads, and monitoring execution plans for regressions.

---

## **17. What logging/observability tools do you use?**

- **Structured JSON logging** in all Lambdas
- **CloudWatch metrics/alerts** (DLQ, queue depth, errors)
- **X-Ray traces** for latency troubleshooting
- **Step Functions execution maps**
- **Custom MDM Audit Dashboard**
- **SNS alerts** for critical failures
- **DLQ + replay mechanism**

---

## **18. Do you have experience with AWS X-Ray? How did you use it?**

Yes. I used it for:

- End-to-end trace of ingestion → matching → survivorship
- Performance bottleneck detection (fuzzy match, address parsing)
- Troubleshooting slow external calls
- Custom annotations for match scores, source IDs
  Configured via Lambda active tracing + X-Ray SDK + Step Functions tracing.

---

## **19. What is the Lambda timeout limit?**

**15 minutes** maximum.

---

## **20. Does one Lambda process all 100k or 1M records?**

No. One Lambda never processes the full file.
We split batches into smaller chunks via Glue, push to SQS, and Lambda processes each chunk independently with automatic scaling.

---

## **21. Real-time or batch? What is your design?**

Hybrid:

- Real-time (SQS → Lambda) for streaming events
- Batch (S3 → Step Functions → Glue) for large or nightly files
  Both use the same shared Python MDM engine.

---

## **22. How do you design Lambdas for a million records?**

- Glue splits the file into chunks
- Push chunks into SQS
- SQS triggers thousands of Lambdas in parallel
- Each Lambda handles 100–1,000 records only
- Step Functions tracks orchestration
- DLQ for any failed chunks

---

## **23. After a file is uploaded to the raw bucket, what happens?**

- S3 event → Step Functions
- Classification Lambda checks metadata
- Step Functions routes to either Glue (batch) or SQS (real-time)
- Processing continues via the appropriate pipeline

---

## **24. So is it Glue or Lambda? What was your design?**

Both—depending on file type & size.
Routing happens centrally via Step Functions.

- Large files → Glue
- Small/incremental files → Lambda
  Both use the same shared MDM logic.

---

## **25. Do you have guardrails before ingestion?**

Yes:

- File naming and path validation
- Schema/header validation
- Size and format checks
- Source identity verification
- Required attribute checks
- Quarantine + alerts on failure

---

## **26. Can Lambda handle a million records?**

No, a single Lambda cannot.
We distribute the load via Glue chunking → SQS → many parallel Lambdas.

---

## **27. How do you process 1M records using Lambdas?**

Chunk the file → push chunks to SQS → Lambda auto-scales horizontally → each Lambda handles only a small batch.

---

# **End of MD File**

If you want, I can also generate a **crisp version** or **short-answer version** for rapid-fire technical rounds.
