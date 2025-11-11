Got it ✅ — below is your **complete interview Q&A transcript** in a clean, professional **Markdown (.md)** format.
Each question is written exactly as asked (based on your messages), followed by a polished, concise, and technically accurate answer tailored to your experience (Murali – Lead Data Engineer, Healthcare Domain).

You can copy-paste this into a file like `Murali_Data_Engineer_Interview_QA.md`.

---

# 🧠 Data Engineer Interview — Murali Mohan

### Company: Bon Secours Mercy Health (Candidate Experience Reference)

### Domain: Healthcare | Cloud: Azure | Core: Python, ADF, Databricks, PostgreSQL

---

## **1. Can you give me a brief introduction about yourself?**

**Answer:**
Hi, my name is **Murali Mohan**, and I have over **12 years of experience** as a **Lead Data Engineer**, with a focus on **Python-based data engineering, cloud architecture, and backend systems**.
Currently, I’m working at **Bon Secours Mercy Health**, where I lead the design and development of **Azure-based data pipelines** that consolidate patient, insurance, and device data into a unified analytics platform.
I primarily use **Azure Data Factory**, **Databricks**, **Blob Storage**, and **PostgreSQL**.
One of my key projects automated patient data ingestion and transformation, reducing manual reporting effort by **over 60%** while ensuring HIPAA-compliant processing.

---

## **2. Yeah, maybe if we can go more into your recent experience, kind of try to understand the systems that you build.**

**Answer:**
At Bon Secours, we built a **centralized patient data and analytics platform** that integrates data from multiple EHRs, wearable devices, and insurance systems.
The goal was to create a **Patient 360 view**.
I designed **ETL/ELT pipelines** using **ADF** for orchestration and **Databricks (PySpark)** for transformation, landing curated data into **Azure Database for PostgreSQL** for BI teams.
This unified data layer now powers both operational and predictive analytics across departments.

---

## **3. What was your level of involvement? Were you coding yourself or mostly leading others?**

**Answer:**
My role is a mix of **hands-on engineering and technical leadership**.
I architected the overall data flow, selected technologies, and built core components like Python-based ETL frameworks and Terraform infrastructure scripts.
I’m hands-on with Python and PySpark for key transformations, while mentoring six developers and overseeing CI/CD automation through **Azure DevOps**.

---

## **4. Can you give me an example of a specific pipeline — source, transformation, data flow, and usage?**

**Answer:**
Sure — one core example is our **Patient 360 Pipeline**:

- **Sources:** EHR (Epic, Cerner), insurance claims (CSV/SFTP), and wearable data (API).
- **Ingestion:** ADF pipelines orchestrated data ingestion, invoking **Python Azure Functions** to fetch and land raw data in **Blob Storage**.
- **Transformation:** Performed in **Azure Databricks (PySpark)** — cleaning, mapping ICD-10 codes, and de-identifying PHI.
- **Storage:** Curated data stored in **Azure Database for PostgreSQL**, following a star schema.
- **Consumers:** Used by **Power BI analysts** and **data scientists** for reporting and patient risk models.
  This pipeline improved data freshness and reduced report prep time by 60%.

---

## **5. So the process was used as an analytical kind of data store, or was it just kind of a presentation layer?**

**Answer:**
It served primarily as an **analytical data layer**.
Our PostgreSQL instance acted as a **curated data mart** for BI and data science teams.
It wasn’t just a reporting layer — it supported aggregations, analytical queries, and machine learning pipelines.
The structure was designed for analytical workloads, not transactional use.

---

## **6. And this was all on AWS?**

**Answer:**
Initially, yes — we started on **AWS** using **S3, Glue, and RDS (PostgreSQL)**.
Later, I helped migrate to **Azure**, reimplementing the same architecture using **ADF**, **Databricks**, and **Blob Storage**.
The migration focused on leveraging Azure-native tools while maintaining the same ELT principles.
Now, our entire data ecosystem runs natively on **Azure**.

---

## **7. Can you describe in particular something you had to optimize, like a pipeline that wasn’t performing well?**

**Answer:**
Yes — one key pipeline that processed encounter and claims data in Databricks began taking nearly **2 hours** instead of the usual 45 minutes.
Using **Spark UI** and **ADF run logs**, I found the issue:

- **Skewed joins** on `patient_id`,
- **Large full reads** from Blob, and
- **No cluster autoscaling**.
  I optimized it by applying **salting**, **broadcast joins**, and **incremental processing** logic, plus enabling **autoscaling**.
  After that, runtime dropped to **~35 minutes**, and we achieved consistent daily SLA compliance.

---

## **8. Unstructured data, your experience with unstructured data processing — you used BeautifulSoup, right?**

**Answer:**
Yes, I’ve worked with unstructured data like **clinical notes, discharge summaries, and insurance PDFs**.
I used **BeautifulSoup** to parse HTML and **PyPDF2** to extract text, followed by **regex**, **NLTK**, and **spaCy** for entity extraction.
We converted this text into structured JSON — extracting entities like _diagnosis, medications, and follow-up recommendations_.
This allowed analysts to access structured clinical data that was previously locked in free-text documents.

---

## **9. Was there a specific use case requested by your end users or business team for this unstructured data?**

**Answer:**
Yes — our **care management team** needed to identify patients’ **follow-up instructions and prescribed medications** from physician notes.
We trained a **custom spaCy NER model** to extract medication names, dosages, and conditions.
The structured output was stored in Azure and joined with EHR data for predictive modeling.
This automated data extraction reduced manual chart review by **70%** and enabled **readmission risk analytics**.

---

## **10. How far did you go with NLP? How much did you use spaCy or NLTK?**

**Answer:**
I built **custom NLP pipelines** with **spaCy and NLTK** for clinical entity extraction.
We fine-tuned a **custom NER model** on 2,000 annotated notes using Prodigy, extending spaCy’s base model to detect entities like _Medication_, _Dosage_, _Frequency_, and _Condition_.
I also used **dependency parsing** to link related entities (e.g., medication → dosage → purpose).
This approach increased entity accuracy by **~30%** over regex-only methods.

---

## **11. Where did spaCy shine for you?**

**Answer:**
It really shined in **extracting structured medication information** from unstructured text.
Regex-based extraction failed due to inconsistent phrasing, but spaCy’s **NER** and **dependency parsing** accurately linked medication, dosage, and condition in context.
That reduced manual data prep time by **over 50%** and made those insights available in real-time for analytics.

---

## **12. Let’s talk about Postgres — when you get an EXPLAIN ANALYZE on a query, what are you looking for to figure out where the problem is?**

**Answer:**
I focus on these key points in `EXPLAIN ANALYZE`:

1. **Scan Type:** Look for sequential scans where an **index scan** should occur — fix by indexing or rewriting non-sargable filters.
2. **Join Type:** Replace inefficient **Nested Loops** with **Hash or Merge joins** where appropriate.
3. **Row Estimates:** If actual vs. estimated rows differ greatly, I run `ANALYZE` or adjust statistics.
4. **Sort/Disk Usage:** “Sort Method: external merge” means it’s spilling to disk — increase `work_mem` or add covering indexes.

Using these, I’ve optimized queries from **28s → 4s** by adding composite indexes and rewriting joins.

---

## **13. Do you work with SQL Server as well? What are the key differences between SQL Server and Postgres?**

**Answer:**
Yes — I’ve worked with **SQL Server** in legacy healthcare systems.
Key differences:

- **SQL Server:** Commercial, tightly integrated with **Power BI, SSIS**, uses **T-SQL**; great for transactional workloads.
- **PostgreSQL:** Open-source, supports **JSON, arrays, and custom data types** — ideal for analytical workloads.
- PostgreSQL offers more control for **partitioning, indexing**, and **schema design**, while SQL Server provides stronger built-in ETL tooling.
  We prefer PostgreSQL for its **flexibility, cost efficiency, and cloud scalability**.

---

## **14. Can you talk a little bit about your experience with Azure Data Factory?**

**Answer:**
Yes — I used **ADF** as the orchestration layer for our entire ETL ecosystem.

- It ingested data from **APIs, SFTP, and on-prem SQL** into **Blob Storage**.
- Triggered **Databricks notebooks** for transformations.
- Loaded curated data into **PostgreSQL**.
- Set up **Logic App alerts**, **parameterized datasets**, and **parallel ForEach loops** for scalability.
  ADF also logged runs to **Log Analytics** for monitoring and SLA tracking.
  We orchestrated **25+ daily pipelines**, processing **8–10 GB** of data reliably.

---

## **15. Can you talk about your experience with Lambda?**

**Answer:**
Sure — I used **AWS Lambda** for **event-driven ETL** and automation.
Examples include:

- API data extraction triggered by **CloudWatch schedules**.
- File validation triggered by **S3 events**.
- Sending messages to **SQS** or invoking **Step Functions** for orchestration.
  All Lambdas were **Python-based**, stateless, and modular.
  On Azure, I use the same approach with **Azure Functions**, leveraging **Blob and HTTP triggers** for ingestion and validation.
  Both follow the same **serverless, event-driven architecture** pattern.

---

## **16. You graduated with a Master’s in 1999 — what were you doing before your 12 years in Python?**

**Answer:**
Good question — in my early career, I worked on **enterprise data systems** using **C#, Oracle PL/SQL**, and ETL tools like **Informatica**.
Around **2011**, I transitioned into **Python and open-source frameworks**, focusing on automation and data pipelines.
It was a natural progression — the domain stayed the same, but the tools evolved.
This background helps me bridge legacy systems with modern cloud data architectures effectively.

---

## **17. We have multiple businesses — how does that align with your experience?**

**Answer:**
That’s actually very similar to my current setup.
At Bon Secours, we support multiple business units — **clinical, insurance, and operations** — all consuming data differently.
I designed **shared pipelines** and **common data models** to support each domain while maintaining central governance and compliance.
So I’m very comfortable building scalable data architectures across multi-domain business environments.

---

## **18. Do you have any questions for us?**

**Answer:**
Yes, just one — I’d love to understand how your team is integrating **Azure Data Factory and NLP workflows**.
Are you primarily orchestrating those pipelines through **ADF + Databricks**, or also experimenting with **Azure Machine Learning or Synapse** for deeper text analytics?

---

# ✅ **End of Interview Summary**

Murali’s answers highlighted:

- Deep expertise in **Azure Data Engineering** (ADF, Databricks, Blob, PostgreSQL)
- Strong **Python and NLP** (BeautifulSoup, spaCy, PySpark) experience
- Clear understanding of **data optimization, governance, and architecture**
- Leadership and migration experience from **AWS → Azure**

---

Would you like me to add a **final section** at the bottom (like “Thank You + Closing Statement”) to use in your post-interview follow-up email?
