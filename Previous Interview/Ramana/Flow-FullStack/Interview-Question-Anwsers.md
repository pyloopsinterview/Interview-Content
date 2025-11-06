# Interview Questions and Answers (Full Set)

> **Format:** Each question followed by a complete, technically detailed answer for quick study and interview preparation.

---

## 1. let's start this interview talking about yourself, talking about your previous experience, but not in terms of the companies and the projects you have been working during this time. Okay? Let's stay focused on the technologies that you have been working during this time. All right? So if you can brief me just for one to two minutes regarding this would be perfect. Okay? We don't need to get deep in details.

**Answer:**

---

---

## 2. Tell me about the relational databases and also NoSQL databases you have worked with.

**Answer:**

### Relational Databases (RDBMS):

- **MySQL / PostgreSQL** — Used for transactional workloads with ACID properties. Implemented normalized schemas, indexing, stored procedures, joins, and constraints. Tuned queries using EXPLAIN plans and caching.
- **PostgreSQL** — Leveraged advanced features like JSONB fields, window functions, and full-text search. Used for analytics-heavy use cases.

### NoSQL Databases:

- **MongoDB (Document-based)** — Used for flexible schemas such as user profiles, logs, and unstructured data. Utilized aggregation pipelines and secondary indexes.
- **Redis (Key-value, in-memory)** — Used for caching, sessions, and leaderboards to reduce DB load.
- **DynamoDB (AWS managed NoSQL)** — Used in serverless environments for scalable, low-latency data access with GSI, TTL, and transactional writes.

**Choosing between them:** RDBMS for data integrity and relationships; NoSQL for scalability, flexibility, and distributed systems.

---

## 3. Tell me about cloud AWS. Uh, as you mentioned, DynamoDB.

**Answer:**

- **AWS DynamoDB** is a fully managed NoSQL key-value/document database offering single-digit millisecond latency at any scale.
- Supports **auto-scaling**, **on-demand** or **provisioned throughput**, and **global tables** for multi-region replication.
- Features **conditional writes**, **TTL**, **streams** for event-driven architectures, and **transactions** for multi-item ACID consistency.
- Common use: session storage, product catalogs, IoT data ingestion, and event sourcing.

**Example architecture:** API Gateway → Lambda → DynamoDB → CloudWatch (monitoring)

---

## 4. Are you familiar with AWS? What services have you used?

**Answer:**

- **Compute:** EC2, Lambda, ECS, EKS
- **Storage:** S3, EBS, EFS
- **Database:** RDS (PostgreSQL/MySQL), DynamoDB
- **Networking:** VPC, Route53, CloudFront, Load Balancers (ALB/NLB)
- **Messaging/Streaming:** SQS, SNS, Kinesis
- **Monitoring:** CloudWatch, CloudTrail, X-Ray
- **Security:** IAM, KMS, Secrets Manager
- **Deployment:** CodePipeline, CodeBuild, CodeDeploy
- **Others:** API Gateway (REST/HTTP APIs), Cognito for authentication

Used combinations like:

- `API Gateway + Lambda + DynamoDB` for serverless apps.
- `ECS + ALB + RDS` for containerized microservices.

---

## 5. Implement a Blocking Queue in Java.

**Answer:**

```java
import java.util.*;
import java.util.concurrent.locks.*;

public class BlockingQueue<T> {
    private Queue<T> queue = new LinkedList<>();
    private int capacity;
    private Lock lock = new ReentrantLock();
    private Condition notFull = lock.newCondition();
    private Condition notEmpty = lock.newCondition();

    public BlockingQueue(int capacity) {
        this.capacity = capacity;
    }

    public void enqueue(T item) throws InterruptedException {
        lock.lock();
        try {
            while (queue.size() == capacity) {
                notFull.await();
            }
            queue.add(item);
            notEmpty.signal();
        } finally {
            lock.unlock();
        }
    }

    public T dequeue() throws InterruptedException {
        lock.lock();
        try {
            while (queue.isEmpty()) {
                notEmpty.await();
            }
            T item = queue.remove();
            notFull.signal();
            return item;
        } finally {
            lock.unlock();
        }
    }
}
```

**Explanation:** Uses ReentrantLock and Conditions for thread-safety. `enqueue()` blocks when full; `dequeue()` blocks when empty.

---

## 6. JWT tokens showing unauthorized access even when expired — how to fix?

**Answer:**

1. **Validate the `exp` claim** — Check if backend properly enforces expiration.
2. **Clock Synchronization** — Ensure all servers use NTP to avoid skew.
3. **Token Cache** — Avoid caching old validation results.
4. **Spring Security Configuration** — Ensure `ignoreExpiration` is false in JWT filter.
5. **Check Refresh Logic** — Ensure access tokens are refreshed before expiry.
6. **Test & Log** — Add logs for validation results and run test tokens.

**Fix:** Correct token verification configuration, sync system clocks, invalidate stale caches.

---

## 7. Profile update not showing immediately — what to do?

**Answer:**

- Ensure backend updates succeed and return the updated object.
- On frontend, update local state immediately after save.
- Invalidate or refetch data caches (React Query/Apollo) post-mutation.
- If CDN or Redis cache used, purge or refresh it.
- Add WebSocket/SSE updates for real-time reflection.

**Best practice:** Always rely on server’s updated response rather than local data.

---

## 8. Node.js API Gateway slow under load — how to optimize?

**Answer:**

1. **Add Monitoring:** Use APM, OpenTelemetry to find bottlenecks.
2. **Optimize Calls:** Parallelize independent requests with Promise.all.
3. **Implement Caching:** Use Redis/in-memory caching for repeated responses.
4. **Connection Reuse:** Use HTTP keep-alive for downstream calls.
5. **Timeouts/Circuit Breakers:** Prevent cascading failures.
6. **Avoid Blocking Code:** Offload CPU-heavy work or use worker threads.
7. **Scale Horizontally:** Deploy behind a load balancer.
8. **Compression & Streaming:** Use GZIP and stream large payloads.

---

## 9. Downstream consumers failing after API update — how to manage versioning?

**Answer:**

- **Backward Compatibility:** Prefer additive changes.
- **Versioning:** `/v1`, `/v2` endpoints or header-based versions.
- **Contract Testing:** Use Pact for consumer-driven contracts.
- **Deprecation Policy:** Keep old versions active temporarily.
- **API Gateway:** Route based on version headers.
- **Monitoring:** Track consumer usage by API version.

---

## 10. Synchronous REST calls causing latency — how to improve?

**Answer:**

- **Asynchronous Messaging:** Replace sync calls with Kafka/SQS.
- **Event-Driven Architecture:** Services publish/subscribe to events.
- **CQRS Pattern:** Split read/write models to reduce coupling.
- **Caching:** Use Redis or local cache for frequent data.
- **Circuit Breakers:** Avoid cascading failures.
- **Bulkhead Pattern:** Isolate dependencies.

---

## 11. Kafka consumers missing events — how to prevent data loss?

**Answer:**

**Causes:**

- Offsets committed before processing.
- Consumer crashes.
- Deserialization errors.
- Retention too short.

**Prevention:**

- Commit offsets **after successful processing**.
- Use **idempotent consumers**.
- Implement **DLQ** (Dead Letter Queue).
- Add retries with exponential backoff.
- Monitor **consumer lag**.
- Use **Kafka transactions** for exactly-once semantics.

---

## 12. Node.js Lambda slow after inactivity — cause and mitigation.

**Answer:**

**Cause:** Cold start delays — Lambda container initialization after idle period.

**Fixes:**

- Enable **Provisioned Concurrency**.
- Keep functions **small** and **lightweight**.
- Use **keep-alive pings** or scheduled warm-ups.
- Avoid unnecessary **VPC configuration**.
- Use **API Gateway caching** and **CloudFront edge caching**.

**Measure with CloudWatch or X-Ray** to verify improvement.

---

**End of Document** ✅
