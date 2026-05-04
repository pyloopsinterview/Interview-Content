# Interview Preparation - Latif Khan (Senior Python Developer)

---

## 1. Introduction (Job Description Aligned)
Hi, my name is Latif. I have around **12 years of experience** in **software engineering**, mainly focused on **Python backend development**.

Currently, I’m working as a **Senior Python Developer** at **Sumitomo Pharma**, where I design and build **scalable, cloud-native backend systems**.

I have strong hands-on experience with **FastAPI**, building **RESTful APIs**, and designing **microservices architectures**.

I’ve worked with **MongoDB and SQL databases**, and implemented **event-driven systems using Kafka** for handling large-scale data.

One of my key projects was an **AI-powered KYC onboarding platform**, where we automated document verification using **AI agents (Google ADK)**.

I also have experience with **Docker, CI/CD pipelines, AWS**, and follow **Agile methodologies**.

---

## 2. Other / Dominant Experience
I also bring experience in:
- **Cloud platforms (AWS)** for scalable deployments  
- **Docker** for containerization  
- **CI/CD pipelines** for automation  
- **ETL/Data processing workflows**  
- **AI/Generative AI systems**  
- Working in **Agile environments with cross-functional teams**

---

## 3. Common Character in Array of Strings
### Approach:
Convert each string into a **set**, then apply **intersection**.

```python
names = ["Latif", "My Name", "Romesh Kosh"]
sets = [set(name.lower()) for name in names]
common_chars = set.intersection(*sets)
common_chars.discard(' ')
print(common_chars if common_chars else "No common character")
```

---

## 4. Repeated Characters in String
- Loop through characters  
- Use **isalpha()**  
- Use **count()**  
- Store only unique repeated characters  

---

## 5. Character Frequency using Dictionary
```python
string = "latifsheetalbhaskar"
char_count = {}

for char in string:
    char_count[char] = char_count.get(char, 0) + 1

for char, count in char_count.items():
    if count > 1:
        print(char, count)
```

---

## 6. Common Characters in Array
```python
arr = ["latif", "sheetal", "bhaskar"]

common_chars = set(arr[0])

for word in arr[1:]:
    common_chars &= set(word)

print(common_chars)
```

---

## 7. __init__ vs __new__
- **__new__** → responsible for **object creation**
- **__init__** → responsible for **initialization**

We override:
- **__init__** → to customize object values  
- **__new__** → for advanced control like **Singleton or immutable objects**

---

## 8. Generators
Generators use **yield** and support **lazy evaluation**.

Benefits:
- **Memory efficient**
- **Processes large data**
- Generates values **on demand**

---

## 9. Backend Architecture
We follow **layered architecture**:

Client → API → Service → Repository → Database

- API → handles requests  
- Service → business logic  
- Repository → DB operations  
- Database → storage  

---

## 10. Third Party Integration
Handled via **Service Layer** to keep separation of concerns.

---

## 11. MongoDB Structure
Hierarchy:
Server → Database → Collection → Document → Fields

---

## 12. Data Storage
- Stored in **BSON format**
- Managed by **WiredTiger engine**
- Uses **compression + indexing**

---

## 13. Authentication
- **JWT tokens**
- **Role-based access (RBAC)**
- Secure API access

---

## 14. Third Party Failure Handling
- **Fallback mechanism**
- **Caching**
- **Retry logic**
- **Circuit breaker**

---

## 15. Memory Management
- Python uses **Garbage Collection**
- Use **generators**
- Clean resources properly

---

## 16. CI/CD Strength
- Automated pipelines  
- Build + test + deploy  
- Docker + AWS  
- Rollback strategy  

---

## 17. CI vs CD
- CI → **integration + testing**
- CD → **deployment**

---

## 18. Git Workflow
pull → branch → code → add → commit → push → PR

---

## 19. After PR
- CI runs  
- Code review  
- Fixes  
- Approval  
- Merge  

---

## 20. Competencies
- Python  
- FastAPI  
- MongoDB  
- Kafka  
- CI/CD  
- Security  

---

## 21. Scale
- Handles **thousands of users/month**
- Supports **millions of records**

---

## 22. MongoDB Collections
- candidates  
- documents  
- kyc_status  
- users  

---

## 23. Strength Summary
- Scalable backend systems  
- Microservices architecture  
- Cloud-native design  
- AI integration  

---

