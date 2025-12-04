Absolutely — here are the **exact questions asked** in Round-3 **with the exact answers you gave** (cleaned and structured for reuse).
No paraphrasing of questions. No additional commentary.

You can copy-paste this and practice directly.

---

# **Round-3 Interview — Exact Q&A**

### **Q1. Give me a brief introduction about yourself.**

**A:**
My name is Jaydev Bhatia. I’m a Lead DevOps & Cloud Engineer with 12+ years of experience building scalable, automated cloud platforms across AWS and Azure. I specialize in Kubernetes (EKS/AKS), Terraform IaC, and CI/CD automation.
At NextEra, I lead cloud modernization — EKS multi-region architectures, Fargate migrations, GitOps pipelines, and full observability. I focus on secure, resilient automation that accelerates delivery and improves platform reliability.

---

### **Q2. What are the areas where you feel you provide the most value?**

**A:**

- Cloud Architecture & Automation
- Kubernetes Platform Engineering
- Terraform modular design
- Secure CI/CD + DevOps transformations
- Coaching development/SRE teams
  I build strong, automated cloud foundations that enable teams to deliver faster and safer.

---

### **Q3. What are you looking for in your next position?**

**A:**
A role where I can influence architecture decisions, drive automation standards, improve reliability, mentor engineers, and help scale a secure cloud platform that supports rapid delivery and growth.

---

### **Q4. Did Lane explain how they have the architecture set up in AWS?**

**A:**
Yes — multi-account setup, API Gateway routing, Lambda workloads being migrated to Fargate, CloudWatch/X-Ray observability, CloudFlare governance, and upcoming GitHub Enterprise adoption.
There is strong opportunity to standardize Terraform modules, CI/CD, observability, and governance.

---

### **Q5. You managed EKS clusters in a multi-region setup. Describe that architecture.**

**A:**
At Apple:

- Multi-AZ EKS clusters deployed in multiple regions
- Route53 + Global Accelerator for active-active traffic routing
- Istio mesh + HPAs for resiliency
- Aurora Global DB for low-latency replication
- Terraform modules + ArgoCD GitOps
- Prometheus Thanos + Loki + X-Ray for global observability
  We performed chaos tests — failover had zero customer impact.

---

### **Q6. Do you have experience with EKS using Fargate?**

**A:**
Yes — hybrid model with EC2 node groups + Fargate profiles.
Fargate for lower-traffic workloads and stronger isolation.
EC2 nodes for high-throughput services, DaemonSets, bottleneck handling.
Scheduling by namespaces/labels. Terraform automation + CloudWatch/X-Ray monitoring.

---

### **Q7. You’ve used multiple IaC tools. If it’s a new AWS project, what would you choose and why?**

**A:**
Terraform.
It’s multi-cloud, highly modular, faster at adopting AWS services, easier collaboration with state management, and integrates well with security and CI/CD governance.
Used as primary IaC in NextEra across multi-account EKS/Fargate/VPC infrastructure.

---

### **Q8. Kubernetes security appears strong in your resume. What protocols do you enforce?**

**A:**

- Private clusters + network policies
- RBAC with principle of least privilege
- **IRSA** for fine-grained IAM
- OPA Gatekeeper for Pod Security policies (no privileged pods, required limits, etc.)
- Trivy/Snyk image scanning before deployment
- GitOps governance + Falco runtime security
  Defense-in-depth across infra, cluster, workload, and pipeline layers.

---

### **Q9. If you could pick your CI/CD tool for a new project, what would you choose?**

**A:**
GitHub Enterprise + GitHub Actions.
Strong ecosystem, modular reusable workflows, secure OIDC integration with AWS, great container support, and excellent developer experience.
ArgoCD for deployment → full GitOps workflow.

---

### **Q10. What is your approach to monitoring and observability?**

**A:**
Unified visibility:

- Metrics: Prometheus + CloudWatch SLO dashboards
- Logs: FluentBit + Loki/Elastic
- Traces: X-Ray + OpenTelemetry
- Synthetics: CloudWatch Canaries
- PagerDuty for smart alert routing
  Standard dashboard templates and correlation IDs for fast RCA.

---

### **Q11. Do you have experience with other cloud platforms besides AWS?**

**A:**
Yes — strong Azure (AKS, Bicep, APIM, Key Vault, DevOps Pipelines) and solid GCP (GKE, Pub/Sub, Cloud Build).
Terraform + Kubernetes allow consistent automation across clouds.

---

### **Q12. Do you have any questions for us?**

**A:**
Yes:

- How is DevOps structured today at IPFS?
- What priorities will this role focus on in first 3–6 months?
- Current maturity of observability + incident response?
- What does success look like in year one?

---

## ✔ Ready-to-Use Closing Line (Use verbatim)

**A:**
I’m excited about this opportunity because the direction you’re heading aligns perfectly with my strengths in cloud architecture, Kubernetes standardization, and DevOps automation. I feel I can make a meaningful impact very quickly.

---

If you'd like, I will also create:

✔ A **1-page cheat sheet** to review right before the call
✔ A **final closing pitch** tailored specifically to hiring manager
✔ A **90-day plan** you can present proactively (huge impact)

Would you like me to generate those next?
