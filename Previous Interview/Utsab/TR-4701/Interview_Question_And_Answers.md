````md

\# Interview Questions and Answers (Complete)



---



\## 1. Where is your AI and ML background?

\*\*Answer:\*\*  

My background is primarily in full-stack and platform engineering, with AI and ML experience focused on applied, production use rather than research. I’ve worked closely with data science teams to integrate ML models into backend services using Python and Go. My responsibility was to expose these models through APIs, ensure scalability, security, monitoring, and make them usable in real business workflows. My strength is operationalizing AI—taking models from development to reliable production systems.



---



\## 2. Any AI agents or tools you are familiar with?

\*\*Answer:\*\*  

Yes. I’ve worked with LLM-based agents using Python frameworks like LangChain. These agents handled tasks such as intelligent search, summarization, and workflow automation. I’ve also integrated vector databases and third-party AI services into backend systems, focusing on reliability, cost control, and clean API exposure.



---



\## 3. What about data ingestion using AI like RAG?

\*\*Answer:\*\*  

I’ve worked with RAG-style data ingestion pipelines. This included parsing and cleaning documents, chunking content, generating embeddings, and storing them in vector stores like FAISS or OpenSearch. I focused on ingestion reliability, metadata tagging, access control, and integrating retrieval layers into AI agents and backend services.



---



\## 4. Any LangGraph experience?

\*\*Answer:\*\*  

Yes. I’ve used LangGraph to design stateful, multi-step AI agent workflows. It helped define deterministic flows for tasks like intent detection, retrieval, tool execution, validation, and response generation. My focus was on state management, error handling, and production readiness.



---



\## 5. What is your experience in CI/CD and training?

\*\*Answer:\*\*  

CI/CD is a core part of my role. I’ve designed and maintained pipelines using GitHub Actions, GitLab CI, and Jenkins. These pipelines cover builds, tests, security scans, and deployments. I’ve also trained and mentored engineers on CI/CD best practices, pipeline debugging, and safe release strategies.



---



\## 6. From a hands-on perspective, did you design and maintain pipelines yourself?

\*\*Answer:\*\*  

Yes. I’ve personally created CI/CD pipelines end to end—writing configurations, defining stages, managing secrets, environment promotion, and implementing rolling or blue-green deployments. I’ve also optimized build performance and resolved pipeline failures.



---



\## 7. What about ETL and ELT systems?

\*\*Answer:\*\*  

I’ve worked with both ETL and ELT systems. For ETL, I built Python pipelines that extracted data from APIs and databases, transformed it through validation and enrichment, and loaded it into downstream systems. For ELT, I designed ingestion into data lakes or warehouses and supported downstream transformations. I focused on data quality, scalability, and observability.



---



\## 8. Any experience with SRE tasks?

\*\*Answer:\*\*  

Yes. I’ve handled SRE responsibilities such as on-call support, incident response, root-cause analysis, and postmortems. I’ve improved reliability through better monitoring, retries, timeouts, health checks, and autoscaling. I consistently owned services in production even without a dedicated SRE title.



---



\## 9. When doing data ingestion, have you used JIRA, GitHub, PagerDuty?

\*\*Answer:\*\*  

Yes. JIRA was used to track ingestion work, incidents, and postmortem follow-ups. GitHub was used for version control, pull requests, code reviews, and CI/CD. PagerDuty handled alerts for ingestion failures and SLA breaches, and I participated in on-call rotations.



---



\## 10. What are some advantages of React?

\*\*Answer:\*\*  

React’s component-based architecture improves reusability and maintainability. Its virtual DOM improves performance, and unidirectional data flow makes state easier to manage. It has a strong ecosystem, excellent TypeScript support, and scales well for large applications.



---



\## 11. What are some advantages of Python versus Go?

\*\*Answer:\*\*  

Python excels in rapid development, data processing, ETL, and AI/ML due to its rich ecosystem. Go excels in performance, concurrency, and operational simplicity, making it ideal for high-throughput, low-latency services. I often use Python for data-heavy workloads and Go for performance-critical services.



---



\## 12. Can you give an example of a failure and how you fixed it?

\*\*Answer:\*\*  

I once designed a data ingestion pipeline that worked functionally but failed under peak load due to poor handling of upstream variability. After recognizing the issue, I redesigned it with batching, backpressure, improved retries, and stronger monitoring. The system became stable, and I documented the lessons learned to avoid repeating the mistake.



---



\## 13. Do you have any questions for me?

\*\*Answer:\*\*  

No questions at this time. Thank you for the opportunity and the discussion.



---



\## 14. Python Code Challenge – Proper Substring Check



\*\*Question:\*\*  

Write a Python program to check whether the \*\*(n-1)th string\*\* is a \*\*proper substring\*\* of the \*\*nth string\*\* in a given list of strings.



A proper substring means:

\- The second last string exists inside the last string

\- The two strings are not exactly equal



---



\### Example Inputs and Outputs



\*\*Input:\*\*

```python

\['a', 'abb', 'sfs', 'oo', 'de', 'sfde']

````



\*\*Output:\*\*



```

True

```



\*\*Input:\*\*



```python

\['a', 'abb', 'sfs', 'oo', 'ee', 'sfde']

```



\*\*Output:\*\*



```

False

```



\*\*Input:\*\*



```python

\['a', 'abb', 'sad', 'ooaaesdfe', 'sfsdfde', 'sfsd', 'sfsdf', 'qwrew']

```



\*\*Output:\*\*



```

False

```



\*\*Input:\*\*



```python

\['a', 'abb', 'sad', 'ooaaesdfe', 'sfsdfde', 'sfsd', 'sfsdf', 'qwsfsdfrew']

```



\*\*Output:\*\*



```

True

```



---



\### Answer (Python Solution)



```python

def check\_proper\_substring(arr):

&nbsp;   if len(arr) < 2:

&nbsp;       return False



&nbsp;   second\_last = arr\[-2]

&nbsp;   last = arr\[-1]



&nbsp;   return second\_last in last and second\_last != last





arr = eval(input())

print(check\_proper\_substring(arr))

```



\*\*Explanation:\*\*



\* Ensure the list has at least two elements

\* Compare the second last and last strings

\* Check for substring presence while ensuring they are not equal



\*\*Time Complexity:\*\* `O(n)` (substring check)

\*\*Space Complexity:\*\* `O(1)`



```

```



