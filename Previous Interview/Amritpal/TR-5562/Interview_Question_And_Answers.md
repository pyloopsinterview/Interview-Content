# Azure Developer Interview – Question & Answer Log

---

## 1. Azure Confidence & Platform Preference

### Q1: How confident are you with Azure compared to other cloud platforms?

**Answer:**
I am highly confident with Microsoft Azure. While I have exposure to multi-cloud environments, my strongest hands-on experience is with Azure, especially in building and deploying Python APIs using Azure App Services, integrating Azure SQL Database, Azure AI Search, and Azure OpenAI, and managing CI/CD with Azure DevOps and Terraform.

---

### Q2: Are you strong across all Azure services mentioned, or any particular service you are most confident in?

**Answer:**
I am strongest in Azure App Services, Azure SQL Database, Azure AI Search, and Azure OpenAI integrations. My core expertise lies in Python API development, RAG workflows, vector search optimization, and full cloud-native application deployment on Azure.

---

## 2. Azure App Service & Infrastructure

### Q3: What is Azure App Service?

**Answer:**
Azure App Service is a fully managed Platform-as-a-Service (PaaS) offering that allows developers to deploy web applications and APIs without managing infrastructure. It handles scaling, patching, load balancing, and security automatically.

---

### Q4: What is the difference between Azure App Service and Azure Virtual Machine?

**Answer:**
Azure App Service is PaaS, where Azure manages infrastructure and runtime. Azure Virtual Machine is IaaS, where you manage the OS, runtime, patching, and scaling manually. App Service is ideal for APIs and web apps, while VMs are suitable for full OS-level control.

---

### Q5: What are Deployment Slots in Azure App Service?

**Answer:**
Deployment Slots are separate live environments (like staging and production) within the same App Service instance. They allow zero-downtime deployments through slot swapping and support quick rollback if needed.

---

### Q6: How do you scale applications in Azure App Service?

**Answer:**
Scaling is done in two ways:
- Vertical Scaling (Scale Up) by upgrading the App Service Plan.
- Horizontal Scaling (Scale Out) by increasing instances.
Auto-scaling rules can be configured based on CPU, memory, or request load.

---

### Q7: How do you secure applications in Azure App Service?

**Answer:**
Security is implemented using Azure AD authentication, Managed Identity for secure service communication, HTTPS enforcement, Private Endpoints, IP restrictions, Azure Key Vault for secrets, and Application Insights for monitoring.

---

## 3. Python Development Experience

### Q8: How many years of hands-on Python experience do you have?

**Answer:**
I have approximately 8–9 years of hands-on Python development experience building REST APIs, backend systems, and AI-driven platforms.

---

### Q9: Which Python frameworks and APIs have you used?

**Answer:**
Primarily FastAPI and Django (with Django REST Framework). I am more experienced with FastAPI for high-performance async APIs. I have also used SQLAlchemy, Pydantic, Celery, PyJWT, Azure SDKs, and LangChain.

---

## 4. Generative AI & RAG Systems

### Q10: How would you design a RAG pipeline in Azure?

**Answer:**
I would design it in three layers:
1. Ingestion Layer – Blob Storage + Azure Function + Chunking + Embeddings via Azure OpenAI + Indexing in Azure AI Search.
2. Retrieval Layer – Query embedding + Hybrid Search (vector + keyword).
3. Generation Layer – Grounded prompt construction + Azure OpenAI response with citations.
Security via Managed Identity and CI/CD via Azure DevOps.

---

### Q11: What challenges have you faced while working on RAG systems?

**Answer:**
Major challenges included hallucination, poor chunking strategy, latency, cost optimization, and security concerns. These were solved by improving chunk overlap logic, implementing hybrid search, optimizing top-k retrieval, caching embeddings, and enforcing citation-based prompt engineering.

---

### Q12: How do you optimize Azure AI Search for vector search?

**Answer:**
Optimization includes:
- Proper index schema design using HNSW.
- Correct embedding dimension configuration.
- Semantic chunking with overlap.
- Hybrid search configuration.
- Metadata filtering.
- Limiting top-k results.
- Scaling replicas and partitions for performance.

---

## 5. Team & Role Understanding

### Q13: Do you have any questions for us?

**Answer:**
Yes. I would like to understand the current architecture, the maturity of the RAG system, CI/CD setup, collaboration structure, and what success looks like in the first 3–6 months.

---

### Q14: What is the expected team size and collaboration model?

**Answer:**
Understanding team size helps clarify collaboration between backend (Python), frontend (React/Node.js), AI engineers, and DevOps teams, and how responsibilities are distributed.

---

## 6. Role Expectations

### Q15: What are the main skill sets required for this Azure Developer role?

**Answer:**
Strong Python API development, Azure App Services, Azure SQL Database, Azure AI Search, Azure OpenAI, RAG architecture, CI/CD with Azure DevOps, Infrastructure as Code using Terraform, and understanding of GenAI concepts.

---