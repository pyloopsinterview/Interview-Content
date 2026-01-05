# Interview Questions with Correct Answers

---

## 1. Do you also work on Angular?
**Answer:**  
Yes, I have worked on Angular earlier in my career. Although my recent projects are more React-focused, I do have hands-on experience with Angular and its core concepts.

---

## 2. So you have also worked on Angular?
**Answer:**  
Yes, I have worked on Angular, mainly in my earlier projects. I’m comfortable with its architecture and fundamentals.

---

## 3. At least, are you aware of the key concepts of Angular?
**Answer:**  
Yes, I’m aware of the key Angular concepts and how Angular applications are structured and built.

---

## 4. What are the concepts of Angular?
**Answer:**  
Angular is component-based. Key concepts include components, modules (NgModules), data binding, directives, services with dependency injection, routing, RxJS and observables, and template-driven and reactive forms.

---

## 5. Have you used cloning?
**Answer:**  
Yes, I’ve used cloning, mainly to avoid mutating objects directly and to ensure proper change detection.

---

## 6. Cloning in the…?
**Answer:**  
In Angular and React, cloning is used to create new object or array references instead of mutating existing ones, which helps frameworks detect changes and update the UI correctly.

---

## 7. In Angular as well as React, components need to communicate with each other. What are the multiple ways?
**Answer:**  
Parent-to-child using inputs/props, child-to-parent using events or callbacks, shared services or state management, router-based data passing, and in some cases direct references like ViewChild.

---

## 8. One screen with multiple tiles sharing data—how will you communicate between them?
**Answer:**  
The best approach is a shared service acting as a single source of truth. All tiles subscribe to shared observable state, and updates from one tile are propagated automatically to others.

---

## 9. What do you understand by lazy loading?
**Answer:**  
Lazy loading means loading modules, components, or data only when they are required, reducing initial load time and improving performance in large applications.

---

## 10. Have you heard about the PubSub mechanism?
**Answer:**  
Yes, I’ve worked with PubSub-style messaging in event-driven architectures.

---

## 11. What is the PubSub mechanism?
**Answer:**  
PubSub is an asynchronous messaging pattern where publishers send messages to topics and subscribers consume them independently, enabling loose coupling and scalability.

---

## 12. Which Java features have you used, and which version are you working on?
**Answer:**  
I primarily work with Java 8+. I use lambdas, streams, Optional, CompletableFuture, ExecutorService, and the modern Date/Time API regularly.

---

## 13. Have you worked on GCP?
**Answer:**  
Yes, I’ve worked on GCP in production, mainly with BigQuery, cloud storage, Kubernetes-based deployments, and integrations with backend services.

---

## 14. What is the difference between Cloud Spanner and BigQuery?
**Answer:**  
Cloud Spanner is a transactional, strongly consistent database for application read/write workloads. BigQuery is an analytical data warehouse optimized for large-scale read-heavy analytics.

---

## 15. If an application needs read and write operations, which will you use—Spanner or BigQuery?
**Answer:**  
Cloud Spanner, because it is designed for transactional read/write workloads with low latency and strong consistency.

---

## 16. Have you ever used Vertex AI in GCP?
**Answer:**  
Yes, I’ve worked with Vertex AI at an integration level, consuming prediction endpoints from backend services and managing data flow around ML models.

---

## 17. In Angular and React, have you written unit test cases?
**Answer:**  
Yes. In React, I use Jest and React Testing Library. In Angular, I use Jasmine and Karma to test components, services, and HTTP interactions.

---

## 18. What is the use of flush and tick in Angular testing?
**Answer:**  
Both are used in fakeAsync tests. `tick()` simulates the passage of a specific amount of time, while `flush()` executes all pending asynchronous tasks at once.

---

## 19. How do you write test cases for mocking APIs?
**Answer:**  
In Angular, I use HttpClientTestingModule and HttpTestingController to intercept and mock HTTP calls. In React, I use Jest mocks or tools like MSW to mock API responses.

---

## 20. How do you test a service that depends on another downstream service?
**Answer:**  
I mock the downstream service using spies or mock implementations, control the returned data, and test only the logic of the main service in isolation.

---

## 21. Brief description of the current project tech stack?
**Answer:**  
Backend with Java Spring Boot and Node.js microservices, frontend with React, cloud on GCP and AWS, data processing using BigQuery and Spark, containerization with Docker and Kubernetes, and CI/CD using Jenkins.

---

## 22. In Spring Boot, how do you handle multiple beans with similar names?
**Answer:**  
By using `@Qualifier` to explicitly select a bean, `@Primary` for default selection, or `@Profile` to activate beans conditionally. Bean overriding is generally avoided.

---

## 23. What happens if you disable second-level cache in Hibernate?
**Answer:**  
Hibernate will no longer cache entities across sessions. Only first-level (session) cache remains, increasing database calls and potentially reducing performance.

---

## 24. Write Java code to find the second most frequent number using streams.
**Answer:**  

```java
Integer result = numbers.stream()
    .collect(Collectors.groupingBy(Function.identity(), Collectors.counting()))
    .entrySet().stream()
    .sorted(Map.Entry.<Integer, Long>comparingByValue().reversed())
    .skip(1)
    .map(Map.Entry::getKey)
    .findFirst()
    .orElse(null);
