# Dynatrace Interview Questions & Answers

## 1. Brief me about your current role and responsibilities.

**Answer:**
Currently, I’m working as a **Lead Cloud DevOps Engineer** at **Kiewit**, mainly focused on **Dynatrace Engineering**, **Observability**, and **Platform Monitoring**.

My day-to-day responsibilities include:

* **Dynatrace administration**
* **OneAgent deployment**
* **Dashboard creation**
* **Alert configuration**
* **Distributed tracing**
* **RUM monitoring**
* **Kubernetes monitoring**
* **Log analysis**
* **Management Zones**
* **RBAC configuration**
* **Monitoring-as-Code automation**

I also work on:

* **Problem investigation**
* **Root cause analysis using Davis AI**
* **ServiceNow integration**
* **CI/CD monitoring automation**
* **Production incident troubleshooting**

---

## 2. How many years of experience do you have with Dynatrace?

**Answer:**
I have around **4 to 5 years of hands-on experience** with **Dynatrace**.

My experience includes:

* **Dynatrace Administration**
* **OneAgent deployment**
* **Distributed Tracing**
* **RUM Monitoring**
* **Synthetic Monitoring**
* **DQL Queries**
* **Dashboards & Alerting**
* **Management Zones**
* **RBAC & Governance**
* **ServiceNow Integration**
* **Monitoring-as-Code Automation**

---

## 3. Have you used the Dynatrace interface?

**Answer:**
Yes, I use the **Dynatrace interface** daily.

Mostly I work with:

* **Dashboards**
* **Problems & Alerts**
* **Service Flow**
* **Distributed Tracing**
* **Log Analytics**
* **Infrastructure Monitoring**
* **Kubernetes Monitoring**
* **Synthetic Monitoring**
* **Management Zones**

I use it mainly for:

* **Production monitoring**
* **Troubleshooting**
* **Root cause analysis**
* **Performance optimization**

---

## 4. How does Dynatrace automatically discover services and dependencies?

**Answer:**
Dynatrace uses **OneAgent** and **automatic instrumentation**.

Once installed, OneAgent automatically detects:

* **Applications**
* **Processes**
* **Services**
* **Containers**
* **Databases**
* **APIs**
* **Network communication**

Using **PurePath Distributed Tracing**, Dynatrace automatically maps:

* **Service dependencies**
* **Request flows**
* **Database calls**
* **External API communication**

This helps generate real-time **topology maps** and **service flow visualization**.

---

## 5. How would you monitor .NET and Java applications on the same host?

**Answer:**
A single **OneAgent** installed on the host can monitor both applications separately.

Dynatrace automatically identifies:

* **Java JVM processes**
* **.NET CLR processes**
* **Associated services and APIs**

For Java:

* **Heap memory**
* **GC metrics**
* **Thread analysis**
* **Method tracing**

For .NET:

* **CLR metrics**
* **Exception tracking**
* **Request tracing**
* **IIS monitoring**

We can separate monitoring using:

* **Management Zones**
* **Tagging**
* **Process group rules**

---

## 6. What is Davis AI in Dynatrace?

**Answer:**
**Davis AI** is Dynatrace’s built-in **AI engine**.

It helps with:

* **Root cause analysis**
* **Problem correlation**
* **Anomaly detection**
* **Dependency analysis**
* **Noise reduction**
* **Smart alerting**

It automatically analyzes:

* **Logs**
* **Metrics**
* **Events**
* **Traces**
* **Infrastructure telemetry**

and identifies the actual root cause of issues.

---

## 7. What are Generative AI, Predictive AI, and Causal AI in Dynatrace?

**Answer:**

### Causal AI

Used for:

* **Root cause analysis**
* **Dependency understanding**
* **Problem correlation**

### Predictive AI

Used for:

* **Capacity forecasting**
* **Performance trend prediction**
* **Resource saturation prediction**

### Generative AI

Used for:

* **Natural language investigations**
* **Problem summarization**
* **DQL assistance**
* **Dashboard recommendations**
* **Log analysis assistance**

---

## 8. Do we need a separate agent for Generative AI?

**Answer:**
No, generally **no separate agent installation** is required.

The existing **OneAgent** collects telemetry data.

For Generative AI:

* **Feature enablement** may be required
* Sometimes a **tenant-level flag** is enabled
* Proper **licensing and permissions** are needed

---

## 9. What are Management Zones?

**Answer:**
**Management Zones** are logical partitions in Dynatrace.

They help organize monitoring data based on:

* **Applications**
* **Teams**
* **Environments**
* **Business units**

They are used for:

* **Access control**
* **Dashboard filtering**
* **Alert segregation**
* **Team-specific visibility**

---

## 10. What if OneAgent cannot be installed?

**Answer:**
If OneAgent installation is restricted, we can use:

* **OpenTelemetry integrations**
* **API-based ingestion**
* **Remote extensions**
* **Cloud integrations**
* **Log forwarding**
* **Custom metrics ingestion**

This helps monitor:

* **Logs**
* **Metrics**
* **Traces**
* **Infrastructure telemetry**

without direct OneAgent installation.

---

## 11. DQL query to fetch ERROR logs from last 24 hours.

```sql
fetch logs
| filter loglevel == "ERROR"
| filter timestamp >= now() - 24h
| sort timestamp desc
```

### Explanation:

* **fetch logs** → Retrieves logs
* **filter loglevel** → Filters ERROR logs
* **timestamp >= now() - 24h** → Last 24 hours logs
* **sort timestamp desc** → Latest logs first

---

## 12. Parse employeeId from JSON logs.

```sql
fetch logs
| fieldsAdd parsed = parseJson(content)
| fields employeeId = parsed.employeeId
| fields timestamp, employeeId
```

### Explanation:

* **parseJson(content)** → Parses JSON payload
* **fieldsAdd** → Creates a new derived field
* **parsed.employeeId** → Extracts employee ID
* **fields** → Displays selected columns

---

## 13. Difference between fields and fieldsAdd.

### fields

Used to:

* Display/select columns
* Similar to SQL SELECT

Example:

```sql
| fields timestamp, content
```

### fieldsAdd

Used to:

* Create a new calculated column
* Add derived values

Example:

```sql
| fieldsAdd parsed = parseJson(content)
```

---

## 14. What is aggregate in DQL?

**Answer:**
`aggregate` is used for:

* **Grouping data**
* **Summarizing logs**
* **Calculations**

Example:

```sql
fetch logs
| filter loglevel == "ERROR"
| aggregate errorCount = count(), by:{dt.entity.service}
```

This counts ERROR logs grouped by service.

---

## 15. Difference between filter and aggregate.

### filter

Used to restrict data.

Example:

```sql
| filter loglevel == "ERROR"
```

Similar to SQL WHERE clause.

### aggregate

Used for:

* Grouping
* Summarization
* Calculations

Example:

```sql
| aggregate errorCount = count(), by:{dt.entity.service}
```

Similar to SQL GROUP BY.

---

## 16. Have you created workflows in Dynatrace?

**Answer:**
Yes, I have worked on **Dynatrace Workflows** for:

* **Event-driven automation**
* **Custom workflow creation**
* **Workflow triggers**
* **Conditional execution**
* **Automation tasks**

Examples include:

* **Kubernetes pod failure workflows**
* **Metric threshold-based workflows**
* **Custom event triggers**
* **Deployment monitoring workflows**

Workflow components include:

* **Triggers**
* **Conditions**
* **Tasks**
* **API actions**
* **Automation steps**

---

## 17. Difference between Merge and Rebase in Git.

### Merge

* Combines branches
* Creates merge commit
* Preserves history

Example:

```bash
git merge feature-branch
```

### Rebase

* Rewrites commit history
* Creates linear history
* No merge commit

Example:

```bash
git rebase main
```

### Usage:

* **Merge** → Shared branches
* **Rebase** → Clean feature branch history
