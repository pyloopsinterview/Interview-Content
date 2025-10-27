# Microservices, Kafka, React & Node.js Q&A

## 1. Investigating slow screen-boot in production

**Q:** You may notice that a new screen-boot application takes a long time to start in the production environment. How would we investigate the results of this type of screen-boot?

**A:** Steps to investigate:

1. **Identify the nature of the slowdown**: Determine if the delay is before the first screen loads or during interaction.
2. **Review system and application logs**: Check timestamps for initialization, database connections, and resource loading.
3. **Check environment and resource usage**: Monitor CPU, memory, network, and I/O usage.
4. **Check database or integration latency**: Optimize queries, connection pools, and API call timing.
5. **Compare configurations** between environments to isolate differences.
6. **Profile or trace startup sequence** using APM tools or custom timers.
7. **Document and compare results** to identify the slowest components.
8. **Take corrective actions**: Optimize caching, lazy loading, or background processing, and scale resources if needed.

---

## 2. Facebook growth explanation

**Q:** Because Facebook which registered a was in the lower environment but becomes the noticeable store among the moderate or higher-paying producers.

**A:** Rephrased interpretations:

1. **Growth/Performance**: “Facebook, which initially operated in a smaller market, later became one of the most prominent and profitable platforms.”
2. **Environment tiers**: “Facebook was first set up in a lower environment for testing, but later became widely used in production.”
3. **Business evolution**: “Although Facebook started small, it quickly grew to become one of the top-performing and high-revenue companies.”

---

## 3. Optimizing API performance

**Q:** How to optimize the performance of an API?

**A:** Key steps:

1. **Measure performance first**: Track response times, throughput, and error rates.
2. **Optimize code**: Reduce loops, use async I/O, efficient data structures, batch processing.
3. **Database optimization**: Indexing, query optimization, caching, connection pooling, avoid N+1 queries.
4. **External dependency optimization**: Parallelize calls, use retries, caching.
5. **Caching**: In-memory, distributed (Redis/Memcached), HTTP caching.
6. **Reduce payload**: Pagination, selective fields, compression.
7. **Infrastructure**: Load balancing, horizontal scaling, keep-alive connections, CDNs.
8. **Profiling and monitoring**: Continuously measure and adjust.
9. **Rate limiting**: Protect APIs from overload.

---

## 4. React app performance degradation

**Q:** The React application works well in its area. Users report slowness and submission issues after continuous use.

**A:** Investigation and fixes:

1. **Memory leaks**: Clean up timers, intervals, subscriptions in `useEffect`.
2. **Excessive re-renders**: Use `React.memo`, `useMemo`, `useCallback`, virtualized lists.
3. **Network requests**: Abort unnecessary calls, avoid duplicates.
4. **Large DOM**: Profile with React DevTools, break components into smaller ones.
5. **Submission issues**: Ensure proper error handling, reset `isSubmitting` state.
6. **Monitoring**: Use DevTools Performance tab and React Profiler.

---

## 5. Polyfills for normalization

**Q:** We have to use polyfills for normalization.

**A:**

- **Polyfills** allow consistent behavior across browsers.
- Common polyfills:
  1. **core-js / regenerator-runtime** for ES6+ features and async/await
  2. **whatwg-fetch** for `fetch()` support
  3. **AbortController / URL polyfills**
  4. **Intl** for date, currency formatting
- Use Babel with `useBuiltIns: "entry"` for selective polyfills.

---

## 6. Graceful Node.js crash handling

**Q:** If a Node app crashes in production due to an exception, how to handle gracefully?

**A:** Steps:

1. **Global error handlers**:

```js
process.on('uncaughtException', (err) => { ... });
process.on('unhandledRejection', (reason) => { ... });
```

2. **Graceful shutdown**: Close DB, servers, and clean resources.
3. **Central error middleware** in Express to catch errors.
4. **Process manager** (PM2, Docker) to auto-restart.
5. **Structured logging & monitoring**: Winston, Sentry.
6. **Prevent common crashes**: Validate inputs, handle promises, isolate services.

---

## 7. Two microservices sharing a database

**Q:** Two microservices are directly accessing the same database schema. What concerns arise and how to address this?

**A:**  
**Concerns:**

- Tight coupling
- Loss of data ownership
- Deployment risks
- Data inconsistency
- Security concerns

**Solutions:**

1. **Each service owns its own DB/schema**
2. Communicate via **APIs or events**
3. Remove direct DB access from non-owning service
4. Optionally use **read-only replicas** or event-driven synchronization
5. Enforce access boundaries at infra level

---

## 8. Kafka consumer duplicates

**Q:** Server consuming Kafka messages occasionally inserts duplicates into DB. How to investigate and prevent?

**A:**  
**Investigation:**

- Check Kafka **offset commits**
- Trace **message keys**
- Check **producer retries** and consumer crashes
- Look for **parallel consumers** or rebalances

**Prevention:**

1. **Idempotent consumer**: Use unique keys or `ON CONFLICT DO NOTHING`
2. **Kafka exactly-once semantics** (EOS) with transactional producers
3. **Deduplication** via cache or table of processed IDs
4. **Commit offsets after DB transaction**
5. **Unique constraints in DB**

---

## 9. Kafka broker crash during high traffic

**Q:** During high traffic, Kafka broker bursts down. How does Kafka handle this?

**A:**

1. **Broker failure detected** by controller/ZooKeeper or KRaft.
2. **Leader election** for affected partitions from in-sync replicas (ISR).
3. Producers/consumers auto-reconnect to new leaders.
4. **Replication recovery**: Broker catches up and rejoins ISR.

**Impact during high traffic:**

- Temporary partition unavailability
- Producer retries
- Consumer lag spikes
- Replication backlog

**Resilience mechanisms:**

- Partition replication
- Leader election
- Idempotent producers
- ISR management
- Controller failover
- Client metadata refresh

---

## 10. Create a generic class in Java that can hold a pair of objects of any types. Implement methods to get and set the values of the pair, and demonstrate its usage with different types.

// Generic Pair class
public class Pair<T, U> {
private T first;
private U second;

    public Pair(T first, U second) {
        this.first = first;
        this.second = second;
    }

    public T getFirst() { return first; }
    public void setFirst(T first) { this.first = first; }

    public U getSecond() { return second; }
    public void setSecond(U second) { this.second = second; }

    @Override
    public String toString() {
        return "(" + first + ", " + second + ")";
    }

    public static void main(String[] args) {
        Pair<Integer, String> pair1 = new Pair<>(1, "One");
        Pair<String, Double> pair2 = new Pair<>("Pi", 3.14);

        System.out.println(pair1);
        System.out.println(pair2);
    }

}

```

```
