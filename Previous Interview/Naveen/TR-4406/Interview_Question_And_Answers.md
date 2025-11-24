Below is the **complete Markdown file** containing **all questions you asked during the interview** along with **strong, experience-based answers** aligned to your Java + Kubernetes + Event-Driven profile.

---

# **Java + Kubernetes Engineer – Interview Q&A (Markdown File)**

### **Based on all questions asked in the conversation**

---

## **1. Brief Introduction**

**Q: Give me a brief introduction.**
**A:**
“Hi, my name is Naveen. I have 12+ years of experience as a Lead Java Engineer with strong hands-on expertise in Java, Kubernetes, AWS, and event-driven microservices. Recently at Roswell Park, I worked on a Clinical Data Integration Platform with 120+ microservices running on EKS. I designed event-driven services using Java/Kotlin, SNS/SQS, Kinesis, clean architecture, and domain-driven design. I built core services like the Clinical Events Orchestrator, handled end-to-end ownership—design, development, integration testing, Dockerization, EKS deployment, autoscaling, OpenTelemetry tracing, GitLab CI/CD—and ensured security compliance including encryption, RBAC, and HIPAA. My experience aligns strongly with Java, Kubernetes, AWS, and scalable event-driven architectures.”

---

## **2. What does partition key design mean in DynamoDB?**

**Q: What do you mean by designing partition keys?**
**A:**
“We used a timeline-based partition key design in DynamoDB. For each patient we used `PATIENT#<patientId>` as the partition key and a sort key like `EVENT#<eventType>#<timestamp>`. This lets us query all clinical events for a patient chronologically, ensures fast lookups, avoids scans, and prevents hot partitions. It was ideal for clinical event timelines.”

---

## **3. Why did you choose DynamoDB for medical data?**

**Q: Why did you use DynamoDB to store medical data?**
**A:**
“Clinical event data is high-volume, time-series, and requires fast ingestion. RDBMS would struggle with scale, sharding, and heavy writes. DynamoDB gives us massive scalability, low-latency reads/writes, flexible schema for diverse clinical events, AWS-native integration with SNS/SQS/Kinesis, cost efficiency, and built-in security features like encryption, IAM, VPC endpoints, and PITR—all required for HIPAA compliance.”

---

## **4. In what format did you receive medical data?**

**Q: What file formats did you receive medical data in?**
**A:**
“We handled structured formats only—no scanned documents. Main formats were FHIR JSON, HL7v2 (converted to JSON), domain-specific JSON events, XML (converted to JSON), and occasional CSV for batch loads. All data entering our system was structured and machine-readable.”

---

## **5. What practical file types did you work with?**

**Q: Tell me the practical file types you handled.**
**A:**
“FHIR JSON, HL7 v2 messages, standard JSON event payloads, XML (converted to JSON), and CSV for batch ingestion.”

---

## **6. Why do you create a class?**

**Q: Why do you create classes in your program?**
**A:**
“To isolate responsibilities, give structure to raw JSON, enable clean domain models, separate parsing/validation logic, ensure clean architecture, improve testability, and make the service maintainable and extensible. For every new event type, data flow, or external integration, a new class ensures clarity and modular design.”

---

## **7. How is creating a class for clinical events beneficial?**

**Q: How does creating a ClinicalEvent class help?**
**A:**
“It gives us strong typing, predictable structure, reusability across layers, clear separation of concerns, easier testing, and maintainability. Downstream services depend on consistent event models, so defining a class ensures stability and clean data flow.”

---

## **8. What are the primitive types in Java?**

**Q: What primitive types have you used?**
**A:**
“int, long, float, double, boolean, char, byte, and short.”

---

## **9. Can primitives be objects?**

**Q: Can primitive types be objects?**
**A:**
“No. But Java provides wrapper classes like Integer, Long, Boolean, etc.”

---

## **10. Have you used Java collection classes?**

**Q: Have you worked with Java collections?**
**A:**
“Yes. I use Lists, Sets, Maps, Queues, and Stream APIs extensively in transformation layers, event processing pipelines, and data manipulation.”

---

## **11. When do you use a Queue vs a List?**

**Q: When would you choose a Queue, and when would you choose a List?**
**A:**
– **Queue:** When I need FIFO behavior or sequential event processing.
– **List:** When I need ordered data, random access, iteration, sorting, filtering, or transformation.

---

## **12. Difference between Hashtable and HashMap**

**Q: What’s the difference between Hashtable and HashMap?**
**A:**
– Hashtable is synchronized, slower, and does not allow null keys/values.
– HashMap is not synchronized, faster, modern, and allows nulls.
In real work, I use HashMap or ConcurrentHashMap—not Hashtable.

---

## **13. What data structure do you use to sort key-value pairs by key?**

**Q: If you need sorted key-value pairs by key, what do you use?**
**A:**
“A TreeMap—it keeps keys sorted automatically.”

---

## **14. What are the HTTP methods?**

**Q: What are the main HTTP methods?**
**A:**
“GET, POST, PUT, PATCH, DELETE, OPTIONS, HEAD.”

---

## **15. How would you design an employee info web service end-to-end?**

**Q: Walk me through designing a simple API to get employee info.**
**A:**
– Define API contract (GET /employees/{id})
– Create domain model
– Build repository layer
– Build service layer
– Build controller
– Add security
– Add logging/monitoring
– Write tests
– Containerize with Docker
– Deploy to Kubernetes
– Automate with GitLab CI/CD

---

## **16. How do you secure an API using JWT?**

**Q: Explain how you secure an API using JWT.**
**A:**
– Expect JWT in Authorization header
– Validate signature, expiry, issuer, audience
– Extract claims (userId, roles)
– Build SecurityContext
– Apply role-based access rules
– Log and monitor
– Store secrets safely (Kubernetes Secrets / AWS Secrets Manager)

---

# **End of Markdown File**

If you want, I can also prepare:
– a **PDF version**
– an **interview cheat sheet**
– a **rapid-fire Q&A list**
– a **Kubernetes-focused Q&A file**
