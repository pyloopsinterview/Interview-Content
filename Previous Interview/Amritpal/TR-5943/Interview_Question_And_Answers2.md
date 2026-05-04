# Interview Questions & Answers (Markdown)

## 1. Introduction

Hi, my name is Amritpal Singh.

I’m a **Senior Python Technical Architect** with around **12 years of experience** building scalable web applications using **Python, Django, and REST APIs**. I have worked on **modernizing legacy systems**, **designing databases**, and **integrating AI/ML solutions** into production systems.

---

## 2. Django Experience

I have strong experience with **Django ORM, views, serializers, and REST APIs**. I’ve built scalable backend systems and optimized queries using **select_related** and **prefetch_related**.

---

## 3. REST API Design

I design APIs using:

* Proper **HTTP methods**
* **Versioning**
* **Validation**
* **Authentication & RBAC**

---

## 4. Legacy Migration

I have migrated **legacy monolithic systems** into **modular Django services** using a **phased approach** and **reverse engineering**.

---

## 5. Database Choice (SQL vs NoSQL)

* Prefer **PostgreSQL (Relational DB)** for **structured data** and **ACID compliance**
* Use **NoSQL** for **unstructured data** and **high scalability use cases**

---

## 6. Raw SQL vs ORM

* Use **ORM by default**
* Use **RAW SQL** for:

  * Performance optimization
  * Complex queries
  * Database-specific features

---

## 7. Development Workflow

1. Requirement Analysis
2. Design
3. Development
4. Testing
5. Code Review
6. Deployment (CI/CD)

---

## 8. Performance Optimization

* Identify **bottlenecks**
* Optimize **queries & indexing**
* Use **caching (Redis)**
* Move heavy tasks to **background jobs**

---

## 9. Machine Learning Experience

* Integrated **ML models** using Django APIs
* Worked with **AWS SageMaker**
* Used **Hugging Face** for NLP tasks

---

## 10. Hugging Face Usage

Used for:

* **Text Classification**
* **Summarization**
* **Named Entity Recognition (NER)**

---

## 11. SQL Query Example

```sql
SELECT 
    c.customer_id,
    c.first_name,
    c.last_name,
    SUM(p.unit_price) AS total_order_value
FROM customers c
JOIN orders o ON c.customer_id = o.customer_id
JOIN products p ON o.product_id = p.product_id
WHERE EXTRACT(YEAR FROM o.order_date) = EXTRACT(YEAR FROM CURRENT_DATE) - 1
GROUP BY c.customer_id, c.first_name, c.last_name
HAVING SUM(p.unit_price) > 1000;
```

---

## 12. OOP Principles

* **Encapsulation**
* **Inheritance**
* **Polymorphism**
* **Abstraction**

---

## 13. React Basics

React is a **JavaScript library** for building **UI** using:

* Components
* Virtual DOM
* Hooks

---

## 14. React State Management

* **Local State** → useState
* **Global State** → Context API / Redux
* **One-way data flow**

---

## 15. Questions to Ask Interviewer

* Current **architecture** (monolith vs microservices)
* **AWS cloud adoption**
* **AI/ML integration strategy**
* Team challenges & expectations

---

## 16. Closing Statement

I’m very interested in this opportunity as it aligns with my experience in **Django**, **scalable systems**, and **AI integration**.
