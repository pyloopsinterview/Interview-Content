## Q1. read json file into python function insert into sql.

Ans. Got it ✅ You want to **read a JSON file in Python** and then **insert its data into an SQL table**.

Suppose you have a JSON file called `data.json`:
```
[
  {"id": 1, "name": "Alice", "age": 28},
  {"id": 2, "name": "Bob", "age": 32},
  {"id": 3, "name": "Charlie", "age": 25}
]

```


using `sqlite3`

```
import json
import sqlite3

def insert_json_to_db(json_file, db_file="mydatabase.db"):
    # Step 1: Read JSON file
    with open(json_file, "r") as f:
        data = json.load(f)

    # Step 2: Connect to SQL database (SQLite used here)
    conn = sqlite3.connect(db_file)
    cursor = conn.cursor()

    # Step 3: Create table if not exists
    cursor.execute("""
        CREATE TABLE IF NOT EXISTS users (
            id INTEGER PRIMARY KEY,
            name TEXT,
            age INTEGER
        )
    """)

    # Step 4: Insert JSON records into SQL
    for record in data:
        cursor.execute("""
            INSERT INTO users (id, name, age) VALUES (?, ?, ?)
        """, (record["id"], record["name"], record["age"]))

    # Step 5: Commit & close
    conn.commit()
    conn.close()

# Run function
insert_json_to_db("data.json")

```

Explanation

1. `json.load(f)` → loads JSON file into a Python list/dict.
    
2. `sqlite3.connect()` → connects to SQLite DB (or use `pyodbc` / `psycopg2` for MSSQL/Postgres).
    
3. Loop through JSON data and insert into SQL using parameterized query (`?`).
    
4. Commit changes and close connection.

## Q2. Do we need pysql ?

Ans. For SQLite, no external driver is required since Python ships with `sqlite3`. But for MySQL or PostgreSQL, yes, we need an external library like `PyMySQL` or `psycopg2` to establish the database connection.

## Q3. How to handle millions of transitions in python.

Ans. If I have to handle millions of transactions in Python, I would avoid loading everything into memory at once. Instead, I’d stream the data using libraries like `ijson`. I’d insert records in batches with `executemany` or use database-specific bulk loaders like `COPY` in Postgres or `LOAD DATA INFILE` in MySQL. I’d also wrap inserts in a single transaction to reduce commit overhead. For very large datasets, I’d parallelize the processing and tune the batch size for optimal performance.

## Q4. So let's assume you have a CSV file, okay? So if I ask you to read it using Python, right? So, how do you write that code actually? Can you help me write the code?

Ans. 
simple version (using csv module)
```
import csv

with open("data.csv", "r") as file:
    reader = csv.reader(file)
    for row in reader:
        print(row)

```

- Opens `data.csv` in **read mode**.
- `csv.reader` parses rows into lists.
- Iterates and prints each row. 
Professional Version (using `pandas`, preferred in interviews)
```
import pandas as pd

# Read CSV file into DataFrame
df = pd.read_csv("data.csv")

# Print the first 5 rows
print(df.head())

```

- - `pandas.read_csv` loads the file into a **DataFrame**.
- `df.head()` shows the first 5 rows.

There are two common ways. The built-in way is using the `csv` module: open the file, create a `csv.reader`, and loop through rows. The professional way is using Pandas, which is optimized for tabular data. With Pandas, I simply do `import pandas as pd` and then `df = pd.read_csv("data.csv")`. That gives me a DataFrame where I can query, filter, and analyze the data easily.

## Q5. print row wise data using pandaas.

Ans. 
```
import pandas as pd

# Read CSV into DataFrame
df = pd.read_csv("data.csv")

# Iterate row by row
for index, row in df.iterrows():
    print(f"Row {index}: {row.to_dict()}")
```
Explanation (for interview)

- `pd.read_csv("data.csv")` → loads the CSV file into a Pandas DataFrame.
    
- `df.iterrows()` → returns each row as `(index, Series)` pair.
    
- `row.to_dict()` → converts that row into a dictionary for easy printing.
    
- `f"Row {index}: ..."` → prints row number with its data.

Sample Output

If `data.csv` is:

`id,name,age 1,Alice,28 2,Bob,32 3,Charlie,25`

Output will be:

`Row 0: {'id': 1, 'name': 'Alice', 'age': 28} Row 1: {'id': 2, 'name': 'Bob', 'age': 32} Row 2: {'id': 3, 'name': 'Charlie', 'age': 25}`

## Q6. Why Pandas and not csv module?
Ans. Pandas is much faster and more convenient for structured data. It provides `iterrows()` or `itertuples()` to process row by row, and I can also use vectorized operations for efficiency.

## Q7. How you use Airflow in your past project.

Ans. 
In my previous project, I used **Apache Airflow** as the orchestration tool to manage and automate complex data workflows. Our main use case was **ETL pipelines** — extracting data from multiple sources like APIs and CSV files, transforming it, and then loading it into a data warehouse.

I created DAGs (Directed Acyclic Graphs) to represent these workflows. Each task in the DAG corresponded to a specific step, such as calling an API, processing the raw data with Python, and inserting the cleaned data into a SQL database. I scheduled these DAGs to run daily and added retry logic to handle failures.

I also made use of **Airflow operators** like `PythonOperator` for custom Python scripts and `BashOperator` for shell tasks. For data quality, I included checks that validated row counts and schema consistency after each load.

One challenge was handling large volumes of data efficiently. To solve that, I used **parallel tasks** in the DAG, breaking down big jobs into smaller chunks. We also integrated Airflow with Slack to send real-time alerts whenever a task failed, so the team could quickly react.

Overall, Airflow helped us achieve **automation, monitoring, and reliability** in our data pipelines, which significantly reduced manual intervention and improved data freshness for downstream analytics.

## Q8. How you gone improve preformation.
Ans.  
To improve performance, I focus on optimization at three levels: **code, database, and orchestration**.
> 
> At the **code level**, I optimize Python scripts by using vectorized operations with libraries like Pandas or NumPy instead of loops, caching intermediate results, and profiling to remove bottlenecks.
> 
> At the **database level**, I use batch inserts instead of row-by-row, apply proper indexing, and use bulk loaders like `COPY` in PostgreSQL or `LOAD DATA INFILE` in MySQL for handling millions of records efficiently.
> 
> At the **orchestration level**, especially with Airflow, I improve performance by parallelizing tasks in the DAG, tuning concurrency parameters, and breaking large jobs into smaller, independent tasks. I also avoid unnecessary dependencies so tasks can run in parallel instead of sequentially.
> 
> Finally, I monitor performance using logs and metrics, and apply incremental or delta loads instead of full reloads whenever possible. This combination of code optimization, efficient database usage, and smart orchestration significantly improves the end-to-end performance.

---

### 🔑 Quick Interview Points to Mention

- Use **batching / bulk operations** instead of one-by-one.
    
- Use **parallelism** in Airflow DAGs.
    
- Optimize SQL with **indexes & query tuning**.
    
- Use **profiling tools** (cProfile, memory_profiler) for Python bottlenecks.
    
- Replace full loads with **incremental loads**.
    
- Add **caching / message queues** where appropriate.

## Q9. Which database you had used?.

Ans. > 
In my projects, I’ve worked with both **relational and NoSQL databases**, depending on the use case.
> 
> For **transactional and structured data**, I mainly used **MySQL** and **PostgreSQL**. MySQL was used in applications that required high availability and fast reads, while PostgreSQL was our choice when we needed advanced features like JSON support and complex queries.
> 
> For **big data and flexible schema use cases**, I worked with **MongoDB**, where we stored semi-structured JSON-like documents, especially for log data and user activity tracking.
> 
> I also integrated with **SQLite** for lightweight use cases like local storage during development and testing.
> 
> In short, I have hands-on experience with MySQL, PostgreSQL, MongoDB, and SQLite, and I choose the database based on scalability, consistency, and data model requirements.”

---

### 🔑 If they push further, you can add:

- **Why MySQL?** → “Good for OLTP, widely supported, efficient for reads/writes.”
    
- **Why PostgreSQL?** → “Better for analytical queries, JSON support, indexing.”
    
- **Why MongoDB?** → “Schema flexibility, great for JSON and hierarchical data.”
    
- **Why SQLite?** → “Lightweight, no server needed, great for dev/test.”