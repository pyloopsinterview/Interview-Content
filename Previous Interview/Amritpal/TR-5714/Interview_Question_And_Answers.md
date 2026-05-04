# Interview Q&A – Senior Python Backend Engineer

---

## Q1: Could you pick a monolith that you broke apart and walk through what you did?

### Answer:
One of the most relevant examples was at AmerisourceBergen, where I worked on a healthcare supply-chain platform.

The system was a tightly coupled monolith built using PHP and Python on on-prem infrastructure. It was difficult to scale, deploy, and maintain.

I started by analyzing the architecture and identifying domain boundaries like order management, inventory, and user services.

We followed an incremental approach:
- Extracted services one by one
- Containerized them using Docker
- Deployed on GKE

We also upgraded Python to 3.11, implemented mTLS security, and introduced CI/CD pipelines.

We improved observability using Prometheus and Grafana.

**Result:** Better scalability, independent deployments, and improved system reliability.

---

## Q2: Could you pick one service you decoupled?

### Answer:
We started with the Order Management Service.

It handled order creation, validation, and status updates, and was tightly coupled with inventory, payment, and user modules.

Steps:
- Defined domain boundaries
- Extracted logic into a Python microservice
- Initially shared DB → later moved to separate DB
- Used REST + event-driven communication

We added monitoring and ensured secure communication.

**Result:** Independent scaling, faster releases, and failure isolation.

---

## Q3: Which modules were coupled and how did you break it using events?

### Answer:
The Order module was tightly coupled with:
- Inventory (stock check)
- Payment (processing)
- User service (validation)

Everything ran in a single synchronous transaction.

We moved to event-driven architecture:

Flow:
- Order Service creates order → `PENDING`
- Publishes `OrderCreated`
- Inventory + Payment services consume events
- Emit success/failure events
- Order Service updates status

We used:
- Idempotency
- Retries
- Eventual consistency

---

## Q4: How did you break the synchronous transaction? What was step one?

### Answer:
Step-by-step:

1. Identify transaction boundary
2. Introduce `PENDING` state
3. Publish `OrderCreated` event
4. Move external calls outside transaction
5. Handle responses via events
6. Add retries, DLQ, idempotency

We used a hybrid model initially to reduce risk.

---

## Q5: What triggered the next steps after order creation?

### Answer:
We used an event-driven approach via Google Pub/Sub.

Flow:
- Order Service publishes `OrderCreated`
- Inventory + Payment services subscribe
- They process and emit events
- Order Service updates state

We avoided polling due to latency and inefficiency.

---

## Q6: Did you move from on-prem to GCP?

### Answer:
Yes, we followed a phased migration:

- New services deployed on GKE
- Monolith remained on-prem initially
- Set up secure VPN + mTLS
- Gradually migrated services and dependencies
- Moved monitoring, messaging, CI/CD to cloud

**Result:** Hybrid → Fully cloud-native system.

---

## Q7: Experience with version migrations?

### Answer:
I have worked on:

- Python 2 → Python 3.11
- PHP upgrades
- RHEL 7 → RHEL 8/9
- OpenSSL upgrades
- Monitoring/logging migrations

Approach:
- Impact analysis
- Incremental rollout
- Strong testing
- Backward compatibility

---

## Q8: Example of a migration you did?

### Answer:
Python 2.7 → Python 3.11 migration.

Steps:
- Code analysis for deprecated modules
- Incremental refactoring
- Dependency upgrades
- Strong testing
- Canary deployments

**Result:** Better performance, security, and maintainability.

---

## Q9: Differences between Python 3.9 and 3.11?

### Answer:
Key differences:

- Performance (20–40% faster)
- Better error messages
- Improved exception handling
- New features (Exception Groups)
- Better async support

**Impact:** Faster APIs, better debugging, improved efficiency.

---

## Q10: When to use asyncio vs threading?

### Answer:

**asyncio:**
- I/O-bound tasks
- Non-blocking operations
- High concurrency

**threading:**
- Blocking libraries
- Legacy integrations

**CPU-bound:**
- Use multiprocessing (due to GIL)

---

## Q11: Questions to ask interviewer

### Suggested Questions:

- What would success look like in the first 3–6 months?
- What are the biggest technical challenges currently?
- Is the system hybrid or fully on GCP?
- How are teams structured?
- How do you approach CI/CD and code quality?

---

# End of Document