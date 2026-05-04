# Interview Q&A – Senior Full-Stack (Python, AI, Healthcare)

---

## 1. Walk me through a recent AWS project

**Answer:**
I worked on a cloud-native automation and monitoring platform for healthcare data pipelines.

The challenge was that multiple legacy systems were processing prescription and distribution data, but there was no centralized visibility or validation.

We designed an event-driven microservices architecture using FastAPI, AWS Lambda, API Gateway, Step Functions, EventBridge, and RDS PostgreSQL.

Prescription files were stored in S3, and workflows were triggered automatically using events.

We also built a React dashboard for real-time monitoring and implemented CI/CD pipelines, which improved reliability and reduced production incidents.

---

## 2. What kind of Python coding was involved?

**Answer:**
Most of the work was hands-on Python development.

I built REST APIs using FastAPI, implemented business logic for validation and transformation, and handled async processing.

I also wrote event-processing logic for EventBridge, integrated AWS services using boto3, and created reusable modules for logging, validation, and error handling.

Additionally, I worked on unit and integration testing to ensure system reliability.

---

## 3. What did the healthcare application do?

**Answer:**
The application acted as a centralized automation and monitoring layer for prescription and distribution data.

It tracked data across systems, validated it at each stage, and triggered workflows when issues occurred.

It provided real-time visibility, reduced manual monitoring, and improved overall reliability of the pipeline.

---

## 4. Was prescription data structured or unstructured?

**Answer:**
It was a mix.

Structured data included IDs, drug codes, and timestamps.

Unstructured data included doctor notes, instructions, and sometimes inconsistent payloads from external systems.

---

## 5. How did you process unstructured data?

**Answer:**
We used a layered approach.

First, we normalized the data (cleaning, formatting).

Then we applied regex and rule-based extraction for known patterns.

We also used dictionary-based mapping for drug names and, in some cases, lightweight NLP tools like spaCy.

Finally, we converted everything into structured format for downstream processing.

---

## 6. What information did you extract from prescriptions?

**Answer:**
We extracted key fields like:
- Patient identifiers  
- Drug name  
- Dosage and frequency  
- Route of administration  
- Quantity  
- Doctor details  
- Prescription date  

We also normalized instructions like “once daily” into structured formats and mapped drugs to standardized codes.

---

## 7. What NLP methods did you use?

**Answer:**
We mainly used rule-based NLP.

This included regex, pattern matching, and dictionary-based entity extraction.

We also used text normalization and occasionally spaCy for NER in complex cases.

The focus was on reliability and explainability rather than heavy ML models.

---

## 8. Was regex reliable across different prescription formats?

**Answer:**
Not by itself.

We handled variability using:
- Input normalization  
- Multiple regex patterns per field  
- Dictionary-based matching  
- Validation layers  

If extraction confidence was low, we flagged it for manual review.

---

## 9. What was the accuracy of your extraction?

**Answer:**
We validated using real datasets.

For critical fields like drug and dosage, accuracy was around 85–90%.

For free-text fields, it was slightly lower.

We also tracked failure rates and used fallback mechanisms to ensure safety.

---

## 10. Where were prescription images stored?

**Answer:**
They were stored in AWS S3.

Metadata was stored in RDS PostgreSQL.

Processing pipelines were triggered using S3 events.

---

## 11. Was the processing automated or scheduled?

**Answer:**
It was mostly event-driven.

When files were uploaded to S3, events triggered Lambda or Step Functions.

Step Functions orchestrated OCR, validation, and processing.

We also had scheduled jobs for batch processing and reconciliation.

---

## 12. Do you have experience with EC2?

**Answer:**
Yes, I’ve used EC2 for hosting services and backend workloads where needed, along with other AWS services.

---

## 13. Do you have exposure to ML or MLOps?

**Answer:**
Yes, mainly from an integration perspective.

I’ve deployed and integrated ML services, containerized models, exposed them via APIs, and monitored outputs.

I understand concepts like model versioning, drift, and production monitoring, though I haven’t built models from scratch.

---

## 14. Have you worked on CI/CD, Terraform, Kubernetes?

**Answer:**
Yes, I’ve worked on CI/CD pipelines using tools like GitHub Actions.

I’ve contributed to Terraform scripts and worked with Docker and Kubernetes for deploying services.

I’ve handled end-to-end deployment for specific services in a team setup.

---

## 15. Do you have any questions for us?

**Answer:**
Yes, I asked about:
- Backend and frontend tech stack  
- Cloud infrastructure (AWS/Azure, Kubernetes/serverless)  
- LLM usage and agent architecture  
- Day-to-day responsibilities and team collaboration  

---

## 16. Closing Statement

**Answer:**
I thanked them for the discussion, expressed interest in the role, and mentioned that I’m excited about working on AI-driven healthcare systems.

---