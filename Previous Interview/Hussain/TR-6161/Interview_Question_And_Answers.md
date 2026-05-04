# GCP Data Engineering Interview Q&A (Detailed Version)

## 1. On-Prem Databases Used for Migration
**Answer:**
In my projects, I have worked with multiple on-prem databases depending on the application domain. The primary databases included Microsoft SQL Server for operational and transactional systems, Oracle for core enterprise and healthcare systems, IBM DB2 for legacy systems, and PostgreSQL for modern applications. Additionally, I also handled file-based systems like CSV and fixed-width files generated from legacy batch processes. These diverse sources required different ingestion strategies and careful schema handling during migration.

---

## 2. Services Used to Migrate Data from Oracle
**Answer:**
For Oracle migration, I used a combination of batch and real-time approaches. For bulk data migration, I extracted data and staged it into GCS, then processed it using Dataproc or Dataflow. For continuous data replication, I used Datastream for CDC (Change Data Capture). Cloud Composer was used for orchestration of workflows. Secure connectivity between on-prem and GCP was established using VPN or Interconnect.

---

## 3. Moving Data from On-Prem to GCS
**Answer:**
To move data from on-prem to GCS, I used multiple approaches based on data size and frequency. For large-scale data transfers, I used Transfer Appliance. For scheduled transfers, I used Storage Transfer Service. For custom pipelines, I used scripts with gsutil to upload extracted files. For real-time or incremental data movement, I used Datastream to continuously capture and stream changes into GCS.

---

## 4. Dataflow Usage
**Answer:**
I have extensively used Dataflow for building scalable data pipelines. It is mainly used for streaming and batch data processing, applying transformations, performing data validation, handling CDC data from Datastream, and loading processed data into BigQuery. Dataflow helps in building fully managed, serverless pipelines.

---

## 5. VPN Setup Components
**Answer:**
While setting up VPN connectivity, I worked on creating a VPC network and subnets, configuring a Cloud VPN Gateway on GCP, and a Customer Gateway on-prem. Then I established a VPN tunnel using IKE protocols and pre-shared keys. I configured Cloud Router for dynamic routing using BGP and set firewall rules to allow required traffic. This ensured secure communication between on-prem and GCP.

---

## 6. Subnet
**Answer:**
A subnet is a logical division of a VPC network with a defined IP range. It allows us to organize resources, isolate workloads, and apply security controls. Each subnet belongs to a specific region and helps in managing traffic and access control efficiently.

---

## 7. Ingress vs Egress
**Answer:**
Ingress refers to incoming traffic into the network, such as data coming from on-prem to GCP. Egress refers to outgoing traffic from the network, such as GCP services calling external APIs. Firewall rules are configured to control both ingress and egress traffic.

---

## 8. Dataproc IP Assignment
**Answer:**
Dataproc clusters get their IP addresses from the subnet they are attached to. When a cluster is created, the master and worker nodes are assigned IPs from the subnet’s CIDR range. This ensures proper network control and connectivity.

---

## 9. Dataproc Errors (Wrong Network)
**Answer:**
If networking is not configured properly, errors can occur such as subnet not found, insufficient IP addresses, connection timeouts, firewall blocking errors, and IAM permission issues. These errors usually indicate problems with network setup, routing, or security configurations.

---

## 10. Credential Storage
**Answer:**
Credentials are securely stored in Google Cloud Secret Manager. They are never hardcoded in the code. At runtime, the application fetches credentials securely using APIs. This ensures security and compliance.

---

## 11. Dataproc DB Connection
**Answer:**
Dataproc jobs fetch credentials from Secret Manager at runtime, then establish a JDBC connection to the database. Proper network connectivity, firewall rules, and IAM permissions are ensured for successful communication.

---

## 12. Dataproc for Migration
**Answer:**
Dataproc is used for migration by running Spark jobs that connect to on-prem databases via JDBC. Data is extracted in parallel, transformed if required, and loaded into GCS or BigQuery.

---

## 13. GCS to BigQuery
**Answer:**
Data is moved from GCS to BigQuery using load jobs, which are efficient and serverless. For transformations, Dataflow pipelines are used. In structured workflows, staging tables are created and transformations are applied using SQL or dbt.

---

## 14. CI/CD Deployment
**Answer:**
We use Git for version control and tools like Jenkins for CI/CD pipelines. Code is promoted from Dev to QA to Prod environments. Configurations are parameterized, and workflows are orchestrated using Cloud Composer.

---

## 15. Dataset & Table Creation
**Answer:**
Datasets are created using Terraform for consistency and automation. Tables are created using BigQuery load jobs, SQL queries, or dbt models depending on the layer.

---

## 16. Terraform Commands
**Answer:**
Terraform commands include terraform init to initialize, terraform plan to preview changes, and terraform apply to create resources.

---

## 17. Destroy Resources
**Answer:**
Resources can be destroyed using terraform destroy. For selective deletion, terraform destroy with target option is used.

---

## 18. Destroy Specific Resource via Code
**Answer:**
To destroy a specific resource, we remove it from the Terraform configuration or use conditional variables. Terraform automatically detects the change and deletes the resource during apply.

---

## 19. Apache Beam Pipeline Explanation
**Answer:**
This pipeline reads streaming data from Pub/Sub, parses JSON messages, assigns timestamps, applies windowing, groups data by event ID, removes duplicates, and outputs the processed data.

---
