Below is the complete **Markdown file** with all the **exact questions asked** during your interview and the **correct answers** you gave, fully formatted for your reference.

---

# MDM Python (AWS) Developer Interview Q&A

**Candidate: Amritpal Singh**

---

### 1️⃣ Question:

**Give me a brief introduction about yourself.**

**Answer:**
Hi, my name is Amritpal Singh. I have a little over **12 years of experience in data engineering, ETL development, and MDM solutions**, with strong hands-on expertise in **Python, AWS, and modern data warehousing platforms like Snowflake**. In my current role at **AmerisourceBergen**, I’m responsible for **designing and building scalable cloud-native data pipelines** using **AWS Lambda, Glue, S3, SNS, SQS, and CloudWatch**.

A recent project I led involved **MDM data onboarding and synchronization** for product and customer master data from multiple upstream systems. I designed a **serverless Python-based pipeline** to standardize, validate, and merge master records before loading them into **Snowflake**. The pipeline supported **ODS and analytics** through **dimensional modeling** and provided **API-based access** for BI teams.

I also focus heavily on **performance tuning**, such as **Glue parallelism and S3 partition optimization**, and maintain **monitoring, documentation, and architectural best practices**. I also **mentor junior developers** and drive **code reviews** to ensure code quality.

**In conclusion**, I bring strong expertise in **Python, MDM, AWS ETL, and scalable data architecture**, aligned directly with this role.

---

### 2️⃣ Question:

**They are currently building a lot from the ground up. Someone with natural curiosity who has been dabbling with AI—even personally—is a great cultural fit. How do you relate to that?**

**Answer:**
I naturally stay **curious about emerging technologies**, especially **AI and automation**. Outside of work, I actively experiment with **Python-based ML models, LLM integrations**, and **AI-powered data enrichment tools** such as **Hugging Face and LangChain**.

I also explore **AWS AI/ML services** like **SageMaker and Comprehend**, and I continuously look for ways to **infuse intelligence into ETL and MDM workflows**. I enjoy being part of **ground-up innovation**, challenging outdated processes, and leveraging AI to **improve data quality and operational efficiency**.

**In summary**, I bring a **curiosity-driven mindset**, continuously learning and proactively applying AI where it adds value.

---

### 3️⃣ Question:

**They want someone focused on creating one single source of truth — not just accepting how it’s always been done. What’s your approach?**

**Answer:**
I always prioritize creating a **single, trusted, authoritative dataset**. In MDM projects, I implement **standardization, survivorship rules, data quality enforcement, and deduplication** across multiple source systems. I push teams to **challenge legacy assumptions**, improve **upstream governance**, and ensure every downstream consumer relies on **the same certified golden records**.

**In conclusion**, I drive **modernized, governed, and unified** master data solutions instead of carrying legacy issues forward.

---

### 4️⃣ Question:

**Can you describe a scalable data pipeline that you designed and implemented using AWS services? And why was it needed?**

**Answer:**
I designed a **serverless MDM onboarding pipeline** with **AWS S3, Glue (PySpark), Lambda, SNS, SQS, and CloudWatch**. It ingested large volumes of product and customer data from multiple OLTP systems, applied **standardization and matching logic**, and produced **golden records** for **Snowflake ODS and analytics**.

It was needed because:

* We had **data inconsistencies** across source systems
* Business needed **a unified source of truth**
* Serverless created **cost efficiency + automatic scaling**
* **Asynchronous messaging** improved **fault tolerance**
* S3 partitioning and tuning **boosted overall performance**

**Conclusion:** The architecture ensured **reliability, scalability, and high-quality master data** for enterprise use.

---

### 5️⃣ Question:

**How do you ensure data quality, security, and compliance in the data architectures that you design?**

**Answer:**
For data quality, I enforce **schema validation, referential integrity, transformation rules, deduplication**, and **automated alerts** using CloudWatch.
For security, I apply **least-privilege IAM roles**, **KMS encryption**, **secure VPC networking**, **TLS enforcement**, and **audited access controls**.
For compliance, I follow governance policies for **PII handling, retention rules**, maintain **data lineage**, and enforce **role-based access** through catalogs and metadata.

**Conclusion:** I align every architecture with strong **preventive quality controls**, **robust security**, and **governance-driven compliance**.

---

### 6️⃣ Question:

**How comfortable are you with developing and debugging AWS Lambda functions and Glue jobs using Python? Can you give an example?**

**Answer:**
I am **highly comfortable** working with both services — building event-driven Lambda workflows and distributed Glue ETL jobs in Python.

Example:
In the MDM onboarding pipeline, **S3 → Lambda → SQS → Glue** formed the core workflow. Lambda executed **real-time schema and business validation** and sent rejected records to a remediation bucket. Glue handled **PySpark transformations, matching, survivorship logic**, and optimizations using **bookmarks, partition pruning**, and **parallel execution**. I used **CloudWatch logs, DLQs**, and **Spark UI** to debug issues, achieving a **40% performance improvement** post-optimization.

**Conclusion:** I am very confident in **designing, debugging, deploying, and optimizing** Lambda and Glue in production.

---

## Final Wrap-Up

All answers provided demonstrate capabilities in **MDM, AWS data engineering, Python ETL, security, and scalable cloud architectures**, ensuring a strong match for the **MDM Python (AWS) Developer** role.

---

If you want, I can also:

* Convert this into **interview speaking script format** for easier delivery
* Add **STAR-based story examples**
* Create a **follow-up Q&A** set for potential deeper grilling

Would you like me to prepare a **Thank-you email** as well after the interview?
