# Naveen Goud - Interview Q&A Preparation

## 1. Are you completely fine with the JD?

**Answer:**\
Yes, absolutely, I'm completely fine with the job description.

The responsibilities and technical stack mentioned in the JD align very
closely with what I've been doing in my recent projects. I have strong
hands-on experience with Java, especially Spring Boot and microservices
architecture, where I've designed and developed scalable,
high-performance APIs and backend systems.

On the frontend side, I've worked extensively with React, building
responsive and intuitive user interfaces using modern concepts like
functional components, hooks, state management, and API integrations.

I'm also very comfortable with RESTful services, relational databases
like PostgreSQL and Oracle, Git, CI/CD pipelines, Docker, and working in
Agile environments. I regularly participate in code reviews, production
support, and performance optimization.

Overall, the JD matches my experience very well, and I'm confident I can
add value to this role from day one.

------------------------------------------------------------------------

## 2. Are you in EST?

**Answer:**\
Yes, I'm currently based in Philadelphia, Pennsylvania, so I operate in
Eastern Standard Time and am fully comfortable working in EST hours.

------------------------------------------------------------------------

## 3. What is the Roswell Park project about, and what was your contribution as a Lead Developer?

**Answer:**\
At Roswell Park, the project was a real-time healthcare event processing
platform. The goal was to process patient-related events, lab updates,
appointment changes, and clinical research data from multiple internal
systems.

We built Java Spring Boot microservices responsible for ingesting,
validating, sequencing, and publishing events with strict ordering and
fault tolerance. Kafka was used for event-driven communication.

My primary focus was backend architecture and microservices development.
I worked on REST APIs, asynchronous processing, performance tuning,
retry mechanisms, and idempotency strategies.

On the frontend, we used React to build dashboards for monitoring event
flow and system health. I contributed to API integration and UI logic.

As a Lead Developer, I: - Designed microservices architecture\
- Defined API contracts and event schemas\
- Conducted code reviews\
- Guided junior developers\
- Handled production issues\
- Collaborated with DevOps on CI/CD and Docker

------------------------------------------------------------------------

## 4. Where did you use Yarn, Scala, Hive, and Spark?

**Answer:**\
Spark, Scala, Hive, and Yarn were used in the analytics layer, not the
transactional microservices layer.

Our Java microservices published events to Kafka. Spark jobs (written in
Scala) processed large volumes of event data for aggregation,
enrichment, and analytics. Yarn managed cluster resources, and Hive was
used as the data warehouse layer.

My involvement included: - Designing event schemas for Spark
consumption\
- Coordinating data contracts\
- Optimizing Kafka partitioning\
- Supporting Spark job performance tuning

------------------------------------------------------------------------

## 5. This application is built in Java. What is your experience with .NET?

**Answer:**\
Yes, the application was built primarily in Java.

My professional experience is strongly centered around Java and Spring
Boot. I do not have production-level development experience building
large-scale applications in .NET Core or ASP.NET.

However, I understand architectural concepts like MVC, dependency
injection, REST APIs, and microservices. My strongest and most hands-on
expertise is in Java.

------------------------------------------------------------------------

## 6. How is your experience in Python?

**Answer:**\
My Python experience has primarily been for scripting, automation, and
data-related tasks.

At Roswell Park, I used Python for: - Log analysis and monitoring
automation\
- ETL utilities\
- Data validation scripts\
- Deployment health checks

It was not enterprise-level backend development like Django or Flask
applications. My core backend expertise is in Java.

------------------------------------------------------------------------

## 7. Where did you implement Identity and Access Management (IAM)?

**Answer:**\
IAM was implemented at Roswell Park for securing APIs and dashboards.

We used Azure Active Directory for authentication and SSO. OAuth 2.0 and
OpenID Connect were used for token-based authentication. JWT tokens were
validated using Spring Security.

We implemented: - Role-based access control\
- Service-to-service authentication\
- Audit logging for compliance

------------------------------------------------------------------------

## 8. How did you use DynamoDB and Kubernetes?

**Answer:**

**DynamoDB:**\
Used for high-speed key-value storage, including: - Event metadata\
- Idempotency keys\
- Temporary workflow state tracking\
- Configuration data

**Kubernetes:**\
Used for: - Deploying containerized microservices\
- Auto-scaling pods\
- Rolling deployments\
- Self-healing containers\
- Managing secrets and configurations

I designed stateless microservices optimized for Kubernetes deployment.

------------------------------------------------------------------------

## 9. Why are you looking for a change?

**Answer:**\
My current domain is healthcare, and I've gained strong experience in
building scalable event-driven systems.

I'm now looking for: - Broader technical growth\
- More full-stack ownership\
- Exposure to new business domains\
- Opportunities to contribute at an architectural level

This role aligns well with my Java, Spring Boot, React, and cloud-native
experience, and I believe it's a natural next step in my career.
