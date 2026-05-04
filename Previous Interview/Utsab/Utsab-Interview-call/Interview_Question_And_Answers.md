# AI Engineer Interview -- Q&A Notes

## 1. Introduction

**Q: Tell me about yourself**\
Hi, my name is Utsab. I have 13+ years of experience in backend
engineering, primarily using Python and building scalable cloud-based
systems. Recently, I've been focused on AI-driven applications,
especially LLM integrations, RAG pipelines, and agent-based workflows.\
Currently, I'm working on an AI healthcare platform, building a clinical
documentation assistant using FastAPI, LLMs, and vector search.

## 2. Event-Driven Architecture

**Q: Have you used Kafka or SNS?**\
I've worked with event-driven patterns and async processing.\
- Producers, consumers, topics\
- Decoupled architecture\
- Scalability benefits

## 3. Architecture Decisions

**Q: When do you choose event-driven vs others?**\
- Event-driven → decoupling, scalability, async workflows\
- Synchronous APIs → low latency, critical operations\
- Serverless → short-lived, event-triggered

## 4. SAP Integration

-   REST / OData APIs\
-   Secure API layers\
-   Generic integration architecture

## 5. API Integration with SAP

-   REST APIs / OData\
-   OAuth2 / tokens\
-   Bi-directional data flow\
-   Loose coupling

## 6. Data Types from SAP

-   Financial data\
-   HR data\
-   Operational data

## 7. Data Transformation Pipeline

Extraction → Cleaning → Structuring → Enrichment → Prompt → LLM →
Validation

## 8. Canonical Data Model

-   Internal schema\
-   External → internal mapping\
-   Consistency

## 9. Data Storage

-   PostgreSQL\
-   MongoDB\
-   FAISS\
-   Cache

## 10. RAG Architecture

-   Embeddings → Vector DB\
-   Similarity search → Context → LLM\
-   Reduces hallucination

## 11. Pinecone

-   Managed vector DB\
-   Auto scaling\
-   Low latency

## 12. Data Security

-   HTTPS + TLS\
-   OAuth2 / JWT\
-   RBAC\
-   Encryption\
-   PII masking

## 13. LLM Evaluation

-   Structured prompts\
-   Validation\
-   Low temperature\
-   RAG

## 14. ML Lifecycle

Data → Preprocessing → Embeddings → LLM → Evaluation → Deployment →
Monitoring

## 15. Agent Tools

-   Custom tools\
-   APIs\
-   DB queries\
-   ReAct pattern

## 16. Azure Event Systems

-   Event Hubs\
-   Service Bus\
-   Event Grid

## 17. Azure Functions

-   HTTP triggers\
-   Webhooks\
-   Event-driven

## 18. CI/CD

Build → Test → Docker → Deploy

## 19. DevOps Ownership

-   Developers: workflows\
-   DevOps: infra

## 20. Databricks

-   Spark\
-   ETL\
-   Delta Lake

## 21. Unstructured Data

Pipeline: Ingestion → Parsing → Chunking → Embeddings → Vector DB →
Retrieval → LLM

## 22. Leadership

-   Tech Lead\
-   Code reviews\
-   Mentoring

## 23. AI Code Assistants

-   GitHub Copilot\
-   Cursor
