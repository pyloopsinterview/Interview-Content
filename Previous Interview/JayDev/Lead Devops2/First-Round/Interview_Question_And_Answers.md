Here is the complete **Markdown file** containing **all questions asked during the interview + your correct answers**, formatted cleanly and professionally.

---

# **Citi Bank – Senior DevOps Engineer Interview Q&A**

### **Candidate: Jaydev Bhatia**

---

## **1. Tell me about your recent project, your role, and tasks you worked on.**

I worked as a Lead DevOps Engineer where I designed and automated a cloud-native platform on AWS using Terraform, Kubernetes (EKS), and Jenkins. My role involved building CI/CD pipelines, containerizing microservices, enabling GitOps, implementing automated deployments, and managing end-to-end infrastructure provisioning. I handled Terraform modules, multi-cluster Kubernetes setups, Helm deployments, CodeBuild/CodeDeploy pipelines, logging/monitoring automation, and zero-downtime production releases.

---

## **2. What is Terraform?**

Terraform is my primary Infrastructure-as-Code tool used to provision AWS resources like VPC, EKS, EC2, IAM, RDS, and networking using declarative code. I create reusable modules, manage S3 remote state with DynamoDB locking, and integrate Terraform into CI/CD pipelines to automate multi-environment deployments.

---

## **3. How long have you been working on AWS?**

I have over **7 years of hands-on AWS experience** designing, automating, and running large-scale cloud platforms.

---

## **4. Do you have hands-on experience with Terraform?**

Yes. I use Terraform daily to build AWS infra, manage remote state, create reusable modules, automate multiple environments, and integrate it with Jenkins and GitHub pipelines.

---

## **5. What is your experience in Kubernetes?**

I have **6+ years of production experience** with Kubernetes across EKS, GKE, and OpenShift. I manage multi-cluster setups, Helm deployments, autoscaling, ingress, GitOps, monitoring, logging, and troubleshooting. Kubernetes is one of my core strengths.

---

## **6. What are Kubernetes workloads?**

Workloads are resources that run applications in the cluster: Deployments, StatefulSets, DaemonSets, Jobs, and CronJobs. They define pod behavior, scaling rules, and lifecycle.

---

## **7. Explain Stateless vs Stateful in Kubernetes.**

- **Stateless (Deployment):** No data stored locally, pods are identical, used for APIs/microservices.
- **Stateful (StatefulSet):** Unique identity + persistent storage, used for Kafka, Redis, databases.

---

## **8. What is a PVC (Persistent Volume Claim)?**

PVC allows pods to use persistent storage that remains intact even if pods restart or move across nodes. Mainly used with StatefulSets and databases.

---

## **9. What are Kubernetes namespaces?**

Namespaces provide logical isolation inside a cluster. I use them to separate environments (dev/qa/prod), apply RBAC, enforce resource quotas, and manage access control.

---

## **10. What DevOps tools have you worked on inside and outside AWS?**

**Outside AWS:** Jenkins, GitHub, GitLab CI, Bitbucket, SonarQube, Nexus, Artifactory, Docker, Kubernetes, ArgoCD, Tekton, Prometheus/Grafana, ELK, Helm, Ansible, Terraform, Pulumi.
**Inside AWS:** CodeBuild, CodeDeploy, CodePipeline, ECR, EKS, EC2, Lambda, VPC, IAM, S3, CloudWatch, RDS, Secrets Manager.

---

## **11. Use case of a CI/CD pipeline you implemented.**

I built a pipeline that automated building containers, running unit/integration tests, SonarQube scans, pushing images to ECR, and deploying to EKS using Helm. Also implemented Terraform infra pipelines, GitOps pipelines with ArgoCD, and blue/green deployments using CodeDeploy.

---

## **12. What deployment tools do you use?**

I use **Jenkins**, **AWS CodeDeploy**, and **ArgoCD** for Kubernetes GitOps deployments.

---

## **13. Continuous workloads in Kubernetes**

Continuous workloads run all the time and use Deployments (stateless) or StatefulSets (stateful) depending on the workload’s data consistency needs.

---

## **14. What configurations do you set in GitHub, CodeBuild, and CodePipeline?**

### **GitHub**

- Branch protections
- PR checks
- Webhooks
- Secrets
- Pull request approvals

### **CodeBuild**

- buildspec.yml
- SonarQube integration
- IAM role
- Docker build + push to ECR
- Environment variables
- Caching

### **CodePipeline**

- Source → Build → Approval → Deploy stages
- Manual approval actions
- SNS notifications
- Integration with CodeDeploy/EKS

---

## **15. Summary of the CI/CD use case (long and humanized).**

I migrated a monolithic logging application into a containerized architecture and built a CI/CD pipeline with GitHub, CodeBuild, and CodePipeline. GitHub handled version control, branch protections, and PR validations. CodeBuild orchestrated the full build process including unit testing, integration testing, security scanning, Docker image creation, and pushing it to ECR. CodePipeline managed the entire flow with approval stages before deploying into QA/Prod. The deployment step used CodeDeploy or Helm-based EKS deployment depending on environment. This created a fully automated, auditable, and secure end-to-end release pipeline with proper governance.

---

## **16. Where have you used Python?**

I used Python for Lambda automation (EBS cleanup, IAM key rotation, EKS scaling), scripting in CI/CD pipelines, interacting with AWS via boto3, automating Kubernetes tasks, and building operational tools for deployment checks and system validation.

---

## **17. List vs Tuple**

- **List:** Mutable, dynamic, used for changing data.
- **Tuple:** Immutable, used for fixed configuration values.

---

## **18. Different AWS services you worked on**

EC2, EKS, ECS, Lambda, VPC, ALB/NLB, IAM, S3, RDS, DynamoDB, CloudWatch, CloudTrail, Route53, ECR, CodeBuild, CodeDeploy, CodePipeline, SNS, SQS, SSM, and Secrets Manager.

---

## **19. What is an Interface Endpoint (AWS PrivateLink)?**

It enables private access to AWS services via internal VPC network without internet or public IPs. It adds an ENI to the VPC for secure traffic.

---

## **20. What is AWS Transit Gateway?**

A central routing hub that connects multiple VPCs and on-prem networks and enables **transitive routing**, replacing complex VPC peering.

---

## **21. How do you classify a subnet as public or private?**

- **Public subnet:** Route table has route to Internet Gateway.
- **Private subnet:** No IGW route; usually routes via NAT Gateway or stays internal.

---

## **22. Purpose of provider.tf and backend.tf**

- **provider.tf:** Defines AWS provider, region, authentication.
- **backend.tf:** Defines remote backend for Terraform state (S3 + DynamoDB lock).

---

## **23. Difference between Stage, Job, and Task in pipelines**

- **Stage:** High-level pipeline phase (Build, Test, Deploy).
- **Job:** Group of tasks executed in a stage; can run parallel.
- **Task/Step:** Smallest action (commands/scripts).

---

## **24. GitHub practical workflow to commit a file**

- Clone repo
- Open in VS Code
- Modify file
- `git add`
- `git commit -m ""`
- `git pull`
- Fix conflicts
- `git push`
- Verify in GitHub

---

If you want, I can generate:

✅ PDF version
✅ DOCX version
✅ More detailed answers
✅ Shorter answers

Just tell me.
