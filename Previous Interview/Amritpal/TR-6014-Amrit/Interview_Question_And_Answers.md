# Interview Questions & Answers (Amritpal Singh)

---

## 1. Tell me about yourself
**Answer:**
Hi, I’m Amritpal Singh, a backend engineer with around 12 years of experience, primarily in Python.  
I’ve worked on building backend systems, APIs, and automation frameworks, especially in healthcare domains.

In my recent role at AmerisourceBergen, I worked as a Lead Python Developer where I designed and built a Python-based test harness from scratch to validate complex workflows across multiple systems.

I enjoy working on problems where systems are not well-defined and building scalable, reliable solutions from the ground up.

---

## 2. Do you have experience in biotech / healthcare workflows?
**Answer:**
I haven’t directly worked in genomics or bioinformatics pipelines, but I’ve worked extensively in healthcare systems with similar characteristics—complex data flows, integrations, and strict requirements around correctness and reliability.

---

## 3. What did your team look like?
**Answer:**
The team was cross-functional, around 6–8 engineers, mostly backend Python developers, along with frontend, QA, and a product manager.

I worked as a lead IC, responsible for system design, implementation, and mentoring.

---

## 4. What are you looking for next?
**Answer:**
I’m looking for a role where I can take ownership of system design and build scalable systems in complex, data-driven environments.

I enjoy working on ambiguous problems and building solutions that have meaningful impact, especially in healthcare.

---

## 5. How do you feel about working on maintenance or legacy systems?
**Answer:**
I’m very comfortable with it. Most real-world systems are not greenfield.

I focus on understanding the system, identifying pain points, and improving things incrementally—whether through refactoring, validation, or improving observability.

---

## 6. Your resume shows many technologies—how did you work with all of them?
**Answer:**
Those technologies reflect the ecosystem I worked in, not that I owned every part deeply.

My core strength is Python and backend systems.  
Other tools like Kafka, Docker, and Kubernetes were part of the system, and I interacted with them as needed.

---

## 7. What is your strongest area?
**Answer:**
My strongest area is backend engineering—Python, API development, system design, and building reliable data-driven workflows.

---

## 8. Describe an ETL pipeline you worked on
**Answer:**
I built Python services that pulled data from multiple APIs, normalized it, validated it, and stored it for downstream use.

Key issues:
- Data inconsistency → solved with validation and normalization
- Duplicate/out-of-order data → handled using idempotency and version checks

---

## 9. Did you build APIs or just test them?
**Answer:**
I’ve done both.

Earlier, I built backend APIs using Django/DRF.  
In my recent role, I focused on building a test harness to validate those APIs end-to-end.

---

## 10. What kind of APIs did you use?
**Answer:**
I used Django REST Framework to build REST APIs—JSON-based, with validation and consistent response structures.

---

## 11. Example of API interaction
**Answer:**
External systems (like pharmacies) would send order data via API.

My service would:
- Validate request
- Normalize data
- Store it
- Expose it internally for downstream systems

---

## 12. Did you work directly with vendors?
**Answer:**
No, I worked at the system integration layer—interacting with vendor systems via APIs rather than directly with organizations.

---

## 13. Is your system like Stripe API integration?
**Answer:**
Conceptually yes—API-based integration.

But unlike transactional APIs like Stripe, our systems handled complex data workflows with validation, retries, and consistency requirements.

---

## 14. What was your greenfield project?
**Answer:**
I designed and built a Python/Django-based test harness from scratch.

It simulated real workflows, triggered APIs, validated responses, and verified database state.

---

## 15. How did you use SageMaker?
**Answer:**
I integrated with SageMaker endpoints from backend services.

I sent input data, received predictions, and integrated results into workflows.  
I didn’t train models—only consumed them.

---

## 16. How did you use Camunda?
**Answer:**
We used Camunda for workflow orchestration.

I integrated Python services with it:
- Triggered workflows via REST APIs
- Used workers to execute tasks
- Handled validation, retries, and idempotency

---

## 17. Thoughts on AI usage in development
**Answer:**
AI helps improve productivity—especially for code generation and debugging.

But I treat it as an assistant.  
Final responsibility, validation, and correctness always remain with me.

---

## 18. Ethical use of AI
**Answer:**
- Avoid sensitive data in AI tools  
- Validate all outputs  
- Be transparent about usage  

If I can’t explain something, I won’t ship it.

---

## 19. Consequences of misrepresenting AI work
**Answer:**
- Loss of trust  
- Reduced credibility  
- Risk of incorrect systems  

Engineering requires ownership—AI output still needs validation.

---

## 20. Questions for interviewer
**Answer:**
- What are the biggest gaps in your current test framework?
- Are workflows event-driven or API-based?
- What does success look like in the first 3–6 months?

---

## 21. What stood out in the job description?
**Answer:**
- Building a test harness from scratch  
- Working with complex data workflows  
- Impact in healthcare systems  

---

## 22. Closing statement
**Answer:**
Thank you for your time—I really enjoyed the conversation and learning about your platform.

Looking forward to hearing from you.

---

# Summary Strengths
- Strong Python backend experience  
- System design & integration  
- Data validation & reliability  
- Experience with complex workflows  
