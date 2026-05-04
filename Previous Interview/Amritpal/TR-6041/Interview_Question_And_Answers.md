# Amritpal Interview Q&A

## 1. Experience Overview

**Q:** How many years of experience do you have?  
**A:** I have around **12 years of IT experience**, with **9–10 years of hands-on experience in Python development**.

---

## 2. Other Programming Languages

**Q:** Have you worked on any languages other than Python?  
**A:** Yes, apart from **Python**, I have strong experience with **JavaScript**, especially using **React** for frontend development. My primary focus has been on **Python (backend)** and **React (frontend)**.

---

## 3. Global Interpreter Lock (GIL)

**Q:** What is the Global Interpreter Lock (GIL)?  
**A:** The **GIL (Global Interpreter Lock)** is a **mutex** that allows only **one thread to execute Python bytecode at a time** in **CPython**. It simplifies **memory management (reference counting)** but limits **true parallelism in multithreading**.

---

## 4. Multiprocessing vs GIL

**Q:** How does multiprocessing work with GIL?  
**A:** In **multiprocessing**, each process has its own **Python interpreter and GIL**, so it enables **true parallel execution** across **multiple CPU cores**, bypassing GIL limitations.

---

## 5. Concurrency vs Parallelism

**Q:** What is the difference between concurrency and parallelism?  
**A:**  
- **Concurrency** → Managing multiple tasks (not necessarily at the same time)  
- **Parallelism** → Executing multiple tasks **simultaneously** using multiple cores  

---

## 6. Execution Phases

**Q:** What are the execution phases?  
**A:**  
- **Ready** → Waiting for CPU  
- **Running** → Executing  
- **Waiting/Blocked** → Waiting for I/O  
- **Completed** → Finished execution  

---

## 7. Concurrency Modes in Python

**Q:** What are different ways to achieve concurrency?  
**A:**  
- **Multithreading** → I/O-bound tasks  
- **Async/Await (asyncio)** → Non-blocking concurrency  
- **Multiprocessing** → CPU-bound tasks  
- **Event-driven systems** → Async workflows  
- **Distributed systems** → Microservices-based concurrency  

---

## 8. Concurrency Tools in Python

**Q:** What tools are used for concurrency in Python?  
**A:**  
- **threading**  
- **asyncio**  
- **multiprocessing**  
- **concurrent.futures**  
- **queue**  

---

## 9. LRU Cache

**Q:** What is LRU Cache?  
**A:** **LRU (Least Recently Used)** cache removes the **least recently accessed item** when the cache reaches its **maximum capacity**.

---

## 10. Django vs Flask

**Q:** When do you use Django vs Flask?  
**A:**  
- **Django** → Full-featured, fast development, built-in features  
- **Flask** → Lightweight, flexible, ideal for **APIs and microservices**  

---

## 11. PUT vs PATCH

**Q:** Difference between PUT and PATCH?  
**A:**  
- **PUT** → Full resource update (replace entire object)  
- **PATCH** → Partial update (modify specific fields only)  

---

## 12. Server-side Validation

**Q:** How do you implement server-side validation?  
**A:**  
- Validate **input data (schema validation using Pydantic/DRF)**  
- Apply **business logic validation**  
- Use **database constraints (UNIQUE, NOT NULL)**  
- Return proper **error responses (400/422)**  
- Prevent **security issues (SQL Injection, XSS)**  

---

## 13. WHERE vs HAVING

**Q:** Difference between WHERE and HAVING?  
**A:**  
- **WHERE** → Filters rows before aggregation  
- **HAVING** → Filters grouped data after aggregation  

---

## 14. Database Indexing

**Q:** Benefit and drawback of indexing?  
**A:**  
- **Benefit** → Faster **read/query performance (SELECT)**  
- **Drawback** → Slower **write operations (INSERT/UPDATE/DELETE)** + extra storage  

---

## 15. AWS Cloud Experience

**Q:** What cloud experience do you have?  
**A:**  
- Worked on **AWS (EC2, Lambda, S3, RDS, API Gateway)**  
- Built **microservices and event-driven systems**  
- Implemented **CI/CD pipelines**  
- Used **CloudWatch for monitoring**  

---

## 16. EC2 Deployment Steps

**Q:** Steps to deploy application on EC2?  
**A:**  
1. Launch **EC2 instance**  
2. Connect via **SSH**  
3. Setup **environment (Python, dependencies)**  
4. Deploy **code (Git clone)**  
5. Run app using **Gunicorn**  
6. Configure **Nginx**  
7. Setup **process manager (systemd)**  

---

## 17. Load Balancer & Scaling

**Q:** How do you handle scaling in AWS?  
**A:**  
- Use **Application Load Balancer (ALB)** to distribute traffic  
- Use **Auto Scaling Groups (ASG)** for dynamic scaling  
- Ensures **high availability and fault tolerance**  

---

## 18. CI/CD Tools

**Q:** What CI/CD tools have you used?  
**A:**  
- **AWS CodePipeline, CodeBuild, CodeDeploy**  
- **GitHub Actions / GitLab CI**  
- **Jenkins**  

---

## 19. React Experience

**Q:** What is your experience with React?  
**A:**  
- Built **dashboards and UI components** using **React (hooks)**  
- Integrated **REST APIs**  
- Developed **monitoring dashboards** for real-time systems  
- Focused on **reusable components and performance**