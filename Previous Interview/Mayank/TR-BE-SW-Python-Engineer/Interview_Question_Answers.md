# Interview Questions & Answers (MD)

This document contains concise, recruiter-friendly and interview-ready answers covering Apache Spark, AWS S3, Kubernetes & Helm, TensorFlow, AWS, Python, and common behavioral/process questions.

---

## 1. Apache Spark

### Q1. What is Apache Spark?
**Answer:**  
Apache Spark is an open-source, distributed computing system designed for large-scale data processing. It provides an interface to program entire clusters with data parallelism and fault tolerance, and is commonly used for ETL, analytics, and streaming workloads.

### Q2. How have you used Spark in your projects?
**Answer:**  
I’ve primarily used PySpark to build and optimize distributed ETL pipelines. Spark was used for large-scale data transformations, joins, aggregations, and enrichment, reading data from sources like databases and S3 and writing processed data to data lakes or warehouses like Snowflake. I’ve also productionized Spark jobs and monitored them for performance and reliability.

### Q3. What is partitioning in Spark and why is it important?
**Answer:**  
Partitioning controls how data is distributed across executors. Proper partitioning improves parallelism, reduces shuffle, and prevents data skew. I use `repartition` or `coalesce` based on workload needs and also partition data on write (for example by date or key) to improve downstream query performance.

### Q4. How do you optimize Spark performance?
**Answer:**  
I focus on partitioning strategy, minimizing shuffle, using broadcast joins when appropriate, caching reused datasets, and tuning executor memory and cores. I also monitor job metrics and logs to identify bottlenecks.

---

## 2. AWS S3 (Simple Storage Service)

### Q5. What is Amazon S3?
**Answer:**  
Amazon S3 is a highly scalable, durable object storage service provided by AWS. It’s commonly used as a data lake, for backup and recovery, and for content storage and distribution.

### Q6. How have you used S3 in your projects?
**Answer:**  
I’ve used S3 as the central storage layer for data platforms, storing raw and processed data. Spark and Python pipelines read from and write to S3, and it’s also used for long-term storage, backups, and integration with analytics and ML workloads.

---

## 3. Kubernetes & Helm

### Q7. What is Kubernetes?
**Answer:**  
Kubernetes is an open-source container orchestration platform that automates the deployment, scaling, and management of containerized applications. It provides features like self-healing, service discovery, load balancing, and rolling updates.

### Q8. What is Helm?
**Answer:**  
Helm is a package manager for Kubernetes. It uses reusable templates called Helm charts to define, install, and upgrade Kubernetes applications in a consistent and repeatable way.

### Q9. Why are Kubernetes and Helm related?
**Answer:**  
Helm runs on top of Kubernetes. Kubernetes manages and runs the containers, while Helm simplifies how applications are packaged, configured, and deployed across environments.

### Q10. How have you used Kubernetes and Helm together?
**Answer:**  
I’ve used Kubernetes to run and scale containerized services and Helm to manage deployments. Helm charts allowed consistent configuration across dev, QA, and production and made upgrades and rollbacks easier.

---

## 4. TensorFlow

### Q11. What is TensorFlow?
**Answer:**  
TensorFlow is a machine learning framework used to build, train, and deploy models that learn from data. It enables large-scale numerical computation and is commonly used for prediction, classification, and pattern recognition.

### Q12. How have you used TensorFlow?
**Answer:**  
I’ve used TensorFlow with Python to train and evaluate machine learning models and integrate model outputs into data pipelines and production systems.

---

## 5. AWS (General)

### Q13. How much AWS experience do you have?
**Answer:**  
I have 8+ years of hands-on AWS experience, primarily supporting data infrastructure and cloud-based deployments.

### Q14. Which AWS services have you worked with?
**Answer:**  
I’ve worked with services such as S3, EC2, IAM, VPC, and integrated them with Spark, Python pipelines, and infrastructure-as-code workflows.

---

## 6. Python

### Q15. How do you use Python in your day-to-day work?
**Answer:**  
Python is my primary language. I use it for data processing, ETL pipelines, automation, and integration with systems like Spark, AWS services, and ML frameworks.

### Q16. Are you comfortable with a Python assessment?
**Answer:**  
Yes. I’m comfortable with Python assessments focused on real-world logic, data manipulation, and clean, readable code.

---

## 7. Background & Experience

### Q17. What is your core technology stack?
**Answer:**  
My core stack is Python, with strong experience in Spark, AWS, data infrastructure, and cloud-native deployments. I also have experience with Java.

### Q18. Do you have deployment experience?
**Answer:**  
Yes. Deployment is part of my day-to-day work, including CI/CD pipelines, infrastructure-as-code, and production releases.

---

## 8. Availability & Process

### Q19. Are you currently working?
**Answer:**  
Yes, but my current engagement is ending, and I’ll be fully available within one to two weeks.

### Q20. Are you comfortable with a fast interview process?
**Answer:**  
Yes. I’m flexible and comfortable moving quickly through interviews and assessments.

---

## 9. Compensation & Work Model

### Q21. Are you comfortable with W-2?
**Answer:**  
Yes, I’m comfortable with W-2 roles.

### Q22. Why consider this role even if the rate is fixed?
**Answer:**  
The company, long-term nature of the role, remote setup, and team quality matter to me. I’ve taken roles at a lower rate when the opportunity and company were a strong fit.
