# GenAI / ML Interview Questions and Answers

## 1. Give a brief introduction about yourself.
I have over 10 years of experience working in data-intensive environments using Python, AWS, and SQL. My work mainly focuses on building scalable backend systems, distributed data pipelines, and AI-driven applications. I have designed cloud-native architectures using services such as Lambda, S3, Step Functions, and container platforms like Kubernetes. Recently my work has been focused on building AI systems including document intelligence platforms, RAG-based systems, and machine learning models for analytics and fraud detection. I also have experience integrating OpenAI APIs, building APIs using Python frameworks, and collaborating with data engineering and frontend teams using tools like React and Tableau.

---

## Project and System Design

### 2. Can you walk me through one project you owned end-to-end?
One project I owned was an AI-powered document intelligence platform. The goal was to process large volumes of enterprise documents and extract structured insights. Documents were uploaded into cloud storage such as S3. Once uploaded, the ingestion pipeline triggered processing services written in Python. The documents were parsed, cleaned, and structured. AI models were used to extract summaries, entities, and classifications. The structured output was stored in a database and indexed into OpenSearch so users could perform fast search and analytics. I was responsible for the system architecture, pipeline development, API development, CI/CD pipelines, and production deployment.

---

### 3. You mentioned processing 4–6 TB of data daily. Can you explain that pipeline?
The pipeline started with ingestion from multiple healthcare systems including electronic health records and claim systems. Data was ingested into a data lake stored in S3. From there we used distributed processing frameworks like Apache Spark to process the data. Spark jobs performed tasks such as validation, schema normalization, deduplication, and enrichment. Once processed, the data was stored in optimized formats like Parquet so it could be efficiently queried. The curated datasets were then used by analytics dashboards and machine learning models.

---

## Performance and Architecture

### 4. How did you achieve sub-second API response time?
To achieve sub-second latency we separated offline processing from online inference. Feature engineering and heavy computations were done earlier in the pipeline. The trained model was loaded into memory when the microservice started so it didn’t need to load during every request. When an API request arrived, the service simply retrieved precomputed features and executed inference using the in-memory model. This allowed the system to return predictions in a few hundred milliseconds.

---

## Fraud Detection Model

### 5. You claimed a 22% improvement in precision. How did you calculate it?
We compared the new model against the existing baseline using historical labeled data. For example, if the previous system had a precision of 63% and the new model achieved 77%, the improvement is calculated as relative improvement between those values. The improvement came from adding new behavioral features, improving feature engineering, and tuning the model.

### 6. Did you expand the training dataset?
Yes. Fraud datasets are usually highly imbalanced. The majority of records represent legitimate transactions while fraud cases are rare. We expanded the dataset by including additional historical data and used balancing techniques such as oversampling the minority class and undersampling the majority class.

### 7. Did you apply normalization during preprocessing?
Yes. Numeric features were normalized or standardized so they were on the same scale. Categorical variables were encoded using techniques like one-hot encoding or frequency encoding. We also handled missing values and removed outliers during preprocessing.

### 8. Was this a classification model like logistic regression?
Yes. Fraud detection is a binary classification problem where the outcome is either fraud or non-fraud. Logistic regression was used initially as a baseline model because it is simple and interpretable. Later we experimented with tree-based models like Random Forest and Gradient Boosting which performed better at capturing complex patterns.

---

## RAG / Generative AI

### 9. Explain how documents move from ingestion to retrieval to final response generation.
First documents are ingested into the system from sources such as PDFs, reports, or knowledge bases. During ingestion, the documents are parsed and split into smaller chunks. Each chunk is converted into an embedding vector using an embedding model. These vectors are stored in a vector database. When a user asks a question, the system converts the question into an embedding. A similarity search retrieves the most relevant document chunks from the vector database. Those retrieved chunks are passed along with the user query to the language model which generates the final response.

### 10. Why do we need to chunk documents?
Chunking improves retrieval accuracy. If a whole document is stored as one embedding, the vector represents multiple topics and retrieval becomes less precise. By splitting documents into smaller chunks, the system can retrieve only the specific section that contains the relevant information.

### 11. What is a vector?
A vector is a list of numbers representing data in mathematical space. Embedding models convert text into vectors so that texts with similar meanings are placed close together in vector space. This allows systems to perform semantic similarity search.

### 12. How do you decide chunk size and embedding model?
Chunk size is selected by balancing context and retrieval precision. Typical chunk sizes range between 300 and 800 tokens. Embedding models are chosen based on semantic quality, latency, cost, and vector dimension size. We evaluate different embeddings using retrieval benchmarks.

### 13. Do you use overlap when chunking documents?
Yes. Overlap is used to ensure context is preserved when sentences span across chunk boundaries. Usually we use around 10-20% overlap between chunks.

---

## Hallucination and Retrieval

### 14. What challenges did you face with hallucination and irrelevant retrieval?
The biggest challenge was ensuring the model stayed grounded in the retrieved documents. Sometimes the model generated information that was not present in the source documents. We mitigated this by designing prompts that instructed the model to only answer using retrieved context and return “insufficient information” if the answer was not present.

---

## Deployment

### 15. How do you deploy ML models to production using Kubernetes or AKS?
The trained model is packaged into a Docker container with all dependencies. The container image is pushed to a container registry. CI/CD pipelines automate testing and deployment. Kubernetes deploys the container as pods and manages scaling, load balancing, and health checks. Monitoring tools track performance and system health.

---

## Scaling Vector Databases

### 16. Did you face performance issues when the vector database grew large?
Yes. As the vector database grows, similarity search can become slower. To address this we used approximate nearest neighbor indexing methods such as HNSW. We also used metadata filtering to narrow the search space and distributed the vector index across multiple nodes.

---

## Evaluation

### 17. How did you evaluate whether RAG retrieval was working well?
We created a benchmark dataset consisting of queries and known relevant documents. We measured retrieval performance using metrics such as Recall@K and Precision@K. We also performed manual evaluation to ensure retrieved documents were relevant.

### 18. Did you compare different embedding models?
Yes. We evaluated different embedding models by running the same set of queries and comparing retrieval results. We measured performance using metrics like Recall@K and Mean Reciprocal Rank while also considering latency and cost.

---

## GenAI System Challenges

### 19. What was the hardest problem you faced while building your first GenAI system?
The hardest problem was ensuring reliable retrieval from large document collections. If the retrieval system fails to return relevant information, the language model can generate hallucinated responses. We addressed this by optimizing chunking strategies, evaluating different embedding models, improving prompts, and implementing scalable vector search infrastructure.
