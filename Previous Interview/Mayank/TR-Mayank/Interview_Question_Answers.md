Below is a **complete Markdown (`.md`)–ready document** containing **all the exact questions you asked today**, **with the corresponding coding answers included**.
You can **copy-paste this directly into a `.md` file** and use it for **interview revision or submission**.

---

````md
# Backend & MongoDB Interview – Questions with Coding Answers

---

## 1. What is a transaction in MongoDB?

**Answer:**
A MongoDB transaction allows multiple read and write operations across documents, collections, or databases to execute atomically. Either all operations succeed or all are rolled back.

```js
session.startTransaction()
db.orders.insertOne(order, { session })
db.trades.insertOne(trade, { session })
session.commitTransaction()
````

---

## 2. If I want to test MongoDB queries online, how can I do that?

**Answer:**
Use MongoDB Atlas Playground, MongoDB Compass, or online MongoDB playgrounds to test queries without a local setup.

---

## 3. How do you route reads to secondary nodes in MongoDB?

**Answer:**
Using read preferences configured at the client or query level.

```js
db.collection.find().readPref("secondary")
```

---

## 4. What is read concern and write concern?

**Answer:**

* Read concern controls data consistency visibility.
* Write concern controls how many nodes must acknowledge a write.

```js
db.collection.insertOne(doc, { writeConcern: { w: "majority" } })
```

---

## 5. When should you use a sharded cluster?

**Answer:**
When data exceeds a few TBs, write throughput is high, or when scaling and fast recovery are required.

---

## 6. How do you choose a shard key?

**Answer:**
A shard key should:

* Have high cardinality
* Be used in most queries
* Not be monotonically increasing

---

## 7. Why is `_id` a bad shard key?

**Answer:**
Because it is monotonically increasing, causing all writes to go to one shard.

---

## 8. What is the ESR rule for MongoDB indexes?

**Answer:**
Indexes should follow:

1. Equality
2. Sort
3. Range

```js
db.trades.createIndex({ symbol: 1, createdAt: -1 })
```

---

## 9. Why does equality come before range in indexes?

**Answer:**
Equality filters narrow down data first, avoiding expensive range scans and in-memory sorting.

---

## 10. How do you decide between embedding and referencing?

**Answer:**

* Embed when data is frequently accessed together.
* Reference when data is large or frequently updated.

---

## 11. How do you prevent duplicate trades on retries?

**Answer:**
Using idempotency with unique indexes.

```js
db.trades.createIndex({ orderId: 1, sequence: 1 }, { unique: true })
```

```python
db.trades.update_one(
    {"orderId": order_id, "sequence": seq},
    {"$setOnInsert": trade},
    upsert=True
)
```

---

## 12. How do you paginate large datasets efficiently?

**Answer:**
Using cursor-based pagination.

```python
db.trades.find(
    {"_id": {"$lt": ObjectId(cursor)}}
).sort("_id", -1).limit(50)
```

---

## 13. Pros and cons of cursor-based pagination?

**Answer:**
**Pros:** Stable, scalable, efficient
**Cons:** Cannot jump to arbitrary pages

---

## 14. How do you design a REST API for pagination and filtering?

**Answer:**
Use query parameters and return cursors.

```json
{
  "data": [...],
  "pagination": { "nextCursor": "abc123" }
}
```

---

## 15. Query to get Apple trades with price ≤ 150

```js
db.trades.find({
  symbol: "AAPL",
  price: { $lte: 150 }
})
```

---

## 16. How do you count trades by product and date?

```js
db.trades.aggregate([
  {
    $group: {
      _id: {
        symbol: "$symbol",
        date: { $dateToString: { format: "%Y-%m-%d", date: "$createdAt" } }
      },
      count: { $sum: 1 }
    }
  }
])
```

---

## 17. How do you get top N traded products?

```js
db.trades.aggregate([
  { $group: { _id: "$symbol", count: { $sum: 1 } } },
  { $sort: { count: -1 } },
  { $limit: 2 }
])
```

---

## 18. How is the count calculated in aggregation?

**Answer:**
MongoDB increments one per document using `$sum: 1`.

---

## 19. Can this be done in Python? What’s the complexity?

```python
from collections import Counter

def top_n_products(trades, n=2):
    return Counter(t["symbol"] for t in trades).most_common(n)
```

**Complexity:** O(N)

---

## 20. Does Python internally sort for top-N?

**Answer:**
Yes. Python uses Timsort (`O(n log n)`) for sorting operations.

---

## 21. Time complexity of merge sort?

**Answer:**
Best, average, worst case: **O(n log n)**

---

## 22. How do you handle tables in backend APIs?

**Answer:**
APIs return structured data; tables are rendered on the frontend.

---

## 23. How do you return table-friendly data?

```json
{
  "columns": ["id", "symbol", "price"],
  "rows": [...]
}
```

---

## 24. How do you convert MongoDB results into a DataFrame?

```python
df = pd.DataFrame(list(db.trades.find()))
```

---

## 25. How do you add a prefix to all IDs in a DataFrame?

```python
df["id"] = "ABC_" + df["id"].astype(str)
```

---

## 26. What frontend components are used for tables?

**Answer:**
React with MUI DataGrid, Ant Design Table, or AG Grid.

---

## 27. What format should a REST API return for tables?

**Answer:**
Structured JSON; tables are rendered by the frontend.

---

# Final One-Line Summary

> I design scalable MongoDB-backed APIs with cursor pagination, idempotent writes, efficient aggregation, and table-ready responses rendered by frontend components.

---

```

---

If you want next, I can:
- Convert this into a **PDF**
- Split into **short/long interview answers**
- Create a **mock interview Q&A**
- Review it as an **interviewer**

Just tell me.
```
