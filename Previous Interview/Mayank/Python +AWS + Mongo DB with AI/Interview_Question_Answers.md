Below is the **complete Markdown file** with all the questions you asked and the senior-level answers provided — formatted cleanly so you can copy-paste and revise before your interview.

---

## 🧠 Senior Python + AI/Cloud Interview Q&A

**Profile Context:**
13+ years experience | Lead AI/ML Python Cloud Developer | Prudential Financial
Python · FastAPI · Flask · AWS · Lambda · ECS Fargate · SQS/SNS · Step Functions · MongoDB · Docker · CICD · AI Agent Framework

---

### **1. You have pretty good experience in Python, right? Have you used any design patterns?**

Yes. I have used multiple design patterns in production systems including:

- **Factory Pattern** for dynamic microservice object creation
- **Decorator Pattern** for cross-cutting concerns like logging & auth
- **Strategy Pattern** for choosing AI workflows dynamically
- **Singleton** for DB connection pools
- **Observer / Pub-Sub** in async event-driven pipelines

Example:
In our AI agent framework, we used Strategy + Factory patterns to dynamically route data validation logic based on claim type, enabling pluggable logic for future modules.

---

### **2. Do you know what a decorator is?**

Yes.
A decorator in Python is a higher-order function that wraps another function to extend its behavior **without modifying its code**.

We use decorators for authentication, input validation, tracing, and performance logging.

---

### **3. Do you know what Pub/Sub is?**

Yes.
Pub/Sub is **asynchronous event-driven communication** where producers publish messages and consumers subscribe to them without tight coupling.

In AWS, we use **SQS + SNS**, and in past projects Kafka for scalable message handling.

---

### **4. You mentioned Kafka — where did you use it?**

In a prior claims automation system, Kafka handled:

- High-volume claim event streaming
- Real-time notifications
- Fan-out processing to multiple AI microservices

It allowed us to handle burst traffic and ensure fault-tolerant processing.

---

### **5. What is your deployment process?**

We follow a CI/CD pipeline:

- PR review → Unit tests → Build Docker Image → Scan → Push to ECR
- Deploy via GitHub Actions to ECS Fargate / Lambda
- Canary release + automated rollback
- Post-deployment validation & CloudWatch alarms

---

### **6. So you deploy on AWS?**

Yes — full AWS stack:

- Compute: ECS Fargate, Lambda
- Networking: API Gateway, VPC, ALB
- Messaging: SQS, SNS, Step Functions
- Storage: S3, MongoDB Atlas, DynamoDB (PoCs)
- CI/CD: GitHub Actions + ECR + IaC (CDK/Terraform)

---

### **7. How do you manage environments?**

We maintain isolated environments:

- **dev → qa → uat → prod**
- Separate VPC & security config
- Version-specific environment configs
- Parameter Store / Secrets Manager for secure configs

---

### **8. Env variables — how do you store secrets?**

- **AWS Secrets Manager** for sensitive secrets
- **Parameter Store** for non-sensitive configs
- Local dev uses `.env` encrypted vault

---

### **9. Which databases are you familiar with?**

- MongoDB (Primary)
- DynamoDB (use case based)
- PostgreSQL
- Redis (caching & token store)

---

### **10. When do you choose MongoDB vs DynamoDB?**

| MongoDB                                       | DynamoDB                             |
| --------------------------------------------- | ------------------------------------ |
| Flexible schema, ACID trans., complex queries | Ultra-low latency, massive scale     |
| Good for document-based models                | Good for key-value & event workloads |

---

### **11. Have you worked on vector search?**

Yes, for text intelligence features.
Used **FAISS / Pinecone / AWS OpenSearch vector engine** to enable semantic search on policy & claim documents.

---

### **12. What is your tech stack? Any front-end?**

Backend heavy, but we do expose UI via:

- Next.js for dashboards
- Salesforce Lightning for enterprise UI
- React for internal ops portals

Primary stack: **Python, FastAPI, MongoDB, AWS, Docker**

---

### **13. How do agents communicate in your current AI agent framework?**

Agents communicate asynchronously via:

- AWS **SQS + SNS**
- Event-driven Step Functions
- S3 event triggers for ingestion
- Lambda orchestration

This decouples services and increases scalability & fault tolerance.

---

### **14. How are agents triggered?**

Main triggers:

- S3 event → Data ingestion agent
- CloudWatch schedule for batch runs
- Step Functions for chaining agents
- API trigger for manual workflows

---

### **15. How is data ingestion handled?**

- Source files uploaded to **S3**
- S3 triggers Lambda
- Lambda validates & cleanses data
- Data pushed to SQS → processed by agent microservices
- Output stored in MongoDB & processed downstream

---

### **16. Do you monitor this AI pipeline?**

Yes — using:

- CloudWatch
- AWS X-Ray tracing
- Prometheus/Grafana for performance
- Structured logs with correlation IDs
- Alerting on latency, queue depth, failures

---

### **17. Have you worked with LLMs?**

Yes — integrated pre-trained models and performed fine-tuning on domain datasets.
Used embeddings + retrieval pipelines for claim classification & policy servicing.

---

### **18. Is this something you did or your team?**

I designed the architecture, led the fine-tuning pipeline & guided engineers. Also personally implemented critical pipeline pieces.

---

### **19. Proud feature in Salesforce?**

Built dynamic form engine & role-based visibility rules for onboarding journeys.
Introduced caching layer & async pipelines → reduced page load by 40%.

---

### **20. Idempotency?**

Idempotency ensures an operation produces the **same result** even if executed multiple times.
We use idempotency keys in API layer to avoid duplicate processing in async pipelines.

---

### **21. REST vs SOAP**

| REST                         | SOAP                             |
| ---------------------------- | -------------------------------- |
| JSON, lightweight, stateless | XML, strict, enterprise security |
| Modern microservices         | Legacy financial/gov systems     |

Used both — Prudential still has SOAP core systems.

---

### **22. Handling API overload — debugging scaling issue**

- Check CloudWatch metrics
- Scale ECS tasks (HPA)
- Tune DB & connection pools
- Queue backpressure handling
- Introduce caching
- Circuit breakers & retry logic

---

### **23. Prevent abusive API calls / rate-limit strategy**

- AWS API Gateway throttling
- Redis rate limit tokens
- Token bucket / sliding window algorithm
- CAPTCHA & MFA for auth endpoints

---

### **24. Authentication vs Authorization**

| Auth        | AuthZ                   |
| ----------- | ----------------------- |
| Who you are | What you can access     |
| JWT login   | Role/scopes permissions |

---

### **25. OAuth2 — PKCE Flow**

PKCE used in public clients (mobile/web) to prevent code interception.
Generates **code_verifier + code_challenge** for secure token exchange.

---

### **26. JWT Authentication Flow**

- User sends creds → only via HTTPS
- Verify & hash pw (bcrypt/argon2)
- Issue **short-lived access token + long-lived refresh token**
- Access token inside header
- Refresh stored in HttpOnly cookie
- Token rotation & blacklist support

---

### **27. Refresh Token — explained**

Refresh token allows generating new access tokens without login.
Stored securely, supports rotation, device tracking & revocation.

---

### **28. When user sends credentials — do we send actual password?**

Yes, raw password travels but:

- **Only via HTTPS**
- Immediately hashed using **bcrypt/argon2**
- Never stored or logged
- We use brute-force protection & MFA

---

### **29. When user sends credentials — do we send actual password?**

def reverse_vowels_in_list(words: list[str]) -> list[str]:
vowels = "aeiouAEIOU"
result_list = []

    for s in words:
        # Extract vowels from the string
        vowel_list = [ch for ch in s if ch in vowels]
        # Reverse the vowels
        vowel_list.reverse()

        result = []
        vowel_index = 0

        for ch in s:
            if ch in vowels:
                result.append(vowel_list[vowel_index])
                vowel_index += 1
            else:
                result.append(ch)

        result_list.append(''.join(result))

    return result_list

# Example usage

input_list = ["hello world", "python", "example"]
output_list = reverse_vowels_in_list(input_list)

print("Input:", input_list)
print("Output:", output_list)

| Complexity Type | Big-O        | Explanation                 |
| --------------- | ------------ | --------------------------- |
| **Time**        | **O(n × m)** | Each string processed fully |
| **Space**       | **O(n × m)** | Output + temp vowel storage |
