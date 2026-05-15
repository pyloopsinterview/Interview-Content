Amritpal Singh - Interview Questions and Answers
1. Tell me about your recent experience and project.
Sure. In my most recent project at AmerisourceBergen, I was working as a Lead Python Developer and Architect in a cloud-native microservices environment. The application was mainly focused on pharmaceutical order processing, pricing validation, compliance checks, and fulfillment operations.

On the backend side, I was heavily involved in developing scalable REST APIs and microservices using Python. Our primary framework was FastAPI, but across my previous projects, I’ve also worked extensively with Django and Flask for enterprise web applications and API development.

We deployed services on AWS using Lambda, ECS Fargate, and EKS Kubernetes. We also used Kafka for asynchronous event-driven communication between services like pricing, compliance, and inventory systems.

On the frontend side, we used Vue.js dashboards for internal business users. I worked closely with frontend developers on API integration, response structures, authentication flows, and performance optimization.

2. How much work did you do in Django vs FastAPI?
In my recent project at AmerisourceBergen, around 70% of the work was focused on FastAPI and microservices development, while around 30% involved Django-related maintenance and enhancements.

FastAPI was mainly used for: - Async REST APIs - High-throughput services - Kafka event processing - Lightweight microservices

Django was mainly used for: - Legacy service maintenance - Authentication modules - Django ORM operations - Admin functionalities

3. What are Q objects in Django?
Q objects are used in Django ORM for creating complex queries dynamically using logical operators like AND, OR, and NOT.

They are especially useful when: - Building dynamic search filters - Combining multiple optional conditions - Writing nested query logic

Operators: - & for AND - | for OR - ~ for NOT

4. Have you used DRF (Django REST Framework)?
Yes, definitely. I have worked extensively with DRF in multiple projects.

Main usage areas: - REST API development - Serializers - Authentication and authorization - Pagination and filtering - Nested serializers - Swagger/OpenAPI documentation - Permissions and role-based access

5. What are ORM and non-ORM data sources?
ORM data sources are databases managed using Object Relational Mapping tools like Django ORM or SQLAlchemy.

Examples: - PostgreSQL - MySQL - Oracle

Non-ORM data sources include: - Kafka - Redis - Elasticsearch - CSV files - External REST APIs - MongoDB - S3 files

6. What are caching strategies in Django?
Some common caching strategies are: - Per-site caching - Per-view caching - Template fragment caching - Low-level caching - Database query caching

Popular cache backends: - Redis - Memcached - File system cache

7. What are common cache strategy terms?
Important caching strategies include: - Cache Aside - Write Through - Write Behind - Read Through - Refresh Ahead

Most commonly used strategy in projects: - Cache Aside using Redis

8. What is Memcached?
Memcached is a distributed in-memory caching system used to improve application performance by reducing repeated database calls.

Common use cases: - Session caching - API response caching - Frequently accessed data

Difference from Redis: - Memcached is lightweight key-value cache - Redis provides advanced features like persistence, streams, pub/sub, and queues

9. What is file system caching?
File system caching stores cached data as files on the server disk instead of memory.

Advantages: - Easy to configure - No external cache server needed

Limitations: - Slower than Redis or Memcached - Not suitable for high-scale distributed systems

10. Difference between One-to-One field and Foreign Key?
Foreign Key: - Many-to-One relationship - Multiple child records can point to one parent

Example: - Multiple employees belong to one department

One-to-One: - One-to-One relationship - Only one record linked to another record

Example: - One user has one profile

11. What is serialization in Django?
Serialization is the process of converting Django model objects into JSON or other transferable formats.

Deserialization converts incoming JSON data back into Python objects.

Types: - Serializer - ModelSerializer

Used for: - REST APIs - Request validation - Response formatting - Nested object handling

12. What is settings.py in Django?
settings.py is the central configuration file of a Django project.

It contains: - Database settings - Installed apps - Middleware - Static/media configuration - Authentication settings - Security configurations - Logging - Cache settings

In enterprise projects, settings are usually split into: - Development - QA - Production configurations

13. How much frontend experience do you have?
Around 65–70% of my work has been backend-focused, while around 30–35% involved frontend work.

Frontend technologies used: - Vue.js - React - JavaScript - TypeScript - HTML/CSS

Frontend responsibilities: - API integration - Dashboard development - Authentication flows - Form validations - UI enhancements

14. What AWS services have you used?
Serverless services: - AWS Lambda - API Gateway - EventBridge - Step Functions - SNS/SQS

Other AWS services: - ECS Fargate - EKS Kubernetes - EC2 - S3 - RDS PostgreSQL - DynamoDB - CloudWatch - IAM - AWS X-Ray - Route 53 - CloudFormation

15. Are you comfortable with coding assessments and whiteboard rounds?
Yes, absolutely. I’m comfortable with coding assessments, debugging exercises, API design discussions, and whiteboard-style technical interviews.

I’m comfortable working on: - Python coding challenges - Backend logic implementation - REST APIs - Database scenarios - Debugging incomplete solutions - System design discussions