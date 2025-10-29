# Full Stack Developer Interview – Q&A (Lavjinder Singh)

---

### **1. Introduction and Experience**

**Question:**  
So, Singh, let's start this interview talking about your previous experiences. You have over 14 years in this field, right? I’d like you to brief me on your past experience — but not in terms of companies or projects — focus on the technologies you’ve worked with, especially those relevant to this position.

**Answer:**  
Hi, my name is Lavjinder. I have 14 years of experience working as a Lead Full Stack Developer.  
My core strengths lie in **Java (Java 17)**, **Spring Boot**, **Microservices**, **React**, **Node.js**, and **GraphQL**.  
I have worked extensively on designing and integrating APIs within a microservices architecture using various design patterns.

I have hands-on experience with **AWS** (25–30 services) including Lambda, API Gateway, SNS, SQS, EC2, CloudWatch, and others.  
Currently, I’m leading a design and development team at **Verizon**, working on large-scale enterprise platforms supporting customer-facing applications.

A key project involves **customer order orchestration and fulfillment systems** handling millions of daily transactions for Verizon broadband and 5G services.  
I lead a team of six developers and act as an architect, migrating monolithic systems to microservices using **Spring Boot**, **Kafka**, **AWS EKS**, and **React with TypeScript**.

Implemented **Kafka-based asynchronous messaging**, **Redis caching**, and **CI/CD pipelines** in **Jenkins** and **AWS CodePipeline**.  
Optimizations reduced average order processing latency by **35%** and improved reliability during peak loads.

---

### **2. Databases**

**Question:**  
Have you worked with relational and NoSQL databases?

**Answer:**  
Yes. I’ve worked with both relational and NoSQL databases:

- **Relational:** MySQL, SQL Server
- **NoSQL:** MongoDB, DynamoDB, Redis  
  MongoDB (document-based), Redis (key-value store), and DynamoDB (managed NoSQL).

---

### **3. Java Thread-Safe Blocking Queue**

**Question:**  
You need to implement a thread-safe blocking queue using Java with enqueue and dequeue methods that block the calling thread if necessary.

**Answer:**  
_(Code or conceptual explanation expected — omitted in transcript)_

---

### **4. Spring Boot API Performance Optimization**

**Question:**  
Your Spring Boot REST API becomes slow under high traffic in production, causing timeouts. How would you investigate and optimize performance?

**Answer:**  
I’d begin by collecting **metrics and logs** via **Datadog APM**, checking if servers or APIs are slow.  
Then, analyze **database performance** using `EXPLAIN` plans, check for missing indexes, and optimize queries.

Monitor **Spring Boot Actuator** endpoints for request timings, **JVM metrics** (memory, GC, threads), and **infrastructure metrics** (CPU, memory, disk, network).  
Use **APM tools** (Datadog/New Relic) for tracing and pinpointing hotspots.

Simulate production load via **JMeter** or **Gatling** and compare performance across environments.  
Common issues include:

- Slow DB queries, missing indexes, N+1 queries
- Connection pool exhaustion
- Blocking operations in controller threads
- Lack of caching
- Large unoptimized JSON serialization

Fixes:

- Add indexes
- Optimize slow queries
- Use connection pooling
- Increase thread pool size
- Implement caching and efficient serialization

---

### **5. Cross-Browser UI Inconsistency**

**Question:**  
UI behaves differently on Chrome, Firefox, or Safari (layout shifts, broken styles). How would you ensure consistent UX across browsers?

**Answer:**  
Use **Polyfills** to normalize UI and handle browser-specific inconsistencies.  
Also, apply **Normalize.css** or CSS resets to standardize default styles across browsers.

---

### **6. Node.js API Gateway Performance**

**Question:**  
A Node.js API Gateway aggregates responses from multiple microservices. Under load, users report increased response times and timeouts. How would you troubleshoot and optimize it?

**Answer:**  
Start by **collecting gateway metrics** — request throughput, response times, error rates.  
Check **Node.js Event Loop lag** using **Clinic.js** or **Prom Client**.  
Monitor **CPU/memory usage** and **downstream service logs** for slow responses.

Use **Prometheus**, **Grafana**, or **New Relic** for observability.  
Load test with **Artillery** or **JMeter** and profile with Node’s built-in profiler or **Clinic.js**.  
Implement **distributed tracing** (OpenTelemetry) to identify slow backend calls.

Common causes:

- Sequential service calls (fix with `Promise.all`)
- Blocking operations (heavy computations or synchronous I/O)
- Inefficient data transformations
- Missing caching
- Network bandwidth issues

Solutions:

- Parallelize service calls
- Offload CPU-heavy tasks
- Implement caching (Redis)
- Tune connection limits

---

### **7. Architectural Improvement for Latency**

**Question:**  
Load testing shows synchronous REST API calls causing latency. What architectural change would you consider to improve performance and resilience?

**Answer:**  
I would shift to **asynchronous communication** using **messaging queues** or **event-driven architecture**.  
This decouples services, improves throughput, and increases system resilience against cascading failures.

---

### **8. Microservice Communication Patterns**

**Question:**  
What microservice design patterns would you use for inter-service communication?

**Answer:**  
Use **message brokers** or **event-driven architecture** instead of direct synchronous calls.  
Options: **RabbitMQ**, **Kafka**, **AWS SNS/SQS**.  
This enables **eventual consistency** and **loose coupling** between services.

---

### **9. Kafka – Duplicate Message Issue**

**Question:**  
Your service consumes messages from Kafka and writes them to a database, but duplicate entries appear. How do you investigate and prevent it?

**Answer:**  
Investigate **Kafka delivery semantics** — by default, Kafka guarantees _at least once_ delivery.  
Check **consumer offset commits** — auto-commit may occur before full processing.

Prevention strategies:

- **Manual offset commits** after successful processing
- **Idempotent processing** (safe reprocessing without duplication)
- Use **UPSERT** instead of INSERT
- Add **unique constraints** or **primary keys** at DB level
- Enable **idempotent producers** (`enable.idempotence=true`)
- Use **Dead Letter Queues (DLQs)** for failed messages
- Monitor **consumer lag** and **retries**

---

### **10. CI/CD Pipeline Optimization**

**Question:**  
Your CI/CD pipeline takes over 25 minutes due to many tests and build steps. How would you optimize it?

**Answer:**  
Steps:

1. **Identify bottlenecks** – check slow tests, builds, or sequential stages.
2. **Parallelize independent steps** – run linting, unit tests, and static analysis concurrently.
3. **Optimize tests** – run only affected or changed test cases.
4. **Split test suites** into smaller shards for parallel execution.
5. **Use caching** – for dependencies, build artifacts, and Docker layers.
6. **Incremental builds** – rebuild only changed modules.

This reduces feedback time and improves developer productivity.

---

### **11. Structuring Large Node.js Lambda Functions**

**Question:**  
Your Node.js Lambda function has become large and complex. How would you structure and package it for better maintainability and performance?

**Answer:**

- **Modularize code:** Split logic into smaller modules with single responsibility.
- **Use AWS Lambda Layers:** Package shared dependencies separately to reduce deployment size and duplication.
- **Minimize dependencies:** Include only runtime dependencies, exclude dev ones.
- **Optimize cold starts:** Keep Lambda lightweight; move heavy initialization outside the handler.
- **Implement lazy loading:** Load large libraries only when needed.
- **Store deployment artifacts in S3** for efficient management.

This ensures better performance, faster deployment, and maintainable architecture.

---

**End of Document**
