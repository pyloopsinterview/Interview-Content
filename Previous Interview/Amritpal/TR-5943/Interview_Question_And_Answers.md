# Full Interview Questions and Answers (Python/Django + AI)

---

## 1. Tell me about yourself

Hi, my name is Amritpal Singh Malhi.

I’m a Senior Python Technical Architect with around 12 years of experience designing and building scalable web applications using Python, Django, REST APIs, and cloud technologies.

I’ve worked extensively on modernizing legacy systems, building API-driven architectures, and deploying applications on AWS.

One of my key projects was at AmerisourceBergen, where I helped transform a monolithic healthcare system into a modular Django-based platform with strong accessibility compliance and secure architecture.

---

## 2. Django Project Explanation

In my project at Comcare Financial, we worked on a healthcare-focused application.

The system was originally monolithic and difficult to maintain. We redesigned it using Django and Django REST Framework.

We structured the system into multiple Django apps such as user management, claims processing, and reporting. PostgreSQL was used for database design, and cron jobs handled background processing.

---

## 3. NoSQL vs Relational DB

I choose relational databases when data is structured and requires strong consistency.

NoSQL is useful for unstructured or high-scale distributed systems.

In most enterprise applications, I prefer relational databases like PostgreSQL.

---

## 4. Raw SQL vs ORM

I prefer Django ORM, but use raw SQL when:
- Performance optimization is required
- Complex queries are needed
- Using database-specific features

---

## 5. Django Workflow

My workflow includes:
- Understanding requirements
- Designing models
- Building APIs
- Testing locally
- Code review and deployment

---

## 6. Docker Postgres Setup

Steps include:
- Use Alpine base image
- Install PostgreSQL
- Initialize DB
- Configure environment variables
- Expose port
- Set volume
- Create entrypoint script

---

## 7. Performance Issue Debugging

Approach:
- Identify slow areas
- Check logs and monitoring
- Optimize queries
- Add caching
- Scale infrastructure

---

## 8. Machine Learning Experience

I have experience integrating ML into applications using APIs, especially in healthcare.

I’ve worked with AWS services and LLM-based solutions for summarization and document processing.

---

## 9. ML Frameworks

Experience includes:
- TensorFlow
- Scikit-learn
- PyTorch
- Hugging Face
- AWS SageMaker & Bedrock

---

## 10. Hugging Face Clarification

Used for:
- Text summarization
- NLP tasks
- Model integration into APIs

---

## 11. Text Summarization

Worked with healthcare reports and documents to generate concise summaries using NLP models.

---

## 12. Normalization

Normalization organizes data to reduce redundancy.

Includes:
- 1NF: Atomic fields
- 2NF: No partial dependency
- 3NF: No transitive dependency

---

## 13. DB Design Experience

Designed database from scratch:
- Identified entities
- Defined relationships
- Applied normalization
- Added indexing

---

## 14. SQL Query Problem

```sql
SELECT 
    c.customer_id,
    c.first_name,
    c.last_name,
    SUM(p.unit_price * o.quantity) AS total_order_value
FROM customers c
JOIN orders o ON c.customer_id = o.customer_id
JOIN products p ON o.product_id = p.product_id
WHERE o.order_date >= DATE '2024-01-01'
  AND o.order_date < DATE '2025-01-01'
GROUP BY c.customer_id, c.first_name, c.last_name
HAVING SUM(p.unit_price * o.quantity) > 1000;
```

---

## 15. OOP Principles

- Encapsulation
- Inheritance
- Polymorphism
- Abstraction

---

## 16. What is React

React is a JavaScript library for building UI using components and Virtual DOM.

---

## 17. React State Management

- useState (local state)
- Context API (shared state)
- Redux (global state)

---

## 18. Questions for Interviewer

- Team structure
- Current challenges
- Success expectations

---

## 19. Closing Statement

Thank you for the opportunity. I look forward to next steps.

