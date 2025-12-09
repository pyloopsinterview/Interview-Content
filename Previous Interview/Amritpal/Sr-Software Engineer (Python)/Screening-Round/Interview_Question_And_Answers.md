Below is a **complete Markdown (MD) file** containing **all the questions you were asked** and the **best, polished interview-ready answers** you can read word-for-word.

You can copy/paste this directly as your **Interview Q&A Notes.md** file.

---

# **Interview Q&A – Senior Software Engineer (Python)

Prepared for Amritpal Singh Malhi**

---

## **1. What is your experience with AWS?**

I have extensive hands-on experience working with **AWS** for more than **6 years**. Most of the applications and data pipelines I’ve built use **serverless** and **cloud-native** components. I work regularly with **AWS Lambda, Glue, S3, SNS, SQS, CloudWatch, API Gateway, IAM**, and **Step Functions**.

I design and deploy **Python-based microservices** and **ETL pipelines**, including event-driven architectures using **SQS** for decoupling and **Lambda** for real-time processing. I also optimize Glue parallelism, Lambda cold-starts, and S3 partitioning for scalable performance.
Overall, AWS is a core part of my engineering work, and I’m very comfortable building end-to-end cloud solutions.

---

## **2. What Python frameworks have you worked with?**

I’ve worked extensively with **Django**, **Django REST Framework**, **Flask**, and **FastAPI** for building APIs and microservices.
For data and ETL workloads, I use **AWS Glue (PySpark)**, **Pandas**, and **SQLAlchemy**.
I also use **Celery** for background tasks and **pytest** for testing.
My primary strengths are in **Django**, **Flask**, and **FastAPI** for backend development.

---

## **3. What databases have you worked on?**

I’ve worked with both **SQL and NoSQL** databases, including:

* **PostgreSQL**
* **MySQL**
* **Snowflake** (for analytics and warehousing)
* **MongoDB** (document-based models)
* **Redis** (caching and in-memory operations)

I’m comfortable with schema design, indexing, optimized queries, and performance tuning across these databases.

---

## **4. Have you ever worked on Docker?**

Yes, I have solid hands-on experience with **Docker**.
I containerize Python services, write optimized **Dockerfiles**, work with **multi-stage builds**, and use **Docker Compose** for local orchestration.
I’ve also deployed containerized workloads to **AWS ECS/ECR**, and worked alongside DevOps engineers to integrate Docker into CI/CD pipelines.

---

## **5. What cloud services have you used in your projects?**

Primarily **AWS**: **Lambda, Glue, S3, SNS, SQS, CloudWatch, API Gateway, IAM, Step Functions, ECR, ECS**, and more.

Apart from AWS, I’ve also used:

### **Azure**

* **Azure Functions**
* **Logic Apps**
* **Blob Storage**
* **Azure SQL**
* **Azure DevOps**

### **GCP**

* **BigQuery**
* **Cloud Storage**
* **Cloud Functions**

I’m comfortable working in **multi-cloud environments**.

---

## **6. Do you have experience outside AWS (Azure/GCP)?**

Yes.
In **Azure**, I’ve worked with **Functions**, **Logic Apps**, **Blob Storage**, and **Azure SQL**.
In **GCP**, I’ve used **BigQuery**, **Cloud Functions**, and **Cloud Storage** for analytics workloads.

Although AWS is my primary cloud platform, I’m fully capable of adapting to Azure or GCP needs.

---

## **7. What is your experience with scalability?**

I have strong experience designing **scalable and resilient** systems.
I use **event-driven architectures** with Lambda, SQS, and SNS, build **stateless Python microservices**, and optimize performance using **Redis**, indexing, pagination, and connection pooling.

For data pipelines, I scale workloads using **AWS Glue**, optimized **PySpark**, and partitioned S3 datasets.
Across clouds, I use serverless components that automatically scale under load.

---

## **8. Have you ever used Kubernetes?**

Yes, I have **working knowledge** of Kubernetes.
I’ve deployed containerized Python apps on Kubernetes using **Deployments, Pods, Services, ConfigMaps, and Ingress**.
I’ve worked with **EKS** on AWS and collaborated with DevOps teams to support CI/CD and rolling updates.

Kubernetes isn’t my everyday tool, but I’m comfortable with deployments, troubleshooting, and maintaining microservices.

---

## **9. How much experience do you have in React?**

I have around **2 years of hands-on experience** with **React**, mainly for dashboards and internal tools.
I’m comfortable with **hooks**, **state management**, **React Router**, **Axios**, and **Material UI**.
While my primary strength is backend engineering, I can efficiently deliver frontend features when required.

---

## **10. How much backend vs frontend experience do you have?**

My experience is **backend-heavy**:

* **Backend:** 80–85%
* **Frontend:** 15–20%

Most of my work focuses on Python microservices, APIs, ETL pipelines, and cloud architecture.
I contribute to React when needed, but my core expertise is backend engineering.

---

## **11. Example of centralized application experience**

A strong example is a **centralized Master Data Management (MDM) application** I built.
Multiple upstream systems were sending inconsistent customer/product data.
I built a centralized onboarding and standardization system using **AWS Glue, Lambda, SQS, S3, and Snowflake**.

This platform became the **single source of truth**, performing cleansing, matching, merging, and exposing the clean master data to downstream analytics and API consumers.

---

## **12. What unit testing tools have you used?**

My primary tool is **pytest**.
I also use:

* **unittest**
* **pytest-mock / unittest.mock**
* **coverage.py**
* **Postman/Newman** for API tests
* **Selenium/Playwright** for end-to-end cases when needed

All tests are integrated into **GitHub Actions**, **Azure DevOps**, or **AWS CodePipeline** for automated CI/CD.

---

If you want, I can also create a **PDF**, **DOCX**, or **Notion-style cheat sheet** of this file.
