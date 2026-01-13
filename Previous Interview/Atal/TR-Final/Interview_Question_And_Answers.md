```md
# Hiring Manager Round – Exact Interview Questions with Correct Answers

This document contains the **exact questions** asked during the **Hiring Manager / Architecture discussion round**, along with **clear, correct, and interview-ready answers** aligned to senior/lead expectations.

---

## 1. Can you give a brief introduction about yourself?
**Answer:**  
I have over 15 years of experience as a Senior/Lead Full-Stack Developer, primarily working on enterprise-scale applications in the healthcare domain. My core expertise includes Java, Spring Boot, React, Angular, cloud-native architectures on GCP and AWS, event-driven systems, and building highly scalable and reliable platforms.

---

## 2. What exactly is your role in your current project?
**Answer:**  
I work as a Senior Full-Stack Developer with end-to-end ownership. I design and develop backend microservices, contribute to frontend architecture, participate in system design discussions, mentor team members, and support production systems with a strong ownership mindset.

---

## 3. Why are you looking for a change from your current organization?
**Answer:**  
I’m looking for an opportunity where I can contribute more to platform-level design, reusable frameworks, and innovation initiatives. I want to work on problems that involve modern architectures and have broader technical impact.

---

## 4. How comfortable are you with Angular, given your recent React focus?
**Answer:**  
I’m comfortable with Angular. While my recent work is more React-focused, I’ve worked extensively with Angular in enterprise projects and understand its core concepts, architecture, and best practices well.

---

## 5. What are the core concepts of Angular?
**Answer:**  
Angular is component-based. Key concepts include components, modules, services with dependency injection, routing, RxJS and observables, directives, content projection, forms (template-driven and reactive), and lifecycle hooks.

---

## 6. What is Angular content projection?
**Answer:**  
Content projection allows a component to receive external content and render it within predefined placeholders using `ng-content`. It’s commonly used for building reusable UI components like cards and layouts.

---

## 7. How do you project header and footer content into the same component?
**Answer:**  
By using multiple `ng-content` elements with selectors. Each selector acts like a named slot, allowing header, body, and footer content to be projected into specific locations.

---

## 8. How do you implement `[(ngModel)]` on a custom Angular component?
**Answer:**  
By implementing `ControlValueAccessor` and registering the component with `NG_VALUE_ACCESSOR`. This allows Angular forms to read and write values to the custom component.

---

## 9. What are the mandatory methods of ControlValueAccessor?
**Answer:**  
The mandatory methods are `writeValue()`, `registerOnChange()`, and `registerOnTouched()`. `setDisabledState()` is optional.

---

## 10. What is your experience with Angular Router Guards?
**Answer:**  
I’ve used router guards such as `CanActivate`, `CanActivateChild`, `CanDeactivate`, `Resolve`, and `CanLoad` to implement authentication, authorization, lazy-loading protection, and unsaved-form handling.

---

## 11. What is your experience with Jasmine unit testing?
**Answer:**  
I’ve written extensive Jasmine unit tests for components, services, guards, and async workflows. I focus on isolated tests, mocking dependencies, and ensuring good coverage for business-critical logic.

---

## 12. How do you mock slow or asynchronous API calls in Jasmine?
**Answer:**  
I mock API calls using spies and return observables with delays. I use `fakeAsync` with `tick()` or `flush()` to simulate time without waiting for real delays.

---

## 13. What is the difference between `tick()` and `flush()`?
**Answer:**  
`tick()` simulates the passage of a specific amount of time, while `flush()` completes all pending asynchronous tasks regardless of time.

---

## 14. Which GCP services have you used?
**Answer:**  
I’ve used BigQuery, Cloud Storage, GKE, Pub/Sub, Cloud Logging, and Monitoring in production environments.

---

## 15. What OLTP experience do you have?
**Answer:**  
I’ve worked on application-driven transactional systems using relational databases, focusing on data consistency, performance, and transactional integrity.

---

## 16. What is the difference between Cloud Spanner and BigQuery?
**Answer:**  
Cloud Spanner is a transactional database for real-time read/write workloads, while BigQuery is an analytical data warehouse optimized for large-scale reporting and analytics.

---

## 17. Why did you use Kafka instead of GCP Pub/Sub?
**Answer:**  
Kafka was already an enterprise-standard messaging backbone with strong replay, ordering, and schema governance. Using Kafka ensured consistency across hybrid environments and reduced operational risk.

---

## 18. How did your cloud application integrate with on-prem Kafka?
**Answer:**  
The integration was done using secure network connectivity such as VPN or interconnect. Kafka was treated as an external service, allowing cloud and on-prem systems to communicate reliably.

---

## 19. How would you architect a system to ingest data from hundreds of healthcare devices?
**Answer:**  
I’d use a durable messaging layer like Kafka or Pub/Sub to decouple ingestion from processing, followed by stream processors for validation and enrichment, and purpose-built storage for transactional and analytical workloads.

---

## 20. How do you handle concurrency in Java microservices?
**Answer:**  
I use bounded thread pools for thread management, immutable data models, stateless processing, and partitioned workloads. This avoids race conditions without relying on locks.

---

## 21. How do you handle different threads in your code?
**Answer:**  
Threads are managed using `ExecutorService`. Tasks are submitted asynchronously, and the executor controls concurrency and resource usage.

---

## 22. How do you ensure consistency while processing events in parallel?
**Answer:**  
By partitioning events by a stable key like patient ID, ensuring ordering per partition, and making database writes idempotent.

---

## 23. How will you scale this system?
**Answer:**  
By decoupling ingestion using a stream, scaling consumers horizontally, partitioning data for parallelism, batching database writes, and auto-scaling based on load and lag.

---

## 24. Can you explain concurrency and threshold handling in your code?
**Answer:**  
Concurrency is handled through asynchronous task execution using a thread pool, while threshold handling is stateless and based on immutable event data, ensuring thread safety.

---

## 25. How do you see yourself contributing to this team?
**Answer:**  
I can contribute by designing scalable systems, building reusable frameworks, mentoring team members, and driving architectural improvements aligned with business goals.

---

## Final Summary
This interview evaluated:
- Architectural thinking and ownership  
- Angular framework depth  
- Testing discipline  
- Cloud and messaging decisions  
- Concurrency, scalability, and system design  

Your answers demonstrated **senior/lead-level maturity** and practical experience.
```
