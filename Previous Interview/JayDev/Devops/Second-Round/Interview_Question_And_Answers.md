# 🧩 AWS DevOps | GitLab | Kubernetes | CI/CD | Security

### All Technical Questions Asked Today (No Code Included)

---

## ✅ 1. How do you restrict communication between Kubernetes pods?

Use **Kubernetes NetworkPolicies** (requires Calico/Cilium CNI).

- Apply a default deny policy (Ingress + Egress)
- Allow only explicitly permitted pod-to-pod communication using labels
- Enforce zero-trust model inside the cluster

➡ Restricts pod communication and prevents lateral movement.

---

## ✅ 2. How do you ensure security while setting up AWS infrastructure?

Security best practices include:

| Area       | Best Practice                                                          |
| ---------- | ---------------------------------------------------------------------- |
| IAM        | Least privilege policies, role-based access with OIDC (no access keys) |
| Networking | Private subnets, deny-all SG rules, VPC firewalling                    |
| Encryption | Enable KMS encryption at rest and TLS in transit                       |
| Secrets    | Store in AWS Secrets Manager, not in code or pipeline                  |
| Monitoring | CloudTrail, GuardDuty, AWS Config, CloudWatch Alerts                   |

➡ Security is applied at design time, not after deployment.

---

## ✅ 3. How do you deploy a third-party vendor Docker image to a secure (banking) Kubernetes cluster?

Precautions include:

- Verify image authenticity (signature validation)
- Scan image for vulnerabilities (supply-chain security)
- Require SBOM (Software Bill of Materials)
- Store image in internal/private registry (never pull directly from vendor registry)
- Deploy first in an isolated non-production namespace
- Enforce pod security (non-root, least privilege, read-only filesystem)
- Deployment only via GitOps (Argo CD), no manual kubectl

➡ “Verify → Scan → Internal registry → Sandbox → Deploy securely”

---

## ✅ 4. What is Blue-Green deployment?

Blue-Green deployment is a **zero-downtime deployment strategy**.

- Blue = current production version
- Green = new version deployed in parallel
- After validation, traffic is switched from Blue → Green
- Rollback = switch back to Blue instantly

➡ Provides instant rollback and safe releases.

---

## ✅ 5. How did you use Argo CD?

Used for **GitOps-based Kubernetes deployments**.

- Syncs Kubernetes manifests/Helm charts from Git
- Ensures cluster state always matches Git state
- Auto-heals if someone manually edits cluster configuration
- Rollback is as simple as reverting Git commit

➡ Argo CD automates Continuous Delivery, not CI.

---

## ✅ 6. How do you use Argo CD in CI/CD pipelines?

- CI: GitLab builds & pushes the image
- CD: Argo CD monitors Git and deploys the new version automatically
- Argo CD continuously reconciles desired vs. actual cluster state

➡ GitLab pushes changes, Argo CD pulls and applies them (GitOps).

---

## ✅ 7. How do you use Helm charts with Argo CD?

- Helm defines the templates and configuration
- Argo CD deploys the Helm chart and manages versions
- Each environment (Dev/QA/Prod) has its own Helm values file

➡ Helm = templating, Argo CD = deployment and drift correction.

---

## ✅ 8. What sensitive parameters do you consider while designing a pipeline for NFT (Non-Functional Testing)?

Key concerns:

| Area                  | What I ensure                                             |
| --------------------- | --------------------------------------------------------- |
| Data                  | No PII or live customer data; synthetic data only         |
| Secrets               | Secure handling using Secrets Manager or secure variables |
| Environment isolation | NFT runs in separate namespace/subnet                     |
| Cost optimization     | Auto destroy environment after testing                    |
| Observability         | Enable logs, metrics, tracing, dashboards                 |

➡ NFT should mimic Prod but without Prod risks.

---

## ✅ 9. What is the most expensive cost in AWS?

**Data Transfer Costs**, especially:

- Cross-AZ traffic inside same region
- Region → region traffic
- Internet data egress

➡ Compute is cheap; chatty architecture is expensive.

---

## ✅ 10. What are the limitations of AWS Lambda?

| Limitation             | Detail                                        |
| ---------------------- | --------------------------------------------- |
| Execution time         | Max 15 minutes                                |
| Cold starts            | Delay on first request (impact for Java/.NET) |
| Stateless              | No persistent storage                         |
| Package size           | Limited deployment size                       |
| Concurrency throttling | Can impact downstream systems                 |

➡ Use Lambda for short-running, event-driven workloads.

---

## ✅ 11. How do you use AWS Lambda?

Used Lambda for:

- ETL automation
- Event-driven processing
- AI pipeline orchestration (S3 → Bedrock → DynamoDB)
- CI/CD hooks and automation tasks

➡ Lambda is ideal for automation and glue logic.

---

## ✅ 12. What SDKs do you use?

| SDK               | Usage                                       |
| ----------------- | ------------------------------------------- |
| boto3 (Python)    | Automation, provisioning, Bedrock           |
| AWS SDK v2 (Java) | Real-time stream processing (Flink/Kinesis) |
| GitLab API        | Pipeline automation and approvals           |

➡ Python + boto3 is primary for DevOps tasks.

---

## ✅ 13. What languages are you comfortable with?

| Language   | Comfort | Where used                      |
| ---------- | ------- | ------------------------------- |
| Python     | 9/10    | Automation, AWS Lambda, Bedrock |
| Java       | 8/10    | Streaming, backend              |
| TypeScript | 7/10    | Frontend dashboards             |
| SQL        | 7/10    | Analytics, ETL                  |

➡ Python = DevOps automation; Java = streaming workloads.

---

## ✅ 14. What is GitLab?

GitLab = All-in-one DevOps platform.

Used for:

- Version control (SCM)
- CI/CD pipelines
- Security scans (SAST, Dependency scanning)
- Infrastructure automation (Terraform apply via pipeline)

➡ GitLab manages entire delivery lifecycle.

---

## ✅ 15. What did you use GitLab Duo (AI assistant) for?

- Auto-generating CI/CD pipeline YAML
- Reviewing Terraform/IAM changes for security issues
- Troubleshooting failed pipelines
- Reducing time to create MR pipelines

➡ AI-assisted DevOps acceleration.

---

---

## ✅ 16. How do you ensure secure artifact deployment / supply-chain security?

Steps:

- Validate signature (image signing)
- Vulnerability scan
- Import to internal private registry
- Deploy to sandbox first
- Apply GitOps-based deployment via Argo CD
- Enforce restrictive security context (least privilege containers)

➡ Trust nothing. Validate everything.

---

## ✅ 17. How do you secure CI/CD pipelines?

- Remove access keys; use IAM OIDC federation
- Use GitLab protected variables
- SAST / SCA scanning enabled
- Peer-reviewed merge requests
- Audit logs & RBAC

➡ Secrets never stay in the pipeline or repo.

---

## ✅ 18. Why ArgoCD + GitLab instead of GitLab-only?

- GitLab manages CI: build/test
- Argo CD manages CD: deploy/sync/drift correction

➡ GitLab = Push automation  
➡ Argo CD = Pull automation (GitOps)

---

# 🔥 Final One-Liner

> **GitLab automates CI. Argo CD automates CD. Kubernetes enforces zero trust. AWS enforces least privilege.**

---
