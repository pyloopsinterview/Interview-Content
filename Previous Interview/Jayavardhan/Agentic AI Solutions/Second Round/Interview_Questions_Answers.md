## Interview Question And Answers

# **Jay – Agentic AI Technical Lead Interview Q&A**

---

## **1️⃣ Transition to AI & Learning Path**

**Q:** You started with UI originally, right? What resources did you use to get yourself educated and transition into AI? Are you familiar with traditional AI — models, training, inference, etc.?

**A:**
You’re absolutely right — I started my career as a UI specialist, primarily focusing on front-end engineering and user experience. Over time, as enterprise systems became more data-driven and intelligent, I naturally transitioned toward backend integrations and distributed systems.

My entry into AI wasn’t an overnight shift; it evolved through **data orchestration, API-driven architectures, and automation frameworks**. Around 2021, I began exploring **applied AI** — working with **Python**, **AWS SageMaker**, and later **Bedrock**.

I studied traditional AI workflows — **training, inference, embeddings, and reinforcement** — and learned through:

- AWS documentation (Bedrock, SageMaker)
- LangChain / LangGraph / CrewAI repos
- NIST AI RMF for Responsible AI governance
- Internal PoCs at McKesson building **multi-agent orchestration** frameworks

So my transition was **systems-led**, leveraging my distributed architecture experience to enable **AI-driven orchestration** in healthcare.

---

## **2️⃣ LangChain Experience**

**Q:** How long have you been working with LangChain? Are you still using it?

**A:**
I started exploring **LangChain** around late **2023** as part of early experiments in **LLM orchestration**.

While we don’t use LangChain directly in production at McKesson, its **concepts** inspired our own orchestration framework — especially **context management, tool abstraction, and agent handoffs**.

We adapted those ideas into a more **enterprise-grade MCP (Model Context Protocol)** framework integrated with **AWS Bedrock**, giving us more control, observability, and compliance.

---

## **3️⃣ Backend vs Agentic AI Leadership**

**Q:** Would you be a better technical lead for backend systems or for agentic AI orchestration?

**A:**
My strength lies in **agentic AI orchestration** — designing frameworks that allow agents to collaborate, reason, and operate securely.

However, that strength is built on a deep background in **backend systems** — event-driven design, APIs, authentication, and observability.

For example, at McKesson I designed the **multi-agent coordination layer**, handling task planning, tool registries, and Bedrock integrations through our internal API Gateway.
So, I’m focused on **agent system design**, but with strong backend depth to make those systems scalable and production-ready.

---

## **4️⃣ Human-in-the-Loop Interaction Design**

**Q:** Have you designed user interaction systems where a human is part of the loop?

**A:**
Yes — I’ve designed several **human-in-the-loop (HITL)** systems where agents collaborate with human operators.

One example is our **AI-driven claims automation** platform: agents processed claims autonomously but escalated ambiguous cases to humans through a dynamic UI.

I designed the **interaction model** — defining pause points, context persistence, and human validation flows.
So while I’m not hands-on with UI code today, I bridge **front-end interaction design** with **AI orchestration** to ensure usability, auditability, and compliance.

---

## **5️⃣ Workflow / Event Framework (EWF)**

**Q:** What type of workflow framework (EWF) do you use for building these applications?

**A:**
We use a **custom event-driven workflow framework (EWF)** built on **AWS Step Functions** and **EventBridge**.

It coordinates agent actions, Bedrock invocations, and HITL steps in an event-driven manner.
Each task or escalation is modeled as a **state transition** with trace IDs and persisted via **DynamoDB**.

We chose this design for its **observability**, **idempotency**, and **security**, with native CloudWatch monitoring and HIPAA-aligned access control.

---

## **6️⃣ AWS Bedrock Usage**

**Q:** What do you use AWS Bedrock for? What specific things do you get from it?

**A:**
We use **AWS Bedrock** as the **managed AI runtime layer** for our orchestration platform.

Specifically, it provides:

1. **Access to foundation models** (Claude, Titan, Llama 3) through a unified API
2. **Prompt management & Bedrock Agents** for reusable skills
3. **IAM/KMS integration** for HIPAA-compliant security
4. **Observability** via CloudWatch and Bedrock trace logs

So, Bedrock acts as our **secure inference backbone**, providing model orchestration, auditability, and consistent governance across AI workflows.

---

## **7️⃣ Agent-Core Services**

**Q:** Are you involved in designing the agent-core services?

**A:**
Yes — I was directly involved in designing our **agent-core architecture**.

It includes:

- **Task Planner Service** – breaks complex workflows into sub-tasks
- **Context Manager** – persists short- and long-term context (DynamoDB + S3)
- **Tool Registry** – defines approved tools & RBAC access
- **Policy & Audit Service** – applies guardrails and OpenTelemetry tracing

I defined their boundaries, communication (EventBridge + gRPC), and compliance mechanisms — ensuring modular, traceable, and secure agent orchestration.

---

## **8️⃣ RAG Architecture Example**

**Q:** Let’s say you’re asked to build a simple RAG app with 20 documents — what are the major components?

**A:**
A RAG system has four main stages:

1. **Ingestion & Preprocessing** – upload docs to S3, clean and chunk text
2. **Embedding & Vector Store** – generate embeddings (Titan) and store in OpenSearch or pgvector
3. **Retrieval Layer** – semantic + lexical search, rank top chunks
4. **Generation & Orchestration** – pass context to Bedrock LLM for grounded responses

We wrap the flow with **observability (CloudWatch + OTel)**, **security (KMS, IAM)**, and **traceability** for HIPAA compliance.

---

## **9️⃣ Scaling RAG from 20 → 20,000 Documents**

**Q:** How would you scale the RAG application to thousands of documents?

**A:**
To scale:

- **Pipeline:** Move to Step Functions + Lambda for batch embedding
- **Storage:** Use OpenSearch or Pinecone for scalable ANN retrieval
- **Hybrid Retrieval:** Semantic + lexical with reranking
- **Caching:** Redis for hot queries
- **Observability:** recall@k, latency, token cost
- **Security:** RBAC and PII sanitization

We treat embedding and retrieval as continuous data pipelines, not one-time steps, ensuring scalability and governance.

---

## **🔟 Chunking Strategies**

**Q:** What chunking strategies do you use?

**A:**
Chunking balances **context retention and retrieval accuracy**.

Common strategies:

- **Fixed-size (500–1000 tokens)**
- **Sliding window overlap (10–30%)**
- **Semantic chunking (by heading or paragraph)**

Example:
A 5k-token doc → 500-token chunks with 100-token overlap = ~13 chunks.

We track metrics like **recall@k**, **chunk density**, and **embedding cost** to tune chunking efficiency.

---

## **11️⃣ Vector Database Selection**

**Q:** Which vector database do you use?

**A:**
In AWS, **Amazon OpenSearch (k-NN)** is our preferred vector store — it’s scalable, supports hybrid search, and aligns with IAM/KMS security.

For smaller PoCs, we sometimes use **pgvector (Aurora)**; for cross-region scale, **Pinecone** is an option.

OpenSearch gives us **low-latency retrieval**, hybrid search (semantic + lexical), and **managed observability** via CloudWatch.

---

## **12️⃣ Embedding Dimensions**

**Q:** When you vectorize, what embedding dimensions do you use?

**A:**
Dimensions are model-defined:

- **Titan Embeddings:** 1,024
- **OpenAI Ada:** 1,536
- **Cohere:** 768

We typically stay between **768–1,024 dimensions** — balancing semantic richness and query latency.

Higher dimensions = better recall, higher cost.
Storage ≈ `num_vectors × dimension × 4 bytes`.
We sometimes use **PCA or OPQ compression** for large-scale optimization.

---

## **13️⃣ Post-Vectorization Workflow**

**Q:** After vectorization, what’s next to build the RAG app?

**A:**
The flow continues with:

1. **Query Embedding** – embed the user query
2. **Retrieval** – search in vector DB for top-K chunks
3. **Reranking** – refine with lexical filters or cross-encoders
4. **Context Assembly** – build structured prompt with doc refs
5. **Generation** – call Bedrock LLM
6. **Governance** – sanitize, log, and audit results

In short: **Retrieve → Rank → Generate → Govern**.

---

## **14️⃣ Retrieval & Citation Flow**

**Q:** How do you retrieve context and show citations in the UI?

**A:**
Each retrieved chunk is tagged with an index `[1]`, `[2]` and doc metadata (title, section).
We embed those references directly into the prompt so the LLM can cite them.

After generation, we parse these references and map them back to document metadata, showing them as clickable citations in the UI.

This provides **traceability**, **explainability**, and supports **Responsible AI compliance**.

---

## **15️⃣ Front-End Frameworks**

**Q:** Do you use Streamlit or React/Angular for chat apps?

**A:**

- **Streamlit / Gradio:** for internal demos or PoCs (Python-native).
- **React / Next.js / Angular:** for enterprise deployments with authentication and audit logging.

At McKesson, we use **React**, connected via **API Gateway** to Bedrock APIs.
The UI streams responses, manages state, and renders citations dynamically.

---

## **16️⃣ Streaming Responses**

**Q:** Our Bedrock chatbot returns responses as a single block. How does streaming work in LLMs?

**A:**
LLMs generate **tokens sequentially** — streaming APIs let you receive tokens as they’re produced.

In **Bedrock**, use `InvokeModelWithResponseStream` (Python SDK):

```python
response = bedrock.invoke_model_with_response_stream(...)
for event in response["body"]:
    chunk = event["chunk"]["bytes"].decode("utf-8")
    yield chunk
```

The backend sends chunks via **SSE or WebSocket**; the UI appends them live, giving the “typing” effect.

Streaming improves **UX**, reduces perceived latency, and allows mid-generation **monitoring and compliance hooks**.

---

## **17️⃣ Collaboration with Tech Leads and Architects**

**Q:** How do you typically collaborate with Tech Leads and Architects?

**A:**
Whenever new features or architecture changes arise, the **Tech Lead** is engaged early — especially during **research spikes**.

We collaborate to:

1. **Validate feasibility**
2. **Identify dependencies & risks**
3. **Refine architecture artifacts**

Architects define the _what and how_, while Tech Leads operationalize it.
We close the loop through **PI/sprint planning** to align architecture and delivery.

This ensures **architecture evolves with implementation feedback** and remains practical.

---

# **✅ End of Q&A**

---
