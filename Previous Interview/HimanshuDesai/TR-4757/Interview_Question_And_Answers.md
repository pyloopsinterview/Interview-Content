# Interview Q&A – Himanshu Desai (Lead DevOps / GCP / FedRAMP)

---

## Q1. How long have you been working in your current role?
**Answer:**  
I’ve been in my current role at Early Warning for a little over **three years**. During this time, I’ve been deeply involved in building, operating, and scaling cloud and Kubernetes platforms in regulated, production environments.

---

## Q2. How do you make Infrastructure as Code (IaC) DRY and FedRAMP compliant?
**Answer:**  
I keep IaC DRY by using reusable Terraform/OpenTofu modules with opinionated defaults. Compliance is baked into the modules themselves—encryption, private networking, IAM least privilege, logging, and audit trails are mandatory. All changes go through Git-based CI/CD with reviews and policy checks, and controls are mapped back to NIST/FedRAMP requirements for auditability.

---

## Q3. If a Terraform state file in S3 is accidentally deleted but production is still running, how do you recover?
**Answer:**  
I don’t touch production resources. First, I restore the latest version from **S3 versioning**. If that’s not possible, I reinitialize Terraform and **import existing resources** back into state, validating everything with `terraform plan` only. The key is restoring or reattaching state without modifying live infrastructure.

---

## Q4. If a Terraform plan shows a destroy for a production bucket or database, what is your process?
**Answer:**  
I treat it as a hard stop. I pause the pipeline, analyze why the destroy is planned, fix the code or state (resource moves, imports, lifecycle `prevent_destroy`), and re-run the plan. Destruction only happens with explicit approval, backups verified, and controlled change windows.

---

## Q5. How do you manage 10 people working on the same Terraform codebase?
**Answer:**  
I use a remote backend with state locking, Git-based workflows with PRs and plan reviews, strong modularization with clear ownership, environment separation, and policy guardrails. No direct production applies from local machines.

---

## Q6. Can Terraform state files be stored in Git?
**Answer:**  
No. State files contain sensitive data, Git has no locking, and it leads to conflicts and security risks. Code goes in Git; state goes in a secure, versioned, locked remote backend.

---

## Q7. Do you have experience with GKE and microservices deployments?
**Answer:**  
Yes. I’ve worked extensively with GKE running containerized microservices using Helm and CI/CD pipelines, focusing on autoscaling, zero-downtime deployments, observability, and secure production operations.

---

## Q8. Describe a production issue you resolved in a microservices environment.
**Answer:**  
We had latency spikes due to database connection pool exhaustion. Pods scaled on CPU, but each pod opened too many DB connections. I adjusted HPA metrics, capped connection pools, improved probes, and added safeguards. Latency normalized and the issue didn’t recur.

---

## Q9. Was the Kubernetes cluster public or private?
**Answer:**  
It was a **private GKE cluster**—private control plane, no public IPs on nodes, and access restricted through private networking and controlled ingress.

---

## Q10. What type of Kubernetes environment was it?
**Answer:**  
A **managed private GKE environment** running production microservices with strong security, autoscaling, observability, and compliance controls.

---

## Q11. How do you implement zero-trust networking between microservices at Layer 7?
**Answer:**  
I use a service mesh (Istio / Anthos Service Mesh) with **mTLS**, strong workload identity, and explicit Layer-7 authorization policies. All traffic is encrypted, authenticated, authorized, and observable. This aligns directly with FedRAMP and NIST requirements.

---

## Q12. How do Gatekeeper or Kyverno fit into Layer 7 zero trust?
**Answer:**  
They don’t enforce traffic directly. Instead, they **prevent misconfigurations** by enforcing policies like mandatory mTLS, required authorization policies, restricted ingress, and security baselines at admission time. The service mesh enforces L7 traffic; Gatekeeper/Kyverno enforce compliance.

---

## Q13. How do you find logs in GKE?
**Answer:**  
I use **Google Cloud Logging (Logs Explorer)**, filtering by project, cluster, namespace, and pod. I correlate logs with Kubernetes events, metrics, and traces to isolate root causes.

---

## Q14. If logs are inside the container and not in Cloud Logging, how do you check them?
**Answer:**  
I use `kubectl logs` for stdout/stderr. If logs are file-based, I exec into the container and inspect the files directly. For crashed pods, I check `kubectl logs --previous`.

---

## Q15. Catalina.out is not stdout—how do you handle that?
**Answer:**  
I exec into the container and inspect `catalina.out`. For long-term fixes, I redirect logs to stdout or use a sidecar/logging agent to forward them to Cloud Logging so logs are centralized and auditable.

---

## Q16. How did you get alerted about the issue?
**Answer:**  
Alerts came from **Google Cloud Monitoring** based on metrics like latency, error rates, and pod restarts. Notifications were sent to **PagerDuty** and team chat channels.

---

## Q17. What exact tools do you use for alerts?
**Answer:**  
**Google Cloud Monitoring** for metrics and alerting, **PagerDuty** for on-call escalation, **Cloud Logging** for logs, and **Cloud Trace** for request tracing.

---

## Q18. Do you use Google Cloud Monitoring in production?
**Answer:**  
Yes. Cloud Monitoring is our primary production monitoring and alerting platform for GKE workloads.

---

## Q19. Do you have experience with MLOps?
**Answer:**  
Yes, from a **platform and operations perspective**. I’ve supported ML workloads on GKE by provisioning GPU clusters, automating infrastructure with Terraform, supporting Kubeflow pipelines, handling model packaging and deployment, monitoring training jobs, and securing ML workflows for production and compliance.

---
