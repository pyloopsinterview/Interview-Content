# 📄 Interview Q&A – Claims Processing Platform (Mayank Patel)

---

## 1. Can you walk through the discrete elements of the claims processing platform and your involvement?

**Answer:**
- The platform consisted of five main layers:
  1. Data Ingestion Layer  
  2. Data Processing & Normalization  
  3. AI/NLP Layer  
  4. Generative AI (RAG) Layer  
  5. API/Serving Layer  

- **My involvement:**
  - Designed ingestion pipelines using Flask APIs and asynchronous messaging (Pub/Sub)
  - Built normalization pipelines for structured and unstructured data
  - Integrated NLP models (spaCy, Hugging Face)
  - Designed and implemented RAG pipelines using LangChain
  - Defined APIs and ensured end-to-end system integration
  - Led architecture discussions and deployment using Vertex AI

---

## 2. What strategy did you use for data normalization?

**Answer:**
- Used a **hybrid approach**:
  - Schema mapping for structured data
  - Rule-based transformations (date formats, currency normalization)
  - NLP + OCR for unstructured data
  - Regex for predictable patterns (e.g., policy IDs)

- Designed a **canonical schema**
- Built modular transformation pipelines via Flask microservices
- Ensured extensibility for new data sources

---

## 3. How did you decide confidence thresholds for detection?

**Answer:**
- Driven by **business impact + model performance**
- Used **precision-recall analysis** to determine optimal cutoffs
- High threshold (~90%+) for critical fields (claim amount, policy ID)
- Lower thresholds for non-critical fields
- Aligned with:
  - Error tolerance
  - Manual review load
  - SLA requirements

- Continuously monitored and adjusted thresholds in production

---

## 4. Were your roles full-time or contract?

**Answer:**
- Most recent roles were **contract-based (C2C)**
- Worked through consulting company
- Responsibilities were **equivalent to full-time roles**
- Owned design, development, and deployment

---

## 5. What are the top 5 things you personally worked on?

**Answer:**
1. End-to-end Claims Processing AI Platform  
2. RAG pipeline using LangChain  
3. NLP-based entity extraction and classification  
4. MLOps with Vertex AI (deployment, monitoring, drift handling)  
5. Microservices architecture (Flask + Kubernetes)

---

## 6. Did team members work independently or collaboratively?

**Answer:**
- Each engineer owned a **specific module**
- Strong collaboration across:
  - API contracts
  - Data schemas
  - Integration points
- Regular syncs ensured alignment
- Integration phases involved close collaboration

---

## 7. Which cloud platform did you use?

**Answer:**
- Used **Google Cloud Platform (GCP)**
- Services:
  - Pub/Sub → async messaging  
  - GKE → container orchestration  
  - Cloud Storage → document storage  
  - Vertex AI → ML lifecycle  
- Designed a **cloud-native, event-driven architecture**

---

## 8. What was the team composition?

**Answer:**
- ~10 members:
  - 5–6 Backend/Full-stack engineers  
  - 2 ML/NLP engineers  
  - 1–2 Data engineers  
  - 1 QA engineer  
- Also worked with Product Manager & Business Analyst
- My role: **Technical Lead + hands-on contributor**

---

## 9. Who did you communicate with and how did requirements flow?

**Answer:**
- Worked with:
  - Product Manager → requirements  
  - Business Analysts → domain inputs  
  - Engineers → implementation  

- Process:
  - Convert business needs → technical design
  - Define schemas, APIs, and workflows
  - Follow Agile (sprints, standups, demos)

- Acted as a **bridge between business and engineering**

---

## 10. Who owned the architecture?

**Answer:**
- Senior Architect:
  - Defined high-level architecture  
  - Cloud strategy, standards  

- My role:
  - Owned **component-level design**
  - Designed AI pipelines, RAG workflows, data processing
  - Collaborated with architect for alignment

---

## 11. Were you doing both design and hands-on engineering?

**Answer:**
- Yes, balanced both:
  - ~40% design  
  - ~60% hands-on coding  

- Approach:
  - Early phase → architecture & design  
  - Later phase → development + integration  

- Ensured:
  - No bottlenecks  
  - Clear ownership across team  

---

## 12. Who was doing the design exactly?

**Answer:**
- **High-level design:** Senior Architect  
- **Detailed/component design:** Myself  

- Owned:
  - AI pipelines  
  - Data flows  
  - Service interactions  

- Collaborated and validated designs with architect

---

# 🔥 Key Strengths Demonstrated

- End-to-end AI system ownership  
- Strong backend + AI integration  
- Production-level MLOps knowledge  
- Business-aligned ML decision-making  
- Leadership + collaboration  

---

# 🚀 Optional Next Prep

- Behavioral Q&A (STAR format)  
- System Design (Whiteboard explanation)  
- LLM / RAG Deep Dive Questions  
