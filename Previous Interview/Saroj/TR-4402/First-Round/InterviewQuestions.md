Here is the **complete Markdown file** containing **all questions you asked during the interview + their exact, correct answers** as per your AWS/Python/TypeScript serverless profile.

---

# **Interview Q&A – Saroj Raj Onta (Full-Stack / Python / AWS Serverless)**

## **1. What is serverless computing?**

Serverless computing is a cloud execution model where the cloud provider automatically handles **server provisioning, scaling, maintenance, and availability**.
Your code runs only when triggered, and you pay only for execution time.
I use serverless heavily with AWS Lambda, Step Functions, DynamoDB, SQS/SNS, and S3.

---

## **2. What is one disadvantage of AWS Lambda?**

One major disadvantage is **cold start latency**.
If a Lambda function hasn’t been invoked for a while, the first request experiences a delay.
To reduce this, I’ve used techniques like minimizing package size and enabling provisioned concurrency for critical paths.

---

## **3. How does serverless computing complement event-driven architecture?**

Serverless complements event-driven architecture because it runs code **in response to events**.
AWS services like S3, SQS, SNS, DynamoDB Streams, and API Gateway generate events that trigger Lambda functions.
This creates a fully decoupled, scalable, and reactive workflow.

---

## **4. What is Event-Driven Architecture?**

Event-driven architecture is a pattern where systems communicate by **producing and consuming events** instead of using direct synchronous calls.
Producers generate events, and consumers react to them.
This results in high scalability, loose coupling, and asynchronous processing.

---

## **5. Design a cost-effective AWS solution for image processing with 7-day high access and long-term audit retention.**

- Store images in **S3**
- Trigger **Lambda** on upload for processing
- Serve through **CloudFront** for 7 days (cached globally)
- Apply S3 **Lifecycle Policy**:

  - Move files to **Glacier Flexible Retrieval** or **Deep Archive** after 7 days

- For audit access, use **S3 Restore** workflow via Lambda
- Use **SQS** if processing needs buffering

This minimizes cost while supporting occasional audit retrieval.

---

## **6. What is the importance of `package.json` in a TypeScript project?**

`package.json` manages:

- Project dependencies
- Dev dependencies like TypeScript, ts-node, Jest
- Scripts such as `build`, `start`, `test`
- Metadata and version control
- Node engine version and module type

It is the core configuration file for any Node/TypeScript project.

---

## **7. What is Redis mainly used for?**

Redis is mainly used for **high-speed in-memory storage**, ideal for:

- Caching
- Session storage
- Pub/Sub messaging
- Distributed locking
- Rate limiting
- Lightweight queues or streams

---

## **8. What are the major components of DynamoDB?**

- **Tables**
- **Items**
- **Attributes**
- **Primary Key** (Partition Key, Sort Key)
- **Partitions**
- **Secondary Indexes** (GSI, LSI)
- **Streams**
- **Capacity Modes** (On-demand, Provisioned)
- **TTL**

---

## **9. Define Partition Key in DynamoDB.**

A **Partition Key** is the primary identifier that DynamoDB uses to **hash and distribute data across partitions**.
It ensures scalability and even data distribution.

---

## **10. Which AWS services have you worked on majorly?**

- Lambda
- Step Functions
- DynamoDB
- S3
- SQS/SNS
- API Gateway + Apigee
- ECS Fargate
- CloudWatch
- IAM
- CodePipeline, CodeBuild, GitHub Actions
- Terraform
- CloudFront
- KMS, CloudTrail, X-Ray

---

## **11. What is AWS Step Functions?**

AWS Step Functions is a **serverless workflow orchestration service** that coordinates multiple steps using state machines.
It supports retries, parallel steps, branching, wait states, and integrates with Lambda and many AWS services.

---

## **12. What is AWS Glue?**

AWS Glue is a **serverless ETL service** used for discovering, cataloging, transforming, and loading data for analytics.
Core components include Glue Data Catalog, Crawlers, Glue Jobs, Workflows, and Triggers.

---

## **13. Have you worked with any messaging framework?**

Yes — mainly:

- **Amazon SQS**
- **Amazon SNS**
- **DynamoDB Streams**
- **Kafka** (in earlier roles)

---

## **14. When do you use SQS vs RabbitMQ?**

### **Use SQS when:**

- Fully managed, serverless queue required
- Massive scale
- No broker maintenance
- At-least-once delivery is acceptable
- Lambda-based event-driven workflows

### **Use RabbitMQ when:**

- Need complex routing (topic, header, direct exchanges)
- Need sub-millisecond latency
- Need bi-directional messaging
- Need full control of acknowledgments
- Comfortable managing a cluster (non-serverless)

---

If you want, I can also generate a **PDF**, **Word**, or **Notion-ready** version.
