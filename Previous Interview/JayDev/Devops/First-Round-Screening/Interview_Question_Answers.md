Here’s your **interview Q&A document** in **Markdown (.md)** format — containing every question and answer you asked for this **Azure DevOps Architect** interview session:

---

# **Azure DevOps Architect Interview – Q&A (Jay)**

---

## **1. Brief Introduction**

Hi, I’m Jay — I have over **12 years of experience in DevOps and Cloud Engineering**, specializing in **Microsoft Azure, automation, and CI/CD architecture**.
Currently, I work as a **Lead DevOps Engineer at Nextera**, leading **cloud modernization and DevSecOps transformation** projects.
I’ve implemented end-to-end **CI/CD pipelines using Azure DevOps**, automated infrastructure with **Terraform**, and deployed containerized microservices on **AKS**.
My work reduced deployment time by **40%** with **zero manual intervention** and improved reliability and compliance.

---

## **2. Azure App Service Containers vs ACI vs AKS**

| Feature          | App Service Containers | Azure Container Instances | AKS                     |
| ---------------- | ---------------------- | ------------------------- | ----------------------- |
| Type             | PaaS                   | Serverless Container      | Managed Kubernetes      |
| Best for         | Web apps / APIs        | Short-lived jobs          | Microservices workloads |
| Scalability      | Simple auto-scale      | No orchestration          | Advanced scaling        |
| Infra management | None                   | None                      | Minimal                 |
| Deployment       | Image → ACR            | CLI/YAML                  | Helm / YAML             |

**Experience Line:**

> “I used AKS for microservices, App Service Containers for APIs, and ACI for short on-demand workloads.”

---

## **3. Deploying a Simple REST API with ACI**

- Build image → Push to **ACR**.
- Run:

  ```bash
  az container create --resource-group myRG --name rest-api --image myacr.azurecr.io/restapi:latest --ip-address public --ports 8080
  ```

- ACI provides instant deployment with no infra management — ideal for quick REST APIs.

---

## **4. Configure Environment Variables & Secrets in ACI**

- Use `--environment-variables` for plain values.
- Secure secrets via **Azure Key Vault + Managed Identity**:

  ```yaml
  environmentVariables:
    - name: DB_PASSWORD
      secureValue: "@Microsoft.KeyVault(SecretUri=https://myvault.vault.azure.net/secrets/dbpassword)"
  ```

- **Managed Identity** handles Key Vault access; no secrets in code/pipeline.

---

## **5. Use Azure Key Vault with Managed Identity**

Steps:

1. Enable Managed Identity on container.
2. Store secrets in Key Vault.
3. Grant access:

   ```bash
   az keyvault set-policy --name MyVault --secret-permissions get list --object-id <identity-id>
   ```

4. Reference in YAML (Key Vault reference).

**One-liner:**

> “Enable Managed Identity, assign access in Key Vault, and inject secrets dynamically — no secrets stored anywhere.”

---

## **6. GitHub Actions Workflow for Container Deployment**

**Flow:**

- Trigger on push → Checkout → Build → Login → Push to ACR → Deploy to AKS.

```yaml
- uses: azure/login@v1
- run: docker build -t myapp:${{ github.sha }} .
- run: az acr login --name myacr
- run: docker push myacr.azurecr.io/myapp:${{ github.sha }}
- run: helm upgrade --install myapp ./chart --set image.tag=${{ github.sha }}
```

**Best Practices:**

- OIDC Auth (no secrets).
- Image version tagging.
- Environment approvals.

---

## **7. Debug GitHub Action Authentication Failure**

Steps:

1. Check authentication step logs.
2. Verify GitHub secrets under **Settings → Secrets and Variables → Actions**.
3. Ensure correct RBAC (`Contributor`, `AcrPush`).
4. Test Azure login locally:

   ```bash
   az login --service-principal -u <client> -p <secret> --tenant <tenant>
   ```

5. Use:

   ```
   ACTIONS_STEP_DEBUG=true
   ```

**One-liner:**

> “I check logs, validate secrets, confirm RBAC, and test Azure login manually. Most issues are expired secrets or missing roles.”

---

## **8. Verify Secrets in GitHub Repo**

- Navigate to **Settings → Secrets → Actions**.
- Ensure secrets exist and match workflow variable names.
- Recreate or update expired Service Principal credentials.

---

## **9. CI/CD Difference – Azure DevOps vs GitHub Actions**

| Area          | Azure DevOps              | GitHub Actions    |
| ------------- | ------------------------- | ----------------- |
| Pipeline Type | YAML + Classic UI         | YAML only         |
| Integration   | Boards, Repos, Artifacts  | GitHub-native     |
| Approvals     | Release gates             | Environments      |
| Governance    | Strong enterprise support | Fast, lightweight |

**One-liner:**

> “Azure DevOps is full ALM; GitHub Actions is event-driven CI/CD — faster and simpler for modern apps.”

---

## **10. Provisioning Takes Too Long**

**Causes & Fixes:**

- Large Docker images → Use multi-stage builds.
- Infra recreated each run → Separate infra and app deployments.
- ACR latency → Enable geo-replication.
- Resource SKU slow → Scale appropriately.

**One-liner:**

> “I build infra once with Terraform, use smaller images, and optimize caching to cut provisioning time.”

---

## **11. Terraform Usage in Azure**

Steps:

1. `az login`
2. Configure backend in Azure Storage.
3. Define infra in `.tf` files.
4. Run:

   ```bash
   terraform init
   terraform plan
   terraform apply
   ```

**One-liner:**

> “I manage Azure infra as code using Terraform with remote state in Azure Storage and apply changes via CI/CD.”

---

## **12. Terraform Apply Fails Due to State Lock**

Steps:

1. Wait if another apply is in progress.
2. If stale lock →

   ```bash
   terraform force-unlock <LOCK_ID>
   terraform refresh
   terraform apply
   ```

**One-liner:**

> “I ensure no active apply is running; if lock is stale, I force unlock and refresh state safely.”

---

## **13. Zero Downtime Deployment Issues**

Zero-downtime may fail when:

- Stateful apps (session in-memory)
- Breaking DB migrations
- Single-instance apps
- Cold start or incompatible APIs

**One-liner:**

> “Zero downtime fails if the app isn’t stateless, DB changes aren’t backward compatible, or single-instance infra exists.”

---

## **14. Staging to Production Swap**

- Deploy to **Staging slot**.
- Warm-up → Validate → Swap with **Production slot**.
- Swap is instant & reversible.

**One-liner:**

> “Deploy to staging, test, and swap with production for zero downtime — rollback just swaps back.”

---

## **15. Multi-Environment CI/CD (Dev → QA → Prod)**

Flow:

- **Build once**, promote artifact across environments.
- Use approvals between stages.
- Separate secrets/configs via Key Vault or variable groups.

**One-liner:**

> “I use a build-once, promote-many pipeline with approvals and environment-based configs in Dev → QA → Prod.”

---

## **16. Best Practices for AKS Deployment**

- Use Helm or Kustomize.
- Store images in ACR (Managed Identity).
- Enable HPA, resource limits, probes, PDB.
- Key Vault for secrets.
- Use rolling/blue-green updates.

**One-liner:**

> “For AKS, I use Helm, ACR with MI, autoscaling, and Key Vault integration for secure, resilient deployments.”

---

## **17. Manage Secrets via Azure Key Vault CSI Driver**

Steps:

1. Enable Key Vault add-on in AKS.
2. Grant Managed Identity Key Vault access.
3. Create `SecretProviderClass`.
4. Mount secrets in pod via volume.

**One-liner:**

> “I use Key Vault CSI driver with Managed Identity to mount secrets securely into pods — no secrets in YAML or Git.”

---

## **18. Pod Keeps Restarting (CrashLoopBackOff)**

Steps:

1. `kubectl get pods`
2. `kubectl logs <pod>`
3. `kubectl describe <pod>`
4. Check probes, OOMKilled, missing secrets/configs.

**One-liner:**

> “I check logs, probes, resource limits, and secrets; fix configuration issues to stop the restart loop.”

---

## **19. Azure Service Running Slow**

Steps:

- Check Application Insights for latency.
- Check Azure Monitor for CPU/memory.
- Scale up/out if needed.
- Optimize DB/storage, enable caching, review network latency.

**One-liner:**

> “I isolate bottlenecks via Application Insights and Azure Monitor, then fix by scaling, caching, or optimizing dependencies.”

---

## **20. Insurance Domain Experience**

- Worked on **policy, claims, and billing** systems.
- Automated CI/CD for underwriting and claims apps.
- Integrated DevSecOps (SonarQube, Snyk, Defender).
- Ensured compliance for PII/PHI data.
- Reduced release time from days to hours via Terraform and Azure DevOps.

**One-liner:**

> “I supported insurance applications across policy, claims, and billing — automated deployments, ensured security, and improved release efficiency.”

---

✅ **End of Document**

---

Would you like me to export this as a downloadable **`.md` file** (Markdown format)?
