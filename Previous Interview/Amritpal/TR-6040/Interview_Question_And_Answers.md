````md id="v4m8qp"
# Interview Questions with Correct Answers (Today)

---

## 1. How would you design a scalable data model for complex loan processing workflows in banking and financial regulatory systems?

### Correct Answer
For complex loan processing, I would design the data model using a **state-driven and event-driven architecture**.

Instead of a single loan table, I would separate the system into core entities:

### Loan Master Table
- loan_id
- customer_id
- product_type
- loan_amount
- interest_rate
- tenure
- current_status
- created_at

### Loan State History Table
This is critical for audit and compliance.

- id
- loan_id
- previous_state
- current_state
- transition_timestamp
- changed_by
- remarks

Example lifecycle:

`SUBMITTED → KYC_PENDING → VERIFIED → UNDER_REVIEW → APPROVED → DISBURSED`

I would also create separate tables for:

- document verification
- risk scoring
- repayment schedule
- audit logs
- compliance workflow

For scalability, each state transition should publish events using Kafka or SQS so other systems like notifications, fraud detection, and reporting can consume asynchronously.

This ensures:

- scalability
- traceability
- compliance
- fault tolerance

---

## 2. What are your optimization steps for a severely slow REST API endpoint relying on complex SQL joins?

### Correct Answer
My approach is always:

**profile → identify → optimize → benchmark**

### Step 1: Identify bottleneck
Check whether latency is coming from:

- API layer
- business logic
- ORM
- SQL
- network

### Step 2: Analyze SQL query
Run:

`EXPLAIN ANALYZE`

Look for:

- full table scans
- missing indexes
- nested loops
- expensive sort operations

### Step 3: Optimize indexes
Create indexes on:

- JOIN columns
- WHERE filters
- ORDER BY
- GROUP BY

### Step 4: Rewrite SQL
- remove unnecessary joins
- avoid `SELECT *`
- fetch only required columns
- filter earlier

### Step 5: Fix ORM issues
Check N+1 query problem.

For example in Django:

- select_related
- prefetch_related

### Step 6: Add caching
Use Redis for repeated reads.

### Step 7: Pagination
Apply limit / offset or cursor-based pagination.

### Step 8: Benchmark
Load test before and after optimization.

---

## 3. If you encounter a memory leak while processing thousands of massive financial files, how would you profile it?

### Correct Answer
First, I verify whether it is a real memory leak or simply high memory consumption.

### Steps
1. Use tools like:
   - memory_profiler
   - tracemalloc
   - psutil

2. Track memory over time.

3. Compare snapshots:
   - before batch
   - after 100 files
   - after 500 files

4. Identify leaking function.

5. Check common causes:
   - full file loading
   - dataframe copies
   - unclosed file handles
   - DB sessions
   - worker process retention

6. Prefer chunk-based processing:

`pd.read_csv(file, chunksize=10000)`

7. Validate fix using long-running batch tests.

---

## 4. Create a real-world scenario for a custom decorator or context manager.

### Correct Answer

### Decorator Example
Use case: centralized logging and performance monitoring

```python
def monitor_execution(func):
    def wrapper(*args, **kwargs):
        start = time.time()
        result = func(*args, **kwargs)
        print(time.time() - start)
        return result
    return wrapper
````

Use it for:

* API timing
* exception logging
* audit logs
* retries

### Context Manager Example

Use case: database transaction handling

```python
with TransactionManager(db_session):
    update_loan()
    insert_audit_log()
```

Best for:

* automatic commit
* rollback
* session close

---

## 5. How do you architect a backend system to ensure sensitive data is tokenized or encrypted at rest and in transit?

### Correct Answer

### In Transit

* HTTPS
* TLS 1.2 / 1.3
* mutual TLS for service-to-service calls

### At Rest

* AES-256 encryption
* AWS KMS
* RDS encryption
* S3 SSE

### Sensitive Fields

For fields like:

* SSN
* account number
* routing number
* PII

I use tokenization.

Example:

`123456789 → TOK_ABC123`

### Key Management

* AWS KMS
* Secrets Manager
* key rotation

### Access Control

* RBAC
* masked data display
* audit logs

---

## 6. How do you inject database credentials securely into Kubernetes pods?

### Correct Answer

My approach is:

**AWS Secrets Manager + CSI Driver + IRSA**

### Flow

`Secrets Manager → CSI Driver → Pod mounted secret`

Best practices:

* never hardcode secrets
* runtime injection
* IAM role-based access
* mounted volume preferred
* automatic rotation
* least privilege

---

## 7. What are the most common causes of memory leaks in React / Angular / Vue SPAs?

### Correct Answer

Most common causes are:

* event listeners not removed
* uncleared intervals / timeouts
* unsubscribed RxJS observables
* stale closures
* detached DOM nodes
* websocket connections not closed
* large retained application state
* async calls updating unmounted components

These issues gradually degrade SPA performance.

---

## 8. Which frontend framework do you mostly prefer?

### Correct Answer

I have worked with React, Angular, and Vue, but **React is my strongest and most preferred framework**.

Reasons:

* component-based architecture
* reusable components
* hooks
* excellent ecosystem
* easier scalability
* strong state management options

---

## 9. How do you prevent runaway cloud costs in serverless architectures?

### Correct Answer

My approach is **controlled elasticity**.

### Key Controls

* concurrency limits
* throttling
* batching using SQS / Kafka
* right-sized memory
* retry limits
* dead-letter queue
* caching
* budget alerts
* CloudWatch billing alarms

### Database Control

* RDS Proxy
* DynamoDB TTL
* autoscaling thresholds

This ensures scalability without unexpected cloud bills.


