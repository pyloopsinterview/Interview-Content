# 📄 Interview Q&A -- **Murali Mohan Rao Nagulapally**

## **1. Brief Introduction**

Hi, my name is **Murali Mohan Rao Nagulapally**, and I have a little
over **12 years of experience** in Python development, API engineering,
and cloud-native microservices.

Recently at **Bon Secours Mercy Health**, I worked extensively on:

-   Python-based REST API development using **Django**
-   Containerizing microservices using **Docker**
-   Deploying into **Kubernetes (EKS)**
-   Automating CI/CD with **GitHub Actions**, improving deployment
    efficiency by **60%**

I modernized a legacy patient data retrieval system into a
**microservices-driven architecture** integrated with **Epic & Cerner**,
secured using **JWT**, and governed through multi-repo enterprise
standards.\
I have collaborated with cross-functional teams and mentored juniors on
API development and CI/CD.

I bring strong hands-on experience in **Python, Django, API design,
Docker, Kubernetes, and scalable architecture**.

------------------------------------------------------------------------

## **2. Write an API that processes an order, validates input, calculates total, and returns response**

``` python
from fastapi import FastAPI
from pydantic import BaseModel
from typing import List

app = FastAPI()

class OrderItem(BaseModel):
    name: str
    quantity: int
    price: float

class Order(BaseModel):
    customer_name: str
    items: List[OrderItem]

@app.post("/process-order")
def process_order(order: Order):
    total_amount = sum(item.quantity * item.price for item in order.items)

    return {
        "customer": order.customer_name,
        "total_bill_amount": total_amount,
        "status": "Order Processed Successfully"
    }
```

------------------------------------------------------------------------

## **3. Explain the Code & Approach**

The solution is structured using:

1.  **Pydantic BaseModels** to validate incoming JSON\
2.  **Business logic layer** to compute totals\
3.  **Clean JSON output** as API response

Automatic validation ensures all fields are properly typed and
mandatory.\
The total amount is computed by iterating over items (quantity ×
price).\
This approach is scalable and production-ready---logging, DB storage,
taxes, and discounts can be added easily.

------------------------------------------------------------------------

## **4. How Do You Handle JSON Data Validation?**

I use **Pydantic BaseModel** to validate request payloads before
execution.\
Validation ensures:

-   Mandatory fields exist\
-   Types are correct (str, int, float, etc.)\
-   Additional rules (min values, regex, enums) can be applied

This approach prevents runtime failures, enforces safety, and keeps APIs
robust and predictable.

------------------------------------------------------------------------

## **5. If Every API Call Needs Logging --- What Steps Do You Take?**

I use a **centralized logging layer**, not per-function logging.

Typically:

-   Logging is implemented via **middleware** or **dependency
    injection**
-   I capture request payloads, timestamps, routes, latency, and status
    codes
-   For distributed systems, I include **trace IDs / correlation IDs**
-   Logs are shipped to **ELK, Loki, or CloudWatch**

This ensures observability, debugging, and audit compliance.

------------------------------------------------------------------------

## **6. Modify Program to Process Multiple Orders & Return Average Value**

``` python
import json
from typing import List

def calculate_average_order_value(order_list: List[dict]):
    order_totals = []

    for order in order_list:
        total_amount = sum(item["quantity"] * item["price"] for item in order["items"])
        order_totals.append(total_amount)

    average_value = sum(order_totals) / len(order_totals)

    return {
        "total_orders": len(order_list),
        "order_totals": order_totals,
        "average_order_value": average_value
    }

with open("orders.json") as file:
    orders = json.load(file)

print(calculate_average_order_value(orders))
```

------------------------------------------------------------------------

## **7. How Do You Run a Container If You Already Have a Dockerfile? (sudo commands)**

``` bash
sudo docker build -t chatgpt-order-api:latest .

sudo docker run -d -p 8000:8000 --name order-api chatgpt-order-api:latest

sudo docker tag chatgpt-order-api:latest <dockerhub-user>/chatgpt-order-api:latest

sudo docker push <dockerhub-user>/chatgpt-order-api:latest

sudo kubectl apply -f deployment.yaml

sudo kubectl get pods

sudo kubectl logs -f <pod-name>

sudo kubectl apply -f service.yaml
```

------------------------------------------------------------------------

## **8. Sample Kubernetes Deployment Setup (sudo Commands)**

``` bash
sudo kubectl apply -f namespace.yaml

sudo kubectl apply -f deployment.yaml

sudo kubectl get deployments -n <namespace>

sudo kubectl get pods -n <namespace>

sudo kubectl describe pod <pod-name> -n <namespace>

sudo kubectl apply -f service.yaml

sudo kubectl get svc -n <namespace>

sudo kubectl scale deployment order-api --replicas=3 -n <namespace>

sudo kubectl rollout status deployment/order-api -n <namespace>
```
