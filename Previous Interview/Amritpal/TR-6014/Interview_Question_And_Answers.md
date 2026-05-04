# 📝 Interview Questions & Answers (Unique Only)

---

## Q1. What are your views on Agentic AI?
**Answer:**  
Agentic AI represents a shift from traditional prompt-response systems to **goal-driven, action-oriented systems**. Instead of just generating answers, these systems can **plan, reason, and execute workflows** using tools and APIs. In my experience, I’ve worked on a similar system for **incident diagnostics**, where the AI agent analyzes logs, alerts, and tickets, and provides **root cause analysis and remediation suggestions**. I see strong value in enterprise environments like **SAP managed services**, but it requires **governance, observability, and control** to be production-ready.

---

## Q2. How was planning handled in your agentic system? Was it deterministic or dynamic? What business problem did it solve and what technologies were used?
**Answer:**  
We used a **hybrid approach** — the overall workflow was **deterministic**, but decision-making within each step was **dynamic using LLMs**. The system followed a pipeline: **incident ingestion → context retrieval → analysis → response generation**. The business problem was **manual incident triage**, which was time-consuming. The system reduced **MTTR and manual effort**. Technologies included **Python, LangGraph-style orchestration, LLMs, vector databases, ServiceNow APIs, and AWS**.

---

## Q3. How did you handle interaction and orchestration across multiple agents?
**Answer:**  
We used a **centralized orchestration model**, where agents were implemented as **modular nodes** rather than independent services. Each node had **specific responsibilities and scoped tool access**. Instead of letting a single LLM decide everything, we followed a **controlled execution flow**, ensuring **predictability, observability, and reliability** in enterprise environments.

---

## Q4. Why didn’t you use a single orchestrator LLM to dynamically select agents?
**Answer:**  
While dynamic routing provides flexibility, it introduces **non-determinism and unpredictability**, which is risky in production systems. Instead, we used a **predefined workflow** with **LLM-driven reasoning within each step**. This ensured **control, traceability, and consistency**, while still allowing flexibility where needed.

---

## Q5. How do you ensure explainability and flexibility in your system?
**Answer:**  
Explainability comes from **structured workflows and traceability**, where each step logs inputs, outputs, and decisions. Flexibility is achieved through **LLM reasoning within each stage**. This provides **controlled flexibility**, allowing the system to adapt without losing transparency.

---

## Q6. How would you ensure data segregation in a multi-tenant, multi-agent platform?
**Answer:**  
I would enforce **tenant isolation at all layers** — data, application, and infrastructure. This includes **tenant-aware data tagging, vector DB namespace isolation, RBAC/IAM controls, scoped context handling, and audit logging**. This ensures **no cross-tenant data leakage** while maintaining scalability.

---

## Q7. How do you choose the right model strategy? Single model vs multi-model vs judge pattern?
**Answer:**  
I start with a **strong baseline model**, then implement **evaluation and feedback loops**. Multi-model approaches are used **selectively**, such as:  
- **Task-specific models** (small for retrieval, large for reasoning)  
- **Judge models** for validation in critical cases  

The goal is to balance **accuracy, cost, and latency** while continuously improving.

---

## Q8. What are the key architectural considerations when building a multi-agent system?
**Answer:**  
Key considerations include:  
- **Problem decomposition** (clear agent roles)  
- **Orchestration strategy** (centralized vs decentralized)  
- **Context and communication design**  
- **Scoped tool access**  
- **State and memory management**  
- **Observability and debugging**  
- **Failure handling**  
- **Security and governance**  

The focus is on building a **modular, controlled, and scalable system**.

---

## Q9. What questions would you ask the interviewer about their AI systems and expectations?
**Answer:**  
I would ask about:  
- Their approach to **AI agent architecture (controlled vs autonomous)**  
- The maturity of **AI adoption in SAP managed services**  
- How AI integrates with **SAP systems (OData, CDS, workflows)**  
- The **priorities for the role** (architecture vs rapid delivery)

---