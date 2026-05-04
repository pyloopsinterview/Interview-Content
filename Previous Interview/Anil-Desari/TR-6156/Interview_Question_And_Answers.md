# Detailed Interview Q&A (Full Version)

---

## 1. Question:
"Could you sort of go a little deep and a little wide with what the differences between BigQuery and Postgres are, and what one might be good at versus another?"

### Answer:

At a high level, BigQuery and PostgreSQL are designed for completely different workloads.

PostgreSQL is a traditional OLTP database, optimized for transactional workloads. It handles inserts, updates, deletes, and ensures ACID compliance with strong consistency. It is ideal for application backends where low latency and real-time operations are required.

BigQuery, on the other hand, is a serverless OLAP data warehouse designed for analytical workloads. It uses columnar storage and is optimized for scanning large datasets and running aggregations across billions of rows.

Architecturally:
- PostgreSQL is typically single-node or vertically scaled.
- BigQuery is massively distributed and serverless.

Performance:
- PostgreSQL → low latency, small queries
- BigQuery → high throughput, large analytical queries

Use cases:
- PostgreSQL → application database
- BigQuery → analytics, reporting, data warehouse

---

## 2. Question:
"If you’re running an application in Kubernetes with many pods and want it to scale elastically, what techniques would you use?"

### Answer:

From a Kubernetes perspective:
- Use Horizontal Pod Autoscaler (HPA)
- Scale based on custom metrics like queue length
- Use KEDA for event-driven scaling
- Configure resource requests/limits
- Use cluster autoscaler

From application side:
- Stateless workers
- Queue-based processing
- Work chunking
- Idempotent processing
- Retry mechanisms and dead-letter queues

---

## 3. Question:
"What are some Kubernetes-native scaling techniques vs application-level techniques?"

### Answer:

Kubernetes:
- HPA (CPU/memory/custom metrics)
- KEDA
- Cluster autoscaler
- Probes (liveness/readiness)

Application:
- Stateless design
- Pull-based queues
- Work partitioning
- Idempotency
- Backpressure handling

---

## 4. Question:
"If you're streaming writes to BigQuery, and you don’t want workers to manage state, how would you design that?"

### Answer:

- Workers remain stateless
- Externalize state into DB or queue
- Use insertId for deduplication
- Micro-batch writes
- Retry failures safely
- Track progress externally

---

## 5. Question:
"How would you ensure streaming writes were successful in an eventually consistent system?"

### Answer:

Use pattern:
Write → Track → Validate → Reconcile

- Idempotent writes
- Track expected records
- Retry failures
- Delayed validation
- Reconciliation jobs
- Partition-based validation

---

## 6. Question:
"Can you explain the Visitor Pattern and how you might use it?"

### Answer:

Visitor Pattern separates operations from object structure.

Use when:
- Object structure is stable
- Operations change frequently

Example:
- accept() method in objects
- visit() method in visitor

Used in:
- data validation
- transformations
- metadata extraction

---

## 7. Question:
"What’s the difference between unit tests and integration tests?"

### Answer:

Unit tests:
- Test individual logic
- Fast
- Use mocks

Integration tests:
- Test system components together
- Use real dependencies

Best practice:
- Majority unit tests
- Some integration tests

Run:
- Unit → local + CI
- Integration → CI + staging

---

## 8. Question:
"What questions do you have for me?"

### Answer:

- Can you explain current architecture?
- How do you handle scaling?
- How do you manage monitoring and validation?
- What are current challenges?
- What does success look like?

---

