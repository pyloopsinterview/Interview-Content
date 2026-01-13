# Python Backend / FastAPI – Interview Questions & Answers

---

## 1. How do you structure and modularize Python backend services?

**Answer:**  
I use a **feature-based modular architecture** with **clear separation of concerns**. Each feature contains its own **router/controller, service, repository, models, and schemas**. This keeps the code **scalable, testable, and easy to evolve**, and allows a **modular monolith** to later split into microservices if needed.

---

## 2. How do you design a medium-sized Python backend service?

**Answer:**  
For a medium-sized system, I prefer a **modular monolith**:

- Single deployable unit  
- Feature-based modules  
- Centralized **config, logging, auth**  
- Async only where needed  

This avoids microservice overhead while maintaining **clean boundaries** and **scalability**.

---

## 3. What are common issues in APIs that query a database?

**Answer:**  
Common issues include:

- **Slow queries** (missing indexes, N+1 queries)  
- **Connection pool exhaustion**  
- **Long-running transactions & locks**  
- **Scalability bottlenecks**  
- **Poor error handling**  
- **Security risks** (SQL injection, over-privileged users)  

I mitigate these with **query optimization, pooling, caching, async processing, and observability**.

---

## 4. How does FastAPI use Python type hints?

**Answer:**  
FastAPI uses **type hints as the API contract**. They define:

- Request parameters  
- Request bodies  
- Response models  
- Dependency injection  

Type hints enable **automatic validation, parsing, and OpenAPI documentation**.

---

## 5. What role does Pydantic play in FastAPI?

**Answer:**  
**Pydantic** handles:

- **Runtime data validation**  
- **Type coercion**  
- **Serialization/deserialization**  
- **Schema enforcement**  

Invalid data automatically returns a **422 validation error**, reducing boilerplate and bugs.

---

## 6. How does Dependency Injection work in FastAPI?

**Answer:**  
FastAPI uses **Depends()** with type hints to **declare dependencies**.

FastAPI then:

- Creates the dependency  
- Injects it into the endpoint  
- Manages lifecycle and cleanup  

This improves **loose coupling, reusability, and testability**.

---

## 7. Can you explain Dependency Injection with an example?

**Answer:**  
A common example is injecting a **database session**:

- Define a dependency that yields a DB session  
- Inject it into endpoints using `Depends()`  

FastAPI ensures **safe creation and cleanup** for every request.

---

## 8. When do you use async in FastAPI?

**Answer:**  
I use **async** when the code is **I/O-bound and non-blocking**, such as:

- Async database calls  
- External API requests  
- File I/O  
- Message queues  

Async improves **throughput and concurrency**.

---

## 9. When should you avoid async in FastAPI?

**Answer:**  
I avoid async when:

- Code is **CPU-bound**  
- Using **blocking libraries**  
- Performing heavy computations  

In such cases, I use **sync endpoints**, **background workers**, or **task queues**.

---

## 10. What happens if async code is written incorrectly?

**Answer:**  
Incorrect async usage can:

- **Block the event loop**  
- Reduce concurrency  
- Cause timeouts and crashes  

Examples include calling `time.sleep()` or sync DB code inside async functions.  
Solution: **use non-blocking calls or offload work**.

---

## 11. How do you design REST endpoints for fraud systems?

**Answer:**  
I design fraud APIs to be:

- **Domain-driven**  
- **Idempotent**  
- **Audit-friendly**  
- **Secure**  

Endpoints focus on **transactions, risk scores, alerts, and decisions**, with strict validation and traceability.

---

## 12. How do you design REST endpoints for event-driven systems?

**Answer:**  
Event APIs are:

- **Immutable**  
- **Idempotent**  
- **Async by design**  

I avoid updates/deletes and rely on **event IDs**, **message queues**, and **at-least-once delivery** with deduplication.

---

## 13. How do you design REST endpoints for data platforms?

**Answer:**  
I separate:

- **Metadata** (datasets, schemas)  
- **Execution** (jobs, pipelines)  
- **Data access**  

Most operations are **async**, returning **job IDs** for status tracking.

---

## 14. What is idempotency in REST APIs?

**Answer:**  
Idempotency ensures that **repeating the same request produces the same result**, without duplicate side effects.  
It is critical for **POST APIs** in distributed systems.

---

## 15. How do you implement idempotency in REST APIs?

**Answer:**  
I implement idempotency by:

- Using an **Idempotency-Key** header  
- Storing request state and response in **Redis or DB**  
- Returning the stored response on retries  

This prevents **duplicate processing** during retries.

---

## 16. Why is idempotency important in fraud and payment systems?

**Answer:**  
Because retries are common due to **timeouts or network failures**.

Without idempotency, retries can cause:

- Duplicate charges  
- Duplicate fraud alerts  
- Inconsistent data  

Idempotency ensures **safety and correctness**.

---

## 17. How do you handle long-running operations in APIs?

**Answer:**  
I use **async workflows**:

- Submit job → return job ID  
- Process in background  
- Poll job status or emit events  

This keeps APIs **responsive and scalable**.

---

## 18. How do you ensure API security?

**Answer:**  
I use:

- **JWT / OAuth2**  
- **RBAC**  
- Input validation  
- Least-privilege DB access  
- Audit logging  

This is especially important for **fraud and healthcare systems**.

---

## 19. How do you ensure observability in backend services?

**Answer:**  
I include:

- **Structured logging**  
- **Metrics**  
- **Health checks**  
- **Tracing & correlation IDs**  

This enables **fast debugging and incident response**.

---

## 20. Why are you planning to move from your current role?

**Answer:**  
My current project is **nearing completion**, and I’m actively handling **knowledge transfer**.

I’m looking for my next role where I can contribute to **long-term, impactful backend systems** and continue growing technically.

---

## 21. How do you handle knowledge transfer at the end of a project?

**Answer:**  
I document:

- Architecture  
- APIs  
- Data flows  
- Runbooks  

I also conduct **KT sessions** and ensure the team is comfortable before transitioning out.

---

## 22. How do you decide between a modular monolith and microservices?

**Answer:**  
I start with a **modular monolith** for simplicity.

I move to microservices only when there’s a clear need for **independent scaling, ownership, or deployment**.

---

## 23. One-line summary of your backend design philosophy

**Answer:**  
I design backend systems to be **modular, idempotent, observable, and scalable**, with a strong focus on **domain-driven design and production reliability**.
