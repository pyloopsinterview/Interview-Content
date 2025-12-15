# ````md

# \# Complete List of Interview Questions Asked by Me — With Correct Answers

# 

# ---

# 

# \## 1. How is your day-to-day activity when working with Kubernetes?

# 

# \*\*Answer:\*\*  

# My day-to-day work involves monitoring service health using logs, metrics, and alerts, followed by hands-on development of Java microservices. I containerize applications using Docker, deploy them to Kubernetes using manifests or Helm, configure autoscaling, resource limits, and health probes, and manage deployments through CI/CD pipelines. I also troubleshoot production issues, perform rollbacks, and collaborate with DevOps teams on security, networking, and observability.

# 

# ---

# 

# \## 2. Is your role more DevOps-oriented, like 60% coding and 40% DevOps?

# 

# \*\*Answer:\*\*  

# Yes, that’s accurate. About 60% of my time is focused on core Java development—API design, business logic, and performance optimization. The remaining 40% is spent on DevOps tasks such as Dockerization, Kubernetes deployments, CI/CD pipelines, autoscaling, observability, and production support. I own the service end to end.

# 

# ---

# 

# \## 3. I have a list of strings like “December is this month” and “Today is Monday”. How do you extract all the words?

# 

# \*\*Answer:\*\*  

# In Java, I iterate over the list of sentences, split each sentence using whitespace, and flatten the results into a single list. Using streams, `flatMap` is used to convert multiple word arrays into a single stream of words.

# 

# \### Code:

# ```java

# List<String> sentences = Arrays.asList(

# &nbsp;   "December is this month",

# &nbsp;   "Today is Monday"

# );

# 

# List<String> words = sentences.stream()

# &nbsp;   .flatMap(sentence -> Arrays.stream(sentence.split("\\\\s+")))

# &nbsp;   .collect(Collectors.toList());

# ````

# 

# ---

# 

# \## 4. What is the difference between `map` and `flatMap`?

# 

# \*\*Answer:\*\*

# `map` performs a one-to-one transformation and returns a stream of collections, such as `Stream<String\[]>`.

# `flatMap` performs a one-to-many transformation and flattens the result into a single stream, such as `Stream<String>`.

# For extracting words from multiple sentences, `flatMap` is the correct choice.

# 

# ---

# 

# \## 5. What is the difference between fail-fast and fail-safe aggregators?

# 

# \*\*Answer:\*\*

# Fail-fast aggregators throw a `ConcurrentModificationException` if the collection is modified during iteration, helping detect bugs early. Fail-safe aggregators work on a snapshot of the collection, allow concurrent modifications, and do not throw exceptions, but they use extra memory and may not reflect real-time changes.

# 

# ---

# 

# \## 6. What is CI and what is CD?

# 

# \*\*Answer:\*\*

# CI (Continuous Integration) automatically builds and tests code whenever changes are committed to the repository.

# CD (Continuous Delivery or Continuous Deployment) automates the process of delivering validated builds to environments. Delivery requires manual approval for production, while deployment pushes changes automatically. Together, CI/CD ensures fast and reliable releases.

# 

# ---

# 

# \## 7. Can you tell me some common annotations used in Spring Boot?

# 

# \*\*Answer:\*\*

# Common annotations include `@SpringBootApplication`, `@RestController`, `@GetMapping`, `@PostMapping`, `@Service`, `@Repository`, `@Component`, `@Autowired`, `@Configuration`, `@Bean`, `@Entity`, `@Valid`, `@ControllerAdvice`, and `@ExceptionHandler`. These cover application startup, REST APIs, dependency injection, persistence, validation, and exception handling.

# 

# ---

# 

# \## 8. What is a component scan?

# 

# \*\*Answer:\*\*

# Component scan is the mechanism by which Spring automatically discovers classes annotated with `@Component`, `@Service`, `@Repository`, and `@Controller` and registers them as beans in the application context. In Spring Boot, it is enabled by default through `@SpringBootApplication`.

# 

# ---

# 

# \## 9. How do you resolve duplicate beans issues in Spring?

# 

# \*\*Answer:\*\*

# I identify the cause, such as overlapping component scans or duplicate bean definitions. I fix it by narrowing scan scopes, removing redundant `@Bean` definitions, or using `@Primary`, `@Qualifier`, or `@Profile` to explicitly control which bean should be injected.

# 

# ---

# 

# \## 10. Can you explain what you do in low-latency distributed systems?

# 

# \*\*Answer:\*\*

# I design and build Java services that process events in memory with minimal latency. I use asynchronous, non-blocking architectures, optimize JVM and garbage collection settings, reduce object allocations, and tune threading models. I also configure infrastructure for predictable performance and continuously monitor p99 and p99.9 latencies.

# 

# ---

# 

# \## 11. In your application, instead of market data, you handle clinical data. How does that work?

# 

# \*\*Answer:\*\*

# Clinical events act like market data streams. We ingest patient-related events in near real time, process them efficiently in memory, maintain correct ordering per patient, and distribute them to downstream systems. The architecture prioritizes low latency, consistency, and regulatory compliance.

# 

# ---

# 

# \## 12. What are the components in between, and what frameworks did you use?

# 

# \*\*Answer:\*\*

# Upstream systems publish events to SNS/SQS or Kinesis. Spring Boot–based ingestion services consume and validate data. Core processing services apply business rules and transformations. DynamoDB is used for persistence. Processed events are redistributed to downstream systems. Everything runs in Docker containers on Kubernetes (EKS), deployed via GitLab CI/CD, with observability using OpenTelemetry.

# 

# ---

# 

# \## 13. If something goes wrong during processing or the data is not compliant, how do you handle it?

# 

# \*\*Answer:\*\*

# Invalid data is rejected early and routed to a Dead Letter Queue. Transient failures are retried with backoff. Permanent failures are quarantined for analysis. The system is idempotent, supports replay, and is monitored using alerts on error rates and DLQ depth.

# 

# ---

# 

# \## 14. Can you name six protocols?

# 

# \*\*Answer:\*\*

# HTTP/HTTPS, gRPC, TCP, FIX protocol, AMQP, and streaming protocols such as Kafka or Kinesis.

# 

# ---

# 

# \## 15. How does the message look when you send it to external parties using FIX?

# 

# \*\*Answer:\*\*

# A FIX message is a tag-value–based message consisting of a header, body, and trailer, sent over a persistent TCP connection. It includes fields such as message type, sender and receiver IDs, sequence numbers, timestamps, order details, and a checksum for integrity.

# 

# ---

# 

# \## 16. What if you use a JSON-based protocol instead of FIX?

# 

# \*\*Answer:\*\*

# We send JSON-based messages that preserve FIX semantics, including message type, sender and receiver identifiers, sequence numbers, timestamps, and order details. This simplifies integration while maintaining reliability, ordering, and low-latency characteristics.

# 

# ---

# 

# \## 17. What are the expectations from this role if I get selected?

# 

# \*\*Answer:\*\*

# The expectation is to be a hands-on Java engineer who owns services end to end—design, development, deployment, and production support. Strong understanding of distributed systems, low-latency design, CI/CD, and collaboration is required, along with a continuous learning mindset and accountability for production systems.

# 

# ---

# 

# ```

# ```



