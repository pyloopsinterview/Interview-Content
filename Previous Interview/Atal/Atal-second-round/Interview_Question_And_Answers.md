# Interview Questions & Answers (Extracted)

## 1. What is Spring Boot and how does it work?
**Answer:**
Spring Boot simplifies building Java applications by providing auto-configuration, embedded servers, and convention over configuration. It uses dependency injection and inversion of control to manage components.

---

## 2. What is Inversion of Control (IoC)?
**Answer:**
IoC means the control of object creation and dependency management is handled by the framework instead of the developer.

---

## 3. What are the types of Dependency Injection?
**Answer:**
- Constructor Injection (recommended)
- Setter Injection
- Field Injection

**Preferred:** Constructor Injection because:
- Makes dependencies explicit
- Improves testability
- Supports immutability

---

## 4. How do you handle Null Pointer Exceptions in Java?
**Answer:**
- Use Optional (Java 8+)
- Null checks
- Avoid returning null
- Use defensive coding
- Use annotations like @NotNull

---

## 5. Do you use assertions?
**Answer:**
Assertions can be useful for debugging but are not recommended for production validation. Prefer proper exception handling and validation logic.

---

## 6. How do you test fault tolerance in microservices?
**Answer:**
- Unit testing
- Integration testing
- Chaos engineering
- Load testing
- Circuit breakers (Resilience4j)

---

## 7. How do you identify bottlenecks in microservices?
**Answer:**
- Monitoring tools
- Logging
- Performance testing
- Distributed tracing
- Load testing

---

## 8. How would you design a system to process high-volume stock market data?
**Answer:**
- Use Kafka for ingestion
- Streaming processing (Kafka Streams)
- Fast DB (Cassandra) for real-time
- Data lake (S3) for storage

---

## 9. How do you avoid duplicate processing in Kafka?
**Answer:**
- Use unique IDs
- Idempotent producers
- Transactional processing

---

## 10. How do you handle latency spikes in distributed systems?
**Answer:**
- Load balancing
- Partitioning
- Scaling consumers
- Monitoring

---

## 11. Which language/framework would you use for stream processing?
**Answer:**
- Java (Kafka Streams / Spring Boot)
- Python (optional)

---

## 12. How do you design a multi-region high availability system?
**Answer:**
- Active-active architecture
- Health checks
- Load balancing
- Failover strategies
- Data replication

---

## 13. How do you maintain data consistency across regions?
**Answer:**
- Centralized writes or reservation system
- Eventual consistency for reads
- Strong consistency for critical operations

---

## 14. How do you prevent overselling in inventory systems?
**Answer:**
- Avoid stale reads during checkout
- Use strong consistency
- Reserve inventory during purchase
- Use transactional systems

---

## 15. What is Chaos Engineering?
**Answer:**
Chaos Engineering is testing system resilience by intentionally introducing failures to observe behavior and improve reliability.

---

