# PBG Full Stack Engineer – Questions & Answers

---

## 1. Explain how a system that connects a Tailwind/HTMX UI to a FastAPI backend that queries a RAG system using Claude on Bedrock and returns a visualized response in Chart.js.

### Answer:

The Tailwind + HTMX frontend sends user queries via AJAX to a FastAPI backend endpoint. The FastAPI service orchestrates a RAG pipeline: it embeds the query, retrieves top-k relevant documents from a vector store (e.g., pgvector or FAISS), constructs a structured prompt, and sends it to Claude via AWS Bedrock. Claude returns a grounded response. The backend formats structured JSON output which is sent back to the frontend. Chart.js then consumes this JSON and renders visualizations dynamically without a full page reload.

---

## 2. A deployment to ECS succeeds, but the frontend can’t reach the API. Walk through how you would troubleshoot using CloudWatch, ALB logs, and Prometheus metrics.

### Answer:

First, I check ALB target group health status to ensure ECS tasks are healthy. Then I review ALB access logs to confirm if requests are reaching the load balancer and inspect response codes (404, 502, 503). Next, I analyze CloudWatch logs for ECS containers to check for startup errors or binding issues (wrong port). I verify security groups and networking (public/private subnets). Finally, I review Prometheus metrics for latency, error rates, and CPU/memory spikes to detect resource exhaustion or scaling issues.

---

## 3. How do you implement authentication and role-based access control across frontend, API, and AI services?

### Answer:

Authentication is implemented using JWT tokens issued by an identity provider (e.g., AWS Cognito). The frontend stores tokens securely and sends them in Authorization headers. The FastAPI backend validates JWT signatures and extracts user roles. Role-based access control (RBAC) is enforced via middleware or dependency injection. Backend services use IAM roles for secure access to Bedrock and S3. Sensitive services remain in private subnets and use least-privilege IAM policies.

---

## 4. Build a FastAPI endpoint for an AI-powered query system.

### Requirements:
- POST /query  
- Pydantic validation  
- Async handling  
- Store in PostgreSQL  
- Return UUID  
- Handle 400/500  
- Bonus: Auth + Rate limiting  

### Answer:

```python
from fastapi import FastAPI, HTTPException, Depends
from pydantic import BaseModel
import asyncpg, uuid, os

app = FastAPI()
DB_URL = os.getenv("DATABASE_URL")

class Query(BaseModel):
    user_id: str
    query: str

async def verify_token(token: str):
    if token != "secure-key":
        raise HTTPException(401, "Unauthorized")

@app.post("/query")
async def query_ai(data: Query, token: str = Depends(verify_token)):
    request_id = str(uuid.uuid4())
    try:
        conn = await asyncpg.connect(DB_URL)
        await conn.execute(
            "INSERT INTO queries(id,user_id,query) VALUES($1,$2,$3)",
            request_id, data.user_id, data.query
        )
        await conn.close()
        return {"request_id": request_id}
    except asyncpg.PostgresError:
        raise HTTPException(400, "Database error")
    except Exception:
        raise HTTPException(500, "Internal server error")


 5. Design and implement a Retrieval-Augmented Generation (RAG) pipeline.
Python Implementation:
import boto3, json, faiss, numpy as np
from sentence_transformers import SentenceTransformer

model = SentenceTransformer("all-MiniLM-L6-v2")
bedrock = boto3.client("bedrock-runtime")
index = faiss.IndexFlatL2(384)
docs = []

def ingest(text):
    chunks = [text[i:i+500] for i in range(0, len(text), 500)]
    emb = model.encode(chunks)
    index.add(np.array(emb))
    docs.extend(chunks)

def rag(query):
    q_emb = model.encode([query])
    _, I = index.search(np.array(q_emb), 3)
    context = "\n".join([docs[i] for i in I[0]])
    prompt = f"Answer only from context:\n{context}\nQ:{query}"

    res = bedrock.invoke_model(
        modelId="anthropic.claude-v2",
        body=json.dumps({
            "prompt": prompt,
            "max_tokens_to_sample": 200,
            "temperature": 0.2
        })
    )
    return json.loads(res["body"].read())
Hallucination Prevention:

Ground responses in retrieved context

Strict prompt instructions

Low temperature

Limit top-k

Cost Optimization:

Cache embeddings

Limit token usage

Optimize chunk size

Latency Optimization:

Async calls

ANN search

Small context window

6. Design a production-ready architecture for an AI-powered SaaS application.
Architecture Flow:

User → ALB → ECS Fargate (FastAPI) →
RDS PostgreSQL (metadata + pgvector) →
S3 (documents) →
AWS Bedrock (Claude)

Monitoring: CloudWatch + Prometheus

Security Model:

JWT Authentication (Cognito)

RBAC in FastAPI

IAM roles for ECS

Secrets Manager

Private subnets for RDS/ECS

TLS + encryption at rest

Scaling & HA:

ECS Auto Scaling

Multi-AZ RDS

ALB across AZs

Read replicas

Stateless containers

7. Broken Code Fix
Original Code:
@app.post("/query")
def query_ai(data: dict):
    response = call_claude(data["query"])
    db.save(response)
    return response
Fixed Version:
from fastapi import FastAPI, HTTPException
from pydantic import BaseModel

app = FastAPI()

class Query(BaseModel):
    query: str

@app.post("/query")
async def query_ai(data: Query):
    try:
        response = await call_claude(data.query)
        await db.save(response)
        return response
    except KeyError:
        raise HTTPException(400, "Invalid input")
    except Exception:
        raise HTTPException(500, "Internal error")

Improvements:

Async function

Pydantic validation

Error handling

Secured input validation