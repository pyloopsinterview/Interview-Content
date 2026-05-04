# Interview Q&A - Python, FastAPI, Vue.js, CI/CD, AI/LLM

---

## 1. System Design

**Q:** How would you design a highly available web application on AWS for a million users?

**A:**

* Use Route 53 for DNS and health checks.
* Application Load Balancer (ALB) to distribute traffic.
* Containerized services on Kubernetes or ECS deployed across multiple Availability Zones.
* Backend microservices using FastAPI.
* Event-driven communication with Kafka.
* Data storage: RDS (Multi-AZ), Redis for caching, S3 for static assets.
* CloudFront for CDN caching.
* Auto-scaling at container and infrastructure levels.
* CI/CD pipelines using GitHub/GitLab.
* Monitoring with CloudWatch, Prometheus, APM tools.
* Resilience via retries, circuit breakers, graceful degradation.

---

## 2. Cost Optimization / Pay-per-use

**Q:** How do you handle pay-per-use in the system?

**A:**

* Design for elasticity to pay only for what is used.
* Use auto-scaling to handle peak and low traffic efficiently.
* Serverless components like AWS Lambda for event-driven tasks.
* Optimize compute resources with Kubernetes cluster autoscaling.
* Storage optimization using S3 and RDS instance selection.
* Caching with Redis and CloudFront reduces repeated backend calls.
* Monitor usage with CloudWatch and cost tools.

---

## 3. Caching in Python

**Q:** How do you handle caching in Python?

**A:**

* Application-level caching: in-memory LRU cache for small, repeatable calls.
* Distributed caching with Redis for multi-service environments.
* Cache-aside pattern: check Redis first, fallback to DB if cache miss.
* Set TTLs for cache expiration, use cache invalidation strategies.
* Write-through/write-back caching when consistency is required.
* Frontend caching via CloudFront and HTTP headers.

---

## 4. Data Structures

**Q:** What data structures have you used in Python?

**A:**

* Dictionaries for fast lookups and mapping IDs.
* Lists for ordered collections.
* Sets for uniqueness and membership checks.
* Tuples for immutable data, namedtuples/dataclasses for readability.
* Queues/deques for task processing or producer-consumer patterns.
* Heaps for priority-based scheduling.
* Heavy usage of dicts, lists, and Redis for performance-critical tasks.

---

## 5. Frontend Frameworks

**Q:** Are you comfortable with Vue.js and React?

**A:**

* Primary experience with Vue.js for frontend development.
* Exposed to React modules and concepts (components, hooks, state).
* Worked on backend integration: REST/GraphQL APIs.
* Debugged frontend-backend interactions.
* Comfortable adapting to both Vue.js and React.

---

## 6. Mentoring and Code Reviews

**Q:** Did you ever disagree with senior engineers while mentoring?

**A:**

* Disagreements are addressed professionally.
* Discuss alternative approaches, backed by data or best practices.
* Open to feedback and compromise for project goals.
* Focus on learning and collaborative decision-making.

---

## 7. Production Issues

**Q:** Can you explain a recent production issue and how you handled it?

**A:**

* Issue: Pricing service latency spike at peak hours.
* Cause: Redis cache keys changed; frequent cache misses led to DB overload.
* Immediate fix: Rolled back recent deployment.
* Root cause fix: Corrected cache key logic, added validation/unit tests.
* Long-term: Monitored cache hit/miss ratios, added alerts for DB spikes, improved deployment testing.

---

## 8. Identification Proof

**Q:** Can you show your identification proof?

**A:**

* Cannot share ID over call.
* Provide through secure channels (vendor, onboarding, background verification).
* Prefer secure and authorized sharing methods.

---

## 9. Python Specifics

**Q:** What is GIL in Python?

**A:**

* GIL (Global Interpreter Lock) ensures only one thread executes Python bytecode at a time.
* Prevents race conditions in memory management for CPython.

**Q:** If GIL exists, why use multithreading?

**A:**

* Useful for I/O-bound tasks like API calls, file I/O.
* For CPU-bound tasks, multiprocessing is preferred.

**Q:** Difference between shallow copy and deep copy?

**A:**

* Shallow copy copies object references, not nested objects.
* Deep copy copies the object and all nested objects.
* Use shallow copy for non-nested/immutable data, deep copy for nested structures.

**Q:** How does Python handle memory management?

**A:**

* Automatic memory management using reference counting.
* Garbage collection for cyclic references.
* Memory pools for small objects via `pymalloc`.

---

## 10. Frontend Concepts

**Q:** What is a virtual DOM?

**A:**

* A lightweight in-memory representation of the real DOM.
* Used by Vue.js/React to minimize direct DOM manipulations.
* Updates calculated via diffing algorithm and patched efficiently.

**Q:** React / Vue.js lifecycle for API calls?

**A:**

* Vue: `created()`, `mounted()` for API calls.
* React: `componentDidMount()` (class), `useEffect()` (functional).
* Call APIs after component initialization to avoid blocking render.

---

## 11. Computed Property

**Q:** What is a computing property?

**A:**

* In Vue.js, a computed property is a reactive value derived from other data.
* Automatically recalculates when dependencies change.
* Used for derived state instead of manual updates.

---

## 12. Handling Large Data in Frontend

**Q:** Handling one lakh records in frontend?

**A:**

* Use pagination or virtual scrolling.
* Lazy load data chunks.
* Avoid rendering all rows at once.
* Use efficient state management and caching.

---

## 13. API Integration in React

**Q:** How to integrate APIs in React?

**A:**

* Use `fetch` or `axios` to call API.
* Call API in `useEffect()` for functional components or `componentDidMount()` for class components.
* Update component state with response.
* Handle loading/error states.
* Ensure cleanup for unmounted components.

---

## 14. AI/LLM Integration

**Q:** Can you walk through AI implementation?

**A:**

* Python for ML/LLM model development.
* FastAPI to expose models as REST/GraphQL endpoints.
* Vue.js frontend consumes model APIs.
* CI/CD for automated testing, deployment, and model versioning.
* Monitoring predictions, latency, and performance.
* LLM usage: text generation, QA, embeddings, vector search.

---

## 15. Python + FastAPI + Vue + AI/LLM Stack

**Q:** Are you comfortable with Python, FastAPI, Vue, CI/CD, leveraging AI/LLM?

**A:**

* Python + FastAPI: Serve AI/LLM models via APIs.
* Vue.js: Frontend UI for interacting with AI services.
* CI/CD: Automate tests, deployments, and model updates.
* AI practices: experiment tracking, monitoring, scalable serving.
* LLM: integrate for text generation, summarization, or QA tasks.
