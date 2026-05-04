# Interview Questions & Answers (Data Engineer / Python / GCP)

_Source Transcript:_ fileciteturn14file0

---

## 1. Tell me about yourself.
**Answer:**
I have around 11 years of experience in Python backend and data engineering, working on data pipelines, ingestion frameworks, and cloud-based systems.

---

## 2. Describe a situation where you redesigned a data ingestion pipeline.
**Answer:**
I worked on redesigning ingestion pipelines by analyzing current bottlenecks, defining trade-offs, and implementing scalable architecture with better performance and maintainability.

---

## 3. How do you document technical decisions?
**Answer:**
For non-trivial decisions, I document trade-offs, architecture choices, and reasoning so the team can align and maintain clarity.

---

## 4. How would you design or redesign an ingestion framework?
**Answer:**
- Understand requirements and data sources
- Design scalable pipeline architecture
- Add preprocessing if required
- Ensure modular and maintainable design
- Optimize performance and reliability

---

## 5. How would you add preprocessing to an existing pipeline?
**Answer:**
Add preprocessing logic as a separate stage in the pipeline to clean, validate, and transform data before ingestion.

---

## 6. What is OpenTelemetry (OTel)?
**Answer:**
OpenTelemetry is an observability framework used for collecting traces, logs, and metrics to monitor distributed systems.

---

## 7. What kind of data pipelines have you built?
**Answer:**
I have built pipelines for healthcare data such as provider data, along with financial and insurance datasets.

---

## 8. Which cloud platform have you used?
**Answer:**
Primarily GCP, using BigQuery for analytics and data warehousing.

---

## 9. What scale of data have you handled?
**Answer:**
Large-scale datasets, including millions of provider records (2–5 million).

---

## 10. What are Slowly Changing Dimensions (SCD)?
**Answer:**
SCD is a data warehousing concept used to manage changes in data over time, preserving historical data.

---

## 11. How do you move large datasets (e.g., 500M rows) from Oracle to GCP?
**Answer:**
- Use parallel processing
- Use ETL pipelines
- Optimize queries
- Use bulk transfer tools
- Ensure efficient data loading into BigQuery

---

## 12. What is Oracle Data Pump?
**Answer:**
A high-performance utility for bulk data export/import in Oracle databases.

---

## 13. Difference between partitioning and clustering?
**Answer:**
- Partitioning: Divides data into segments
- Clustering: Organizes data physically for efficient querying

---

## 14. Which Python libraries do you use for data engineering?
**Answer:**
Common libraries include Pandas, API libraries, and orchestration tools for pipelines.

---

## 15. How do you transpose a DataFrame in Pandas?
**Answer:**
Using:
`df.T` or `df.transpose()`

---

## 16. What is wrong with incorrect outlier detection logic?
**Answer:**
Incorrect logic may return a boolean mask instead of actual filtered data or use wrong conditions.

---

## 17. How do you detect outliers?
**Answer:**
Using:
- Z-score method
- Interquartile Range (IQR)

---

## 18. Why are you looking for a job change?
**Answer:**
My current project is ending, and I am looking for new challenges and growth opportunities.

---

## 19. Are you open to relocation?
**Answer:**
Yes, but it may take 2–3 months due to family considerations.

---

## 20. What is your current location?
**Answer:**
Alpharetta, Georgia.

---

## 21. Do you require sponsorship?
**Answer:**
No, I am a green card holder.

---

## 22. When would you use Data Pump vs direct connection?
**Answer:**
- Data Pump: Bulk data transfer
- Direct connection: Incremental or real-time data transfer

---

