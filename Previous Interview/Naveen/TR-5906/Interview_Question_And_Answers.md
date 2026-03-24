# Java Full Stack Interview Q&A (Azure + Microservices)

## 1. What types of testing are done on package releases? What tools are used?

**Answer:**

We follow multiple types of testing:

- **Unit Testing** – JUnit, Mockito  
- **Integration Testing** – Spring Boot Test  
- **API Testing** – Postman, Rest Assured  
- **End-to-End Testing** – Cypress / Selenium  
- **Performance Testing** – JMeter  
- **Regression Testing** – Automated suites  

We also integrate tests into CI/CD pipelines using **Azure DevOps** and use **SonarQube** for code quality.

---

## 2. Have you done performance testing on backend applications?

**Answer:**

Yes, we used **JMeter** for load and stress testing of Spring Boot APIs.

- Measured response time and throughput  
- Identified bottlenecks in DB queries  
- Optimized using indexing and query tuning  
- Implemented Azure Functions (async processing)  

Monitoring was done using **Azure Application Insights**.

---

## 3. What databases have you used?

**Answer:**

- **Relational Databases:** MySQL, Azure SQL  
- **NoSQL Database:** MongoDB  

Used:
- Spring Data JPA  
- Spring Data MongoDB  

Worked on:
- Joins  
- Indexing  
- Stored procedures  
- Query optimization  
- Performance tuning  

---

## 4. Experience with containerization and orchestration?

**Answer:**

- **Docker** for containerization  
- **Kubernetes (AKS)** for orchestration  

Used:
- Dockerfiles  
- Deployments  
- Services  
- ConfigMaps  
- Secrets  

Integrated with Azure DevOps CI/CD pipelines.

---

## 5. What CI/CD tools have you used?

**Answer:**

Used **Azure DevOps**:

- Build pipelines (CI)  
- Release pipelines (CD)  
- Automated testing  
- Deployment to AKS  

Integrated with:
- Docker  
- Azure Container Registry (ACR)  

---

## 6. What tools are used for monitoring?

**Answer:**

- Azure Application Insights  
- Azure Monitor  
- Log Analytics  

Tracked:
- Request latency  
- Failure rates  
- Exceptions  

---

## 7. How does alerting work?

**Answer:**

Used Azure Monitor + Application Insights:

Alerts based on:
- Response time  
- Errors  
- CPU usage  

Notifications via email  

Custom alerts using Log Analytics queries.

---

## 8. How do you identify errors in applications?

**Answer:**

- Use Application Insights for:
  - Exceptions  
  - Stack traces  

- Use Log Analytics for log queries  

- Trace requests using **Correlation IDs**  

Then fix and deploy using Azure DevOps pipeline.

---

## 9. What Azure cloud services have you used?

**Answer:**

- AKS – Orchestration  
- Azure Functions – Async processing  
- Azure SQL – Database  
- ACR – Image storage  
- Azure DevOps – CI/CD  
- Application Insights – Monitoring  
- Key Vault – Secrets management  

---

## 10. Experience with Azure SQL?

**Answer:**

Used for structured data (billing, claims)

Worked on:
- SQL queries  
- Indexing  
- Stored procedures  
- Performance tuning  

Integrated using Spring Data JPA.

---

## 11. Have you used Azure Service Bus?

**Answer:**

Yes, used for asynchronous communication:

- **Queues** → Point-to-point  
- **Topics** → Pub-Sub  

Features:
- Decoupling services  
- Dead Letter Queue (DLQ)  
- Retry mechanism  

---

## 12. What tool is used for orchestration?

**Answer:**

**Kubernetes (AKS)**

Flow:
Docker → ACR → AKS

Used:
- Deployments  
- Services  
- Auto-scaling  

---

## 13. How did you test frontend components?

**Answer:**

- Unit Testing – Jest / Karma / Jasmine  
- Integration Testing – API + UI  
- E2E Testing – Cypress / Selenium  
- Manual testing for UI validation  

Integrated with CI/CD pipelines.

---

## 14. Experience with Vitest?

**Answer:**

Used for frontend unit testing  

- Faster than Jest  
- Supports:
  - Mocking  
  - Assertions  
  - Coverage  

---

## 15. Coding Question (Employee Filter)

### Pseudocode:
create empty list result

for each employee in employeeList:
    if employee.salary > 5000:
        name = employee.name
        uppercaseName = convert name to uppercase
        add uppercaseName to result

return result

### Java Code:
```java
public static List<String> getEmployeeNames(List<Employee> employeeList) {
    List<String> result = new ArrayList<>();

    for (Employee employee : employeeList) {
        if (employee.getSalary() > 5000) {
            String name = employee.getName();
            String uppercaseName = name.toUpperCase();
            result.add(uppercaseName);
        }
    }

    return result;
}
```

---

## Tip for Interview

- Keep answers short and structured  
- Use real project examples  
- Mention tools + impact (performance, optimization, scaling)
