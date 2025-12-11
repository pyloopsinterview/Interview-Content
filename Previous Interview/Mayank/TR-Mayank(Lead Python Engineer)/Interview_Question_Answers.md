---

# Interview Q&A – Mayank (Lead Python Engineer)

## 1. Migration between MongoDB and SQL — Can you describe in detail what you did?

**Answer:**
I led the full end-to-end migration from MongoDB to SQL. I started by analyzing existing collections, nested JSON structures, array fields, and implicit relationships. Using that analysis, I designed relational schemas with proper indexing, constraints, and table relationships.
I built PySpark-based migration jobs to extract data from MongoDB, flatten nested documents, normalize arrays, fix inconsistent data types, and reshape records into SQL-ready formats.
We implemented incremental migration to avoid downtime and used validation checks to compare counts, data quality, and referential accuracy. After stabilizing loads, we cut over downstream APIs, analytics, and workflows to the SQL layer.

---

## 2. Can you describe some disadvantages of working with microservices?

**Answer:**
Microservices add operational complexity because every service has its own deployment, monitoring, and scaling. Communication happens over the network, introducing latency and risk of cascading failures.
Maintaining data consistency is harder because each service typically owns its own database. Testing becomes more complex, especially end-to-end tests.
Observability must be very strong—distributed tracing, logs, and metrics are essential. Finally, infrastructure costs generally increase due to multiple compute resources, databases, and CI/CD pipelines.

---

## 3. What cloud provider are you most familiar with?

**Answer:**
AWS. I have extensive hands-on experience with EC2, S3, Lambda, API Gateway, CloudWatch, IAM, SQS, SNS, Glue, EMR, Redshift, DynamoDB, ECS, and ECR. I’ve used AWS for microservice deployments, data pipelines, security design, monitoring, and CI/CD automation.

---

## 4. Can you explain a project you worked on involving real-time data ingestion?

**Answer:**
Yes. At Prudential, we built a real-time ingestion pipeline for claim documents and workflow events. Events were published to AWS Kinesis Streams whenever a claim changed, a new document was uploaded, or an OCR process finished.
I built a PySpark Structured Streaming job that consumed these events, normalized schemas, enriched data from MongoDB, performed validation, and routed invalid records to a quarantine S3 bucket.
Clean data was written to MongoDB for low-latency serving and SQL tables for analytics. The pipeline triggered FastAPI microservices for AI workflows, enabling end-to-end processing within seconds.

---

## 5. Give me an example of your real-time ingestion project in Prudential.

**Answer:**
We implemented a real-time claims intelligence system. Claim, document, and OCR events were streamed into AWS Kinesis. PySpark streaming transformed and validated the events, flattened OCR outputs, enriched records, and pushed cleaned data to MongoDB and SQL.
This powered real-time AI classification, entity extraction, and workflow automation. For example, when a new medical record was uploaded, the pipeline ingested it, triggered OCR, sent the output to NLP models, and updated the workflow engine—all in near real time.

---

## 6. What tools are you familiar with for monitoring and alerting?

**Answer:**
AWS CloudWatch for logs, metrics, alarms, dashboards, and tracing via X-Ray.
Prometheus and Grafana for metrics, dashboards, and alert rules.
ELK Stack (Elasticsearch + Kibana) for log aggregation and troubleshooting.
Datadog for APM, service maps, container metrics, and alerting.
Also Spark History Server and EMR logs for pipeline monitoring.

---

