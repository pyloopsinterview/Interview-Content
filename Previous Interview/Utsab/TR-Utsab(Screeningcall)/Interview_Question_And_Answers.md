# Interview Q&A – Backend / Full Stack (Healthcare + Platform)

---

## 1. Introduction

**Q: Can you introduce yourself?**

**Answer:**

Hi, my name is Utsab. I’m a Lead Full Stack Developer with around 13 years of experience, primarily focused on building scalable backend systems and full-stack platforms.

Currently, I’m working with Health First, where I design and build production-grade applications using TypeScript, React, GraphQL, Go, and Python. Over time, my role has become more backend-focused, especially around distributed systems, API design, and service orchestration.

In my current project, I work on a member care and provider interaction platform. One of the key features I owned end-to-end was improving the appointment scheduling and eligibility experience.

On the frontend, I built reusable React components using TypeScript. On the backend, I designed GraphQL APIs, worked on schema design and resolvers, and contributed to Go-based microservices handling eligibility and scheduling workflows.

I also worked with Python services for background processing and reporting. I typically work across the full lifecycle—from design to deployment and production support—and I also mentor junior engineers and conduct design reviews.

---

## 2. Understanding the Project (LabCorp / Monolith)

**Q: Do you understand the project setup and challenges?**

**Answer:**

Yes, from what I understand, this is a central backend monolith that acts as the core orchestration layer for multiple workflows like test catalog management, lab processing, genetic interpretation, and reporting.

It integrates with external systems like EHRs using FHIR data and also connects with provider-facing and patient-facing applications.

The main challenge seems to be integrating this system with LabCorp’s larger ecosystem while managing technical debt and preparing for long-term migration.

This is similar to systems I’ve worked on, where a central service coordinates multiple workflows and integrates with downstream services. I’m comfortable handling such backend-heavy, distributed workflows and evolving systems.

---

## 3. AWS Experience

**Q: What is your experience with AWS?**

**Answer:**

I have solid experience working in AWS-based environments, mainly from a backend and platform perspective.

In my current role, services are deployed on AWS using container-based architectures like ECS. I’ve worked with services like S3 for storage, Lambda for lightweight processing, and CloudWatch for monitoring.

I’ve also worked with asynchronous workflows using queues, handling retries and ensuring system reliability.

In terms of CI/CD, I’ve worked with pipelines that automate deployments into AWS environments.

While I’m not deeply focused on infrastructure provisioning, I’m very comfortable building and running backend systems in AWS and collaborating with DevOps teams.

---

## 4. ML / GPT / TensorFlow Question

**Q: Can you use GPT-2 with TensorFlow? Isn’t TensorFlow diagnostic?**

**Answer:**

GPT-2 is a model architecture, and it can be used with frameworks like PyTorch or TensorFlow.

TensorFlow is not diagnostic—it’s a general-purpose deep learning framework, similar to PyTorch.

In practice, GPT-2 is more commonly used with PyTorch, especially through libraries like Hugging Face Transformers.

In my experience, I haven’t trained models like GPT-2 from scratch, but I’ve worked with Python-based services that integrate ML models into backend systems.

My strength is more on the application and integration side—building APIs and systems around ML models rather than training them.

---

## 5. Terraform / Infrastructure

**Q: Do you have experience with Terraform?**

**Answer:**

I’ve had exposure to Terraform through collaboration with DevOps teams.

I’ve worked in environments where infrastructure is managed using Terraform, so I understand concepts like modules, variables, and environment configurations.

My primary focus has been on backend and application development, but I’m comfortable working within Terraform-managed environments, debugging issues, and aligning application design with infrastructure.

If needed, I can quickly pick up more hands-on Terraform work.

---

## 6. Current Role / Availability

**Q: What is your current situation?**

**Answer:**

I’m currently working with Health First, but my contract is expected to end next Friday.

So I’m actively exploring new opportunities and would be available to start immediately after that.

---

**Q: Why is your contract ending?**

**Answer:**

It was a contract role tied to a specific project scope, and now that the major deliverables are complete, the engagement is coming to an end.

---

## 7. Questions You Asked Interviewer

**Q: What questions do you have for us?**

**Answer:**

I had a few questions:

1. From an architecture standpoint, how are you planning to evolve the monolith? Are you moving toward modularization or services over time?

2. What are the biggest challenges currently in integrating with LabCorp systems? Is it more around data consistency, workflows, or interoperability?

3. How do you balance technical debt with ongoing feature development?

4. How do backend engineers collaborate with data engineering and DevOps teams?

5. What would success look like for this role in the first 3 to 6 months?

---

## 8. Follow-up Response (After Interviewer Feedback)

**Q: Response when interviewer said “ask Doug later”**

**Answer:**

Got it, that makes sense—that’s helpful.

I’ll definitely bring that up with Doug, especially around the long-term architecture and modernization approach.

From what you described, it sounds like a lot of the current work is around integrating with LabCorp’s ecosystem and ensuring everything works reliably together.

That’s something I enjoy working on—especially evolving existing systems, improving integrations, and gradually modernizing without disrupting workflows.

---

## 9. Closing Statement

**Q: Final impression**

**Answer:**

This role aligns really well with what I enjoy working on—backend-heavy systems, complex workflows, and evolving architectures—so I’d be really excited to contribute here.

---

# End of Document