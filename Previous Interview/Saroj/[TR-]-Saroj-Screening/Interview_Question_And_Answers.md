# Saroj Interview: Full Stack Developer / Tech Lead Role

## Role Context
- Full Stack Developer / Full Stack Tech Lead
- Skills highlighted: Java, Python, JavaScript, AWS, Microservices, LLMs, React

---

## Q1: Microservices vs Monolithic Architecture  
**Question:**  
What do microservices solve compared to monolithic architecture?  
When would you *not* choose microservices?

**Answer:**  
- **Monolithic issues:** Tightly coupled UI, business logic, DB; hard to scale/deploy; small changes impact entire app.  
- **Microservices solve:** Break system into small, independent services (e.g., order, inventory). Each is scalable, deployable independently.  
- **When NOT to use microservices:**  
  - App is small or not complex → microservices add unnecessary operational overhead (distributed tracing, API gateway, service discovery).  
  - Team lacks DevOps maturity.  
  - Unclear domain boundaries → leads to tight coupling across services.  
  - In such cases, modular monolithic is better.

---

## Q2: Database per Microservice?  
**Question:**  
Should each microservice have its own database?

**Answer:**  
- ✅ **Yes, generally.** It maintains loose coupling and service independence.  
- Sharing a DB creates tight coupling — changes in one service impact others.  
- Separate DB ownership allows each service to choose best DB type (e.g., Postgres for transactions, MongoDB for flexible/high-volume data).  
- **Exception:** not mandatory in all cases, but highly recommended.

---

## Q3: Synchronous vs Asynchronous Communication  
**Question:**  
When do you choose synchronous vs asynchronous communication in microservices?

**Answer:**  
- **Synchronous (e.g., REST APIs):**  
  - When immediate response is needed (e.g., payment validation, inventory check in real-time).  
  - Downside: tight coupling, latency, cascading failures.  
- **Asynchronous (e.g., message queues, event-driven):**  
  - When operation is not time-critical (e.g., send notifications, update analytics, inventory sync after order).  
  - Improves resilience, reduces blocking, better handling of spikes.  
- **Mix of both:** synchronous for real-time ops, async for background tasks.

---

## Q4: Modeling Metadata for 5,000+ Sources  
**Question:**  
How would you model metadata for ~5,000 sources (tables, files, columns, events)?

**Answer:**  
- Treat metadata as a separate domain.  
- Build **centralized metadata service** as single source of truth.  
- Storage:  
  - Postgres for strong relationships (source → tables → columns).  
  - MongoDB for dynamic/nested data.  
  - Hybrid approach if needed.  
- Optimizations: indexing, pagination, filtering APIs, caching, read replicas.  
- Communication: other services interact via REST/GraphQL APIs — no direct DB access.  
- Event-driven updates: publish events when metadata changes.

---

## Q5: Handling Latency — Product Enrollment by 1,000 Customers  
**Question:**  
1,000 customers enrolling 1,000 products simultaneously — high latency. How do you handle it?

**Answer:**  
- **Asynchronous processing:** Accept request quickly, push to message queue (Kafka/RabbitMQ), return acknowledgment; process in background.  
- **Bulk processing & batching:** Group operations instead of one-by-one.  
- **Horizontal scaling:** Multiple workers on AWS.  
- Reduces blocking calls and API latency.

---

## Q6: Caching & Cost Control for LLM Calls  
**Question:**  
LLMs are expensive. How do you implement caching and cost control?

**Answer:**  
- **Multilevel caching:**  
  - Response caching (Redis/in-memory) for repeated queries.  
  - Embedding caching.  
  - Vector search result caching.  
- **Cache key normalization:** lowercase, remove noise, hash-based keys.  
- **TTL-based eviction** (1–24 hours depending on data freshness).  
- **Optimize RAG pipelines:** only top-k relevant chunks, smaller context window.

---

## Q7: LLM Feature Causes Quality Degradation — How to Roll Back?  
**Question:**  
After adding a new feature, LLM service quality degrades. How do you roll back safely?

**Answer:**  
- **Track metrics:** accuracy, latency, user feedback — compare before/after.  
- **Offline evaluation:** golden dataset + regression testing.  
- **Canary release:** gradual rollout (5% → 20% → 50% → 100%).  
- **Version everything:** model versions, prompt templates, RAG pipelines.  
- **Feature flags + traffic routing:** disable new feature instantly; redirect 100% traffic to old stable version → zero downtime rollback.

---

## Q8: Terraform State Lock Error  
**Question:**  
Two pipelines try to apply Terraform changes on same state (70 existing + 4 new resources). Build fails with `state lock` error. How to resolve?

**Answer:**  
- Terraform uses state locking to prevent concurrent modifications.  
- **Check** if another apply is actually running → wait & retry.  
- If lock remains after pipeline fails → manually release:  
  `terraform force-unlock <LOCK_ID>`  
- **Prevent recurrence:**  
  - Use remote backend with locking (S3 + DynamoDB).  
  - Pipeline serialization.  
  - Separate state files per environment (workspaces).  
  - Approval steps in Jenkins.

---

## Q9: Feature Gating in React Without Duplicating Backend  
**Question:**  
How to implement frontend feature gating without duplicating backend logic?

**Answer:**  
- Backend is **single source of truth** — sends user roles/permissions via token or user-info API.  
- On frontend: store permissions in React Context API or Redux.  
- Create reusable `hasPermission()` utility function.  
- Use Higher-Order Components (HOCs) for reusability.  
- Conditional rendering: hide/show components, enable/disable buttons, restrict routes via guards.  
- No hardcoding — backend permissions drive everything.

---

## Q10: Preventing Prompt Injection & Data Leakage in LLMs (Healthcare/HIPAA)  
**Question:**  
How do you prevent prompt injection and data leakage for healthcare data (PHI/HIPAA)?

**Answer:**  
- Treat LLM as **untrusted**.  
- **RBAC at API layer** — only authorized users can retrieve sensitive chunks.  
- **Retrieval guard** — filter results based on user permissions before sending to LLM.  
- **Input validation & prompt sanitization** — block patterns like "ignore instructions", data exfiltration attempts.  
- **Data masking / tokenization** — remove or mask PHI before embedding or response generation.

---

## Q11: Observability — Definition & Approach  
**Question:**  
What is observability? How do you implement it?

**Answer:**  
Observability = understanding system internals from external data.  
- **Logs** — what happened exactly.  
- **Metrics** — CPU, latency, throughput.  
- **Traces** — request flow across services.

---

## Q12: Infrastructure as Code (IaC) — Terraform & State Management  
**Question:**  
What do you use for IaC? How do you manage Terraform state?

**Answer:**  
- **Primary:** Terraform. Also AWS CloudFormation.  
- Remote backend (S3 + DynamoDB) for state locking & consistency.  
- Separate state files per environment.  
- CI/CD pipeline: GitHub Actions/Jenkins → build → push to ECR → deploy to ECS.

---

## Q13: RAG — When and Why to Use It  
**Question:**  
What is RAG? When do you use it and why?

**Answer:**  
- **RAG = Retrieval + Generation**  
  - Retrieval: fetch relevant data from vector DB/knowledge base.  
  - Generation: LLM answers using retrieved context.  
- **Why use RAG:**  
  - Prevents hallucination.  
  - Provides real-time, domain-specific context.  
  - Essential for dynamic or private/enterprise data.  
  - Improves accuracy.

---

## Closing Notes from Interviewer  
- Moving to customer-level interview.  
- Role: Full Stack Developer (Healthcare — Cigna).  
- Required: Python, AWS, React, FastAPI/Django/Flask, SQL, Kubernetes, ETL, microservices.  
- Basics & fundamentals matter most.