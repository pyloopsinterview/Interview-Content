# Backend / Java Developer Interview -- Questions & Answers

------------------------------------------------------------------------

## 1. Introduction of your experience and current project

**Question:** Introduction of your experience and current project

**Answer:**\
I am a backend-focused developer with experience in Java, Spring Boot,
and microservices architecture.\
Currently, I am working on distributed systems where I develop REST
APIs, handle database integration, implement validation logic, and
support CI/CD deployments across environments.

------------------------------------------------------------------------

## 2. Is this role primarily backend development?

**Question:** Is this role primarily backend development?

**Answer:**\
Yes, this role primarily focuses on backend development including API
development, business logic implementation, database operations,
performance optimization, and deployment support.

------------------------------------------------------------------------

## 3. Explain your experience with frontend and DevOps

**Question:** Explain your experience with frontend and DevOps

**Answer:**\
**Frontend:** Experience integrating React applications with backend
APIs, handling authentication (JWT), and debugging API responses.\
**DevOps:** Experience with Docker containerization, CI/CD pipelines,
multi-zone deployments, monitoring, and logging.

------------------------------------------------------------------------

## 4. Discuss the most challenging task you have worked on

**Question:** Discuss the most challenging task you have worked on

**Answer:**\
One challenging task was handling distributed transactions in a
microservices environment, optimizing repository calls (avoiding
unnecessary getAll()), and improving validation logic for better
performance and maintainability.

------------------------------------------------------------------------

## 5. Explain the architecture of your application

**Question:** Explain the architecture of your application

**Answer:**\
The application follows a microservices architecture: - API Gateway as
single entry point\
- Separate services with independent databases\
- REST-based communication\
- Load balancing and multi-zone deployment

------------------------------------------------------------------------

## 6. How does frontend communicate with backend services?

**Question:** How does frontend communicate with backend services?

**Answer:**\
Frontend → API Gateway → Backend Service → Database\
Communication is done using REST APIs over HTTPS with JSON payload and
JWT authentication.

------------------------------------------------------------------------

## 7. How do you deploy services across different zones?

**Question:** How do you deploy services across different zones?

**Answer:**\
Using Docker containers, CI/CD pipelines, cloud load balancers, and
deploying service replicas across multiple availability zones.

------------------------------------------------------------------------

## 8. Are you familiar with microservices architectural patterns?

**Question:** Are you familiar with microservices architectural
patterns?

**Answer:**\
Yes. Common patterns include: - API Gateway\
- Service Registry\
- Circuit Breaker\
- Saga Pattern\
- Sidecar Pattern\
- Event-Driven Architecture

------------------------------------------------------------------------

## 9. Explain the API Gateway pattern

**Question:** Explain the API Gateway pattern

**Answer:**\
API Gateway acts as a single entry point for client requests.\
It handles routing, authentication, rate limiting, logging, and load
balancing.

------------------------------------------------------------------------

## 10. How do you register or remove services in an API Gateway?

**Question:** How do you register or remove services in an API Gateway?

**Answer:**\
Using service registry tools like Eureka or Consul. Services
auto-register on startup and deregister on shutdown with health checks.

------------------------------------------------------------------------

## 11. What is a service mesh or mesh network?

**Question:** What is a service mesh or mesh network?

**Answer:**\
Service mesh is an infrastructure layer that manages service-to-service
communication, providing traffic control, security (mTLS), retries, and
observability.

------------------------------------------------------------------------

## 12. What does the sidecar pattern mean?

**Question:** What does the sidecar pattern mean?

**Answer:**\
Sidecar is an architectural pattern where a helper container runs
alongside the main application container to handle logging, monitoring,
security, or networking.

------------------------------------------------------------------------

## 13. Is sidecar a microprocessor system or architectural pattern?

**Question:** Is sidecar a microprocessor system or architectural
pattern?

**Answer:**\
Sidecar is an architectural pattern, not a microprocessor system.

------------------------------------------------------------------------

## 14. Which Java collections do you usually use?

**Question:** Which Java collections do you usually use?

**Answer:**\
ArrayList, LinkedList, HashMap, LinkedHashMap, HashSet, LinkedHashSet,
ConcurrentHashMap.

------------------------------------------------------------------------

## 15. What are LinkedHashMap and LinkedHashSet?

**Question:** What are LinkedHashMap and LinkedHashSet?

**Answer:**\
LinkedHashMap maintains insertion order for key-value pairs.\
LinkedHashSet maintains insertion order and does not allow duplicate
values.

------------------------------------------------------------------------

## 16. What is the difference between LinkedHashMap and LinkedHashSet?

**Question:** What is the difference between LinkedHashMap and
LinkedHashSet?

**Answer:**\
- LinkedHashMap stores key-value pairs\
- LinkedHashSet stores only unique values

------------------------------------------------------------------------

## 17. Explain collisions and rehashing (inflation) in Java collections

**Question:** Explain collisions and rehashing (inflation) in Java
collections

**Answer:**\
Collision occurs when two keys generate the same hash value.\
Rehashing occurs when the load factor exceeds a threshold and the
internal capacity increases.

------------------------------------------------------------------------

## 18. How do you make objects immutable in Java?

**Question:** How do you make objects immutable in Java?

**Answer:**\
- Declare class as final\
- Make fields private final\
- No setters\
- Initialize via constructor\
- Return defensive copies for mutable objects

------------------------------------------------------------------------

## 19. Explain Java collections hierarchy

**Question:** Explain Java collections hierarchy

**Answer:**\
Collection (Interface)\
→ List\
→ Set\
→ Queue\
Map is a separate hierarchy.

------------------------------------------------------------------------

## 20. Where are objects stored in Java memory?

**Question:** Where are objects stored in Java memory?

**Answer:**\
Objects are stored in Heap memory. Local variables are stored in Stack
memory.

------------------------------------------------------------------------

## 21. Explain Java memory areas (heap, stack, metaspace, etc.)

**Question:** Explain Java memory areas

**Answer:**\
- Heap\
- Stack\
- Metaspace\
- Program Counter\
- Native Method Stack

------------------------------------------------------------------------

## 22. Review this pull request -- would you approve it?

**Question:** Review this pull request -- would you approve it?

**Answer:**\
I would check validation logic, exception handling, clean code
practices, performance issues, and test coverage before approving.

------------------------------------------------------------------------

## 23. What problems do you see in this code?

**Question:** What problems do you see in this code?

**Answer:**\
- Unnecessary getAll() calls\
- Missing validation\
- Poor error handling\
- Lack of test coverage

------------------------------------------------------------------------

## 24. How would you fix the validation logic?

**Question:** How would you fix the validation logic?

**Answer:**\
Use annotation-based validation, proper null checks, throw meaningful
exceptions, and add unit tests.

------------------------------------------------------------------------

## 25. What else must be changed besides validation?

**Question:** What else must be changed besides validation?

**Answer:**\
Repository calls should be optimized, unnecessary database fetches
removed, proper error handling added, and code refactored for clean
architecture.

------------------------------------------------------------------------

## 26. What should be passed to the repository instead of getAll()?

**Question:** What should be passed to the repository instead of
getAll()?

**Answer:**\
Instead of getAll(), use: - findById()\
- existsById()\
- findByField()\
Only fetch required data.

------------------------------------------------------------------------

## 27. Explain Reactor validation test prototype

**Question:** Explain Reactor validation test prototype

**Answer:**\
Use StepVerifier to test Mono or Flux responses, validate expected
output, and verify error scenarios.

------------------------------------------------------------------------

## 28. Fix validation in the given code

**Question:** Fix validation in the given code

**Answer:**\
Remove blocking calls, implement proper validation before service logic,
handle errors reactively, and ensure test coverage.

------------------------------------------------------------------------

## 29. Finalize the corrected version of the code

**Question:** Finalize the corrected version of the code

**Answer:**\
The corrected version should: - Avoid unnecessary DB calls\
- Follow SOLID principles\
- Include proper validation\
- Handle exceptions properly\
- Include unit tests
