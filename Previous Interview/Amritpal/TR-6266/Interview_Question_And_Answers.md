# Interview Questions & Answers (Python Backend / AWS / Data)

_Source Transcript:_ fileciteturn11file0

---

## 1. Tell me about your experience.
**Answer:**
I am a Senior Python Backend Engineer with around 12 years of experience building scalable APIs, cloud-native microservices, and data platforms.

---

## 2. What is your role in the current project?
**Answer:**
My primary role is backend development, but I also have some exposure to frontend technologies.

---

## 3. Are you involved in build and deployment (CI/CD)?
**Answer:**
Yes, I am involved in building applications, running unit and integration tests, packaging code, and deploying it using CI/CD pipelines.

---

## 4. Do you have experience with AWS Lambda?
**Answer:**
Yes, I have experience working with AWS Lambda for backend services and deployments.

---

## 5. How do you build and deploy a Python application?
**Answer:**
- Develop backend using FastAPI
- Write unit and integration tests
- Package dependencies
- Create deployment artifact
- Deploy using pipelines or cloud services (Lambda/ECS/EKS)

---

## 6. How would you deploy without Jenkins or pipelines?
**Answer:**
- Prepare code locally
- Manage dependencies using requirements.txt
- Package application manually
- Deploy to cloud services (Lambda, ECS, etc.)

---

## 7. How do you check equality between two objects in Python?
**Answer:**
- Use `==` for value comparison
- Use `is` for identity comparison

---

## 8. How to enforce a function to accept only string input?
**Answer:**
- Use type checking (`isinstance`)
- Use type hints
- Validate input inside function

---

## 9. How to remove duplicates from a list?
**Answer:**
Convert list to a set and back to list:
`list(set(data))`

---

## 10. What happens when you add duplicate values to a set?
**Answer:**
Duplicate values are ignored automatically.

---

## 11. What is a tuple?
**Answer:**
A tuple is an immutable collection of elements, similar to a list but cannot be modified after creation.

---

## 12. Difference between DataFrame and DynamicFrame?
**Answer:**
- DataFrame: Structured data (Pandas/Spark)
- DynamicFrame: Used in AWS Glue, supports semi-structured data

---

## 13. When do you use DynamicFrame?
**Answer:**
When working with semi-structured or inconsistent data in AWS Glue ETL pipelines.

---

## 14. How to group large data by customer ID?
**Answer:**
Use groupby operation in DataFrame:
`df.groupby("customer_id")`

---

## 15. Difference between multithreading and multiprocessing?
**Answer:**
- Multithreading: Good for I/O-bound tasks
- Multiprocessing: Good for CPU-bound tasks

---

## 16. When to use multithreading vs multiprocessing?
**Answer:**
- Multithreading → I/O tasks (API calls, DB)
- Multiprocessing → Heavy computation tasks

---

## 17. What is map and reduce in Python?
**Answer:**
- map: Applies function to each element
- reduce: Aggregates results into a single value

---

## 18. How do you handle exceptions in Python?
**Answer:**
Using try-except blocks to catch and handle errors.

---

## 19. Difference between else and finally in exception handling?
**Answer:**
- else: Executes if no exception occurs
- finally: Executes always

---

## 20. How to unit test AWS Glue jobs?
**Answer:**
- Separate logic from Glue-specific code
- Use mocks for AWS services
- Test logic locally

---

## 21. How to test Glue jobs locally without AWS?
**Answer:**
- Simulate environment using local tools
- Use Docker or AWS LocalStack
- Mock AWS services

---

## 22. Have you used AWS LocalStack?
**Answer:**
Yes, for simulating AWS services locally during development and testing.

---
