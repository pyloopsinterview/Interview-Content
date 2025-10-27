# Interview Questions Asked to Murali Mohan Rao Nagulapally

## **Date:** October 27, 2025

# Python and React Interview Q&A

---

## 1. Can you introduce yourself?

**Answer:**
Hi, my name is Amritpal Singh, and I have over 12 years of experience in data
engineering and ETL development, specializing in Python, Snowflake, Control-M,
and Data Warehousing also I do have extensive experience on AWS services like
Lambda,S3, SNS, SQS, CloudWatch. Currently, I’m working with AmerisourceBergen
as a Senior Python ETL Developer.
In my current role, I’m primarily responsible for designing and developing robust ETL
pipelines to process and integrate large volumes of healthcare and pharmaceutical
data across multiple sources.
One of the key projects I’ve led at AmerisourceBergen is the “Pharma Distribution
Data Modernization Initiative”, where our goal was to migrate legacy ETL workflows
from Informatica and Oracle into a modern, cloud-based Snowflake data platform.
I designed Python-based ETL frameworks that extracted data from various
upstream systems — including ERP, logistics, and order management — transformed it using Pandas and PySpark, and then loaded it efficiently into
Snowflake using Snowpipe and Streams/Tasks.
We scheduled and orchestrated the workflows through Control-M, implementing
event-driven triggers and dependency management to ensure reliability and
minimal downtime.
I also worked closely with the data governance and analytics teams to build
reusable data models, define data quality checks, and create automated validation
scripts that improved data accuracy and reduced manual intervention.
Apart from development, I also contribute to code reviews, and Mentor my Junior
developer is they are stuck in something i pare program with them.

---

## 2. In Python ecosystem, what frameworks, libraries, or modules have you used mostly? How did you talk to the databases?

**Answer:**
I have mostly used the following in the Python ecosystem:

- **Flask** and **FastAPI** for backend REST API development.
- **NumPy**, **Pandas**, and **Matplotlib** for data analysis and visualization.
- **SQLAlchemy** and **PyMongo** for database interaction.

**Example:**

```python
from sqlalchemy import create_engine
engine = create_engine("mysql+pymysql://user:password@localhost/dbname")
connection = engine.connect()
result = connection.execute("SELECT * FROM users")
```

---

## 3. What about unit testing?

**Answer:**
I have used **unittest** and **pytest** frameworks for unit testing.

- Used **pytest fixtures** and **mocking** for isolating dependencies.
- Integrated with **CI/CD** pipelines to run automated test suites.

**Example:**

```python
def add(a, b):
    return a + b

def test_add():
    assert add(2, 3) == 5
```

---

## 4. It’s a gap right, Murali? You have completed, you know, 1994 something, right?

**Answer:**
Yes, there is a gap. During that time, I focused on personal development and upskilling myself with modern technologies like Python, React, and Node.js to stay current in the industry.

---

## 5. What is GIL in Python?

**Answer:**
**GIL (Global Interpreter Lock)** is a mutex that ensures only one thread executes Python bytecode at a time in CPython.

- It simplifies memory management.
- However, it prevents true parallel execution of threads for **CPU-bound** tasks.
- **I/O-bound** tasks can still benefit from multithreading.

---

## 6. To take advantage of the multi-core architecture, how will we do it if there is a mutex lock always and there is a single thread we can use?

**Answer:**
We can use the **multiprocessing** module instead of threading.

- Each process runs in its own Python interpreter, bypassing the GIL.
- Allows true parallelism on multiple CPU cores.

**Example:**

```python
from multiprocessing import Pool

def square(n):
    return n * n

if __name__ == "__main__":
    with Pool(4) as p:
        print(p.map(square, [1, 2, 3, 4]))
```

---

## 7. What is IO-bound and CPU-bound?

**Answer:**

- **IO-bound** tasks: Spend most time waiting for input/output operations (e.g., network calls, file reads).
- **CPU-bound** tasks: Spend most time performing computations (e.g., data processing, number crunching).

---

## 8. For IO-bound or CPU-bound, which one should be used for which?

**Answer:**

- **IO-bound → Multi-threading** (because threads can switch during I/O wait).
- **CPU-bound → Multiprocessing** (because it uses multiple CPU cores in parallel).

---

## 9. How does Garbage Collection (GC) work in Python?

**Answer:**
Python uses **reference counting** and **cyclic garbage collection**:

- Each object has a reference count.
- When the count drops to zero, memory is freed.
- The cyclic GC detects and collects objects involved in reference cycles.

You can control it via the `gc` module:

```python
import gc
gc.collect()
```

---

## 10. What frameworks have you used for Analytics?

**Answer:**

- **NumPy** → Numerical computations.
- **Pandas** → Data cleaning and manipulation.
- **Matplotlib / Seaborn** → Visualization.
- **Scikit-learn** → Machine learning.
- **FastAPI** → Serving analytics results via APIs.

---

## 11. What about TensorFlow and PyTorch?

**Answer:**
Yes, I’ve worked with both:

- **TensorFlow** for production-level model deployment.
- **PyTorch** for research and experimentation, as it supports dynamic computation graphs.

Used them for:

- Building and training models.
- Data preprocessing with NumPy and Pandas.
- Model evaluation and visualization with Matplotlib.

---

## 12. Why is NumPy fast? What makes NumPy blazing fast?

**Answer:**
NumPy is fast because:

- It is **implemented in C**.
- Uses **vectorized operations** (avoiding Python loops).
- Stores data in **contiguous memory blocks** for cache efficiency.
- Supports **broadcasting** for fast array operations.

---

## 13. Example of a Python function having a few input and output pairs

**Question Example:**

```
Input 1: "ABCDEF", 2
Output 1: "BA", "DC", "FE"

Input 2: "ABCDEF", 3
Output 2: "CBA", "EDC"

Input 3: "ABCDEF", 4
Output 3: "DCBA", "FEDC"
```

**Answer:**

```python
def reverse_in_groups(s, n):
    result = []
    for i in range(0, len(s), n):
        result.append(s[i:i+n][::-1])
    return result

# Examples
print(reverse_in_groups("ABCDEF", 2))  # ['BA', 'DC', 'FE']
print(reverse_in_groups("ABCDEF", 3))  # ['CBA', 'EDC']
print(reverse_in_groups("ABCDEF", 4))  # ['DCBA', 'FEDC']
```

---

## 14. Give the code for reverse in groups.

**Answer:**

```python
def reverse_in_groups(s, k):
    return [s[i:i+k][::-1] for i in range(0, len(s), k)]

print(reverse_in_groups("ABCDEF", 2))  # ['BA', 'DC', 'FE']
```

---

## 15. Give the reverse of the given combination.

**Answer:**
To reverse a given string completely:

```python
s = "ABCDEF"
print(s[::-1])  # "FEDCBA"
```

If you want group-based reversal, use the `reverse_in_groups()` function above.

---

## 16. When should we use Redux and when Context API in React?

**Answer:**

- **Redux**:

  - For large-scale applications with complex global state.
  - When multiple components need shared data updates.
  - When you need debugging tools and middleware like `redux-thunk`.

- **Context API**:

  - For smaller applications or limited global state.
  - Simpler setup, less boilerplate.

**Rule:**

> Use Redux for large, complex state management.
> Use Context API for small or medium apps with simple global state.

---

## 17. Have you ever worked on a large-scale application? How to optimize the performance?

**Answer:**
Yes. Performance optimization strategies I’ve used include:

**Backend:**

- Query optimization and indexing.
- Redis caching.
- Asynchronous processing with Celery or asyncio.

**Frontend:**

- Lazy loading and code splitting.
- Memoization (`React.memo`, `useMemo`).
- Minimizing re-renders and reducing bundle size.

**Infrastructure:**

- CDN for static assets.
- Load balancers and auto-scaling groups in AWS.

---

## 18. We are trying to consume very large high-resolution images creating rendering issues; how can we stop that activity?

**Answer:**

- **Lazy load** images using `loading="lazy"`.
- **Compress/resize** images using services like **Cloudinary** or libraries like `sharp`.
- Convert images to **WebP** format.
- Implement **progressive image loading**.
- Set **max resolution limits** for uploads.

**Example:**

```jsx
<img src="image.webp" loading="lazy" alt="Optimized Image" />
```

---

```

---

Would you like me to add an **intro section** (like “Profile Summary – Murali Mohan, Python & React Developer”) at the top of this markdown file for a more professional touch?
```
