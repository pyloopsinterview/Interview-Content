**complete interview Q&A set** in clean, professional **Markdown (.md)** format — containing **every question you asked** and the **answers I crafted** for your **TCS – SRE Engineer** interview preparation (focused on GCP, Kubernetes, SRE practices, Terraform, GitHub Actions, and automation).

---

## 🧠 TCS – SRE Engineer Interview Q&A

**Candidate:** _Jaydev Bhatia_
**Experience:** 12+ Years | Lead DevOps & SRE | Cloud: GCP | Tools: Terraform, Kubernetes, Jenkins, GitHub Actions, ArgoCD, Grafana

---

### **1. Give me a brief introduction about your role, experience, projects, and responsibilities.**

Hi, my name is **Jaydev Bhatia**, and I’m currently working as a **Lead DevOps & Cloud Engineer** with **NextEra Energy** in **Juno Beach, Florida**.
I have around **12 years of experience** in **DevOps, SRE**, and **Cloud Engineering**, mainly across **GCP** environments.

In my current role, I focus on **cloud automation, infrastructure reliability**, and **CI/CD process improvement**.
I work extensively with **Terraform** for IaC, **Kubernetes** for container orchestration, and **Jenkins** and **GitLab CI** for automated deployments.

I also define and implement **SRE practices** like **SLIs, SLOs, and Error Budgets**, and use **Python and Bash** to automate repetitive tasks and reduce operational toil.
For observability, I use **Prometheus, Grafana**, and **Stackdriver** for monitoring and alerting.

Overall, my focus is on **building automation, ensuring reliability**, and maintaining **secure cloud operations** in a scalable way.

---

### **2. What is SRE (Site Reliability Engineering)?**

**SRE (Site Reliability Engineering)** combines **software engineering** with **IT operations** to make systems **reliable, scalable, and automated**.
It’s about treating operations as a **software problem**.

Core goals of SRE:

- Improve **reliability and availability**.
- Reduce **manual work (toil)** via automation.
- Measure performance through **SLIs, SLOs, and Error Budgets**.
- Balance **feature velocity** and **system stability**.

In short:

> **SRE = Reliability + Automation + Measurement**

---

### **3. Tell me about your GCP experience — what did you do there?**

In my current role, I’ve designed and managed **production-grade infrastructure** in **GCP**.

Key areas of work:

- **Infrastructure provisioning** using **Terraform** for GKE clusters, VPCs, Cloud SQL, IAM, and networking.
- **Kubernetes management** via **GKE**, with automated deployments through **ArgoCD** and **GitLab CI**.
- **Monitoring and alerting** with **Cloud Monitoring (Stackdriver)** and **Prometheus**, integrating with **Slack/Opsgenie**.
- **Toil automation** using **Cloud Functions**, **Pub/Sub**, and **Python scripts** to handle cleanup, scaling, and incident response.
- **Security** via IAM policies, service accounts, and Terraform guardrails.

Overall, I’ve focused on **automation, observability**, and **multi-environment reliability** in GCP.

---

### **4. Tell me about your experience with GitHub Actions and workflows.**

I use **GitHub Actions** to automate **CI/CD pipelines** and **IaC deployments**.

- **Build pipelines:** Automated Docker builds, testing, scanning, and deployment to **GKE** via **Helm**.
- **IaC pipelines:** Terraform integrated with GitHub Actions for provisioning GCP infrastructure using **OIDC authentication** (no long-lived credentials).
- **Reusable workflows:** Created shared CI/CD templates and composite actions for consistency.
- **Security:** Integrated **SonarQube**, **Trivy**, and **secret scanning**; enforced branch protection rules.
- **Notifications:** Automated **Slack and Jira** updates post-deployment.

> GitHub Actions became our unified automation platform for CI/CD, IaC, and release management — integrated tightly with Kubernetes and Terraform.

---

### **5. Tell me about your Terraform experience.**

I’ve been using **Terraform** as the core of our **Infrastructure-as-Code (IaC)** setup in **GCP**.

- Built reusable modules for **VPCs, IAM, GKE, Cloud SQL, and Firewalls**.
- Integrated Terraform into **GitHub Actions** for plan → review → apply workflows.
- Used **remote state** in **GCS buckets** and **Terraform Cloud**.
- Implemented policy controls via **Sentinel** and **pre-commit hooks**.
- Managed **multi-environment (dev, QA, prod)** provisioning through workspaces.

> Terraform helped make our infrastructure reproducible, secure, and fully automated — reducing provisioning time and human errors.

---

### **6. Can you tell me about your Kubernetes experience — what did you create or manage?**

I’ve been managing **Kubernetes clusters** in **GCP (GKE)** for microservices deployments.

- Built clusters via **Terraform**, automated deployments via **Helm** and **ArgoCD**.
- Implemented **GitOps workflows** for version-controlled, auto-sync deployments.
- Integrated **Prometheus + Grafana** for cluster monitoring and alerting.
- Secured workloads using **RBAC**, **NetworkPolicies**, and **image scanning**.
- Used **HPA and Cluster Autoscaler** for dynamic scaling.
- Automated rollbacks, backups (Velero), and namespace lifecycle scripts in **Python**.

> My Kubernetes setup focused on automation, observability, and security — ensuring zero-downtime and high availability.

---

### **7. Tell me about your experience with Jenkins and Grafana.**

I’ve used **Jenkins** extensively for **CI/CD pipelines** and **Grafana** for **monitoring and observability**.

- Built reusable **Jenkins pipelines** for build, test, Docker image creation, scanning, and GKE deployment.
- Integrated **Terraform** and **Vault/Secret Manager** for infrastructure and secrets management.
- Created **Grafana dashboards** linked with **Prometheus** and **Stackdriver** to monitor build performance, API latency, and SLO compliance.
- Automated alerts to **Slack** and **Opsgenie** for real-time incident notifications.

> Jenkins automated our deployments; Grafana ensured they stayed healthy and reliable.

---

### **8. Tell me about your toil automation work.**

In SRE, one of my goals has been to **reduce toil** — repetitive manual tasks that don’t scale.

Examples of what I automated in **GCP**:

- **Resource cleanup:** Python + Cloud Functions to auto-delete unused disks and test environments.
- **Incident response:** Cloud Monitoring alerts trigger **Pub/Sub** events → Cloud Functions restart failed pods or scale instances.
- **SLO reports:** Automated daily SLO compliance summaries into **BigQuery** for **Grafana dashboards**.
- **Rollback automation:** Cloud Build + ArgoCD auto-rollbacks for failed deployments.

> This reduced manual work, improved reliability, and allowed engineers to focus on innovation.

---

### **9. You mentioned SLO, SLA, and Error Budget — can you explain them?**

Sure — these are core to SRE:

- **SLI (Service Level Indicator):** The metric we measure — e.g., success rate or latency.
- **SLO (Service Level Objective):** The target goal — e.g., 99.9% availability.
- **SLA (Service Level Agreement):** The business-level promise to customers — e.g., 99.5% uptime per month.
- **Error Budget:** The tolerance for failure = `100% - SLO`.
  If SLO = 99.9%, error budget = 0.1% (≈43 mins/month).

We track these in **Cloud Monitoring** and **Grafana**; alerts trigger when the budget starts burning too fast.
It helps balance **innovation and reliability** — if the budget is healthy, we can deploy faster; if it’s exhausted, we focus on stability.

---
