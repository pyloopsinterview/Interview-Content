# Node.js Interview Questions & Answers

---

## Section 1: Basics

### Q1. What is Node.js and how is it different from traditional web servers?  
**Ans:** Node.js is a JavaScript runtime built on Chrome’s V8 engine. Unlike traditional servers that create a new thread per request, Node.js is single-threaded and event-driven, making it lightweight and efficient for handling many concurrent connections.

---

### Q2. Why is Node.js single-threaded, and how does it handle concurrency?  
**Ans:** Node.js uses a single-threaded event loop to handle requests asynchronously. It delegates I/O operations to the OS or worker threads, allowing it to handle many requests concurrently without blocking.

---

### Q3. Explain the event loop in Node.js.  
**Ans:** The event loop is a mechanism that allows Node.js to perform non-blocking I/O. It continuously checks the call stack and callback queue, executing callbacks as they become available, enabling asynchronous execution in a single-threaded environment.

---

### Q4. What are callbacks in Node.js? What problems do they cause?  
**Ans:** Callbacks are functions passed as arguments to be executed after an asynchronous operation completes. Excessive nesting of callbacks can lead to “callback hell,” making code hard to read and maintain.

---

### Q5. Difference between setImmediate(), process.nextTick(), and setTimeout().  
**Ans:**  
- `process.nextTick()`: Executes callbacks **before the next event loop iteration**.  
- `setImmediate()`: Executes callbacks **after the current poll phase**.  
- `setTimeout(fn, 0)`: Schedules callbacks to run **after at least 0ms**, in the timer phase.  

---

### Q6. What are Streams in Node.js? Types of streams?  
**Ans:** Streams allow reading or writing data piece by piece instead of all at once. Types:  
- **Readable**: For reading data (e.g., fs.createReadStream)  
- **Writable**: For writing data (e.g., fs.createWriteStream)  
- **Duplex**: Can read and write (e.g., net.Socket)  
- **Transform**: Modifies data while reading/writing (e.g., zlib streams)  

---

### Q7. Explain the concept of middleware in Node.js.  
**Ans:** Middleware is a function that has access to request, response, and next in the request-response cycle. It’s commonly used in frameworks like Express for logging, authentication, or modifying requests.

---

### Q8. Difference between synchronous and asynchronous functions in Node.js.  
**Ans:**  
- **Synchronous**: Blocks the thread until completion (e.g., fs.readFileSync).  
- **Asynchronous**: Non-blocking, allows other operations to continue while waiting for completion (e.g., fs.readFile with callback).

---

### Q9. What is require() in Node.js and how does module caching work?  
**Ans:** `require()` imports modules. Node.js caches modules after the first load, so subsequent `require()` calls return the cached version, improving performance.

---

### Q10. Explain CommonJS vs ES Modules in Node.js.  
**Ans:**  
- **CommonJS**: Uses `require` and `module.exports`, synchronous loading, standard in Node.js.  
- **ES Modules (ESM)**: Uses `import` and `export`, supports asynchronous loading, part of the modern JavaScript standard.

---

## Section 2: Intermediate

### Q11. What are Promises and async/await in Node.js?  
**Ans:**  
- **Promises**: Objects representing eventual completion or failure of an async operation.  
- **async/await**: Syntax sugar over promises for writing asynchronous code in a synchronous style.

---

### Q12. How do you handle errors in asynchronous code?  
**Ans:** Using `.catch()` with promises or `try-catch` blocks inside `async` functions. Proper error handling prevents unhandled rejections and crashes.

---

### Q13. What are process objects in Node.js?  
**Ans:** The `process` object provides information about and control over the Node.js process, including environment variables, stdout/stderr, and process lifecycle events.

---

### Q14. Explain the difference between spawn, exec, and fork in Node.js.  
**Ans:**  
- `spawn`: Starts a new process, streams output.  
- `exec`: Runs a command, buffers output (good for small data).  
- `fork`: Special case of spawn to create a new Node.js process, communicates via IPC.

---

### Q15. What is an EventEmitter in Node.js? Give a real use case.  
**Ans:** `EventEmitter` is a class that allows emitting and listening to events. Example: `http.Server` emits `request` events, or a custom logger can emit `log` events.

---

### Q16. How does clustering work in Node.js?  
**Ans:** Clustering creates multiple worker processes to utilize multi-core CPUs. The master process distributes incoming connections to workers, improving throughput for CPU-bound tasks.

---

### Q17. Explain how you can achieve multithreading in Node.js.  
**Ans:** Node.js can achieve multithreading using **worker threads** (introduced in v10.5) or offloading CPU-intensive tasks to child processes while keeping the event loop non-blocking.

---

### Q18. What is the role of libuv in Node.js?  
**Ans:** libuv is a C library that handles asynchronous I/O operations for Node.js, including the event loop, file system operations, networking, and thread pooling.

---

### Q19. How do you handle uncaught exceptions in Node.js?  
**Ans:** Using `process.on('uncaughtException', callback)` or `process.on('unhandledRejection', callback)`. These should log errors and gracefully exit, as the process might be in an unstable state.

---

### Q20. Explain difference between process.env and dotenv package.  
**Ans:**  
- `process.env`: Accesses environment variables in Node.js.  
- `dotenv`: Loads variables from a `.env` file into `process.env`, making it easier to manage configurations.

---

## Section 3: Advanced

### Q21. What is JWT and how is it implemented in Node.js?  
**Ans:** JWT (JSON Web Token) is a token-based authentication mechanism. In Node.js, packages like `jsonwebtoken` are used to sign, verify, and decode tokens for secure user authentication.

---

### Q22. How do you implement authentication and authorization in Node.js?  
**Ans:** Authentication verifies identity (e.g., using JWT or OAuth). Authorization checks user permissions for accessing resources. Middleware in Express is often used to enforce both.

---

### Q23. What is rate limiting and how would you implement it in Node.js?  
**Ans:** Rate limiting restricts the number of API calls a user can make in a given time. It can be implemented using packages like `express-rate-limit` or custom in-memory counters.

---

### Q24. How do you secure a Node.js application from SQL Injection & XSS?  
**Ans:**  
- Use parameterized queries or ORM libraries to prevent SQL injection.  
- Sanitize user input and escape output to prevent XSS.  
- Use security libraries like `helmet` for HTTP headers.

---

### Q25. Explain CORS in Node.js. How to enable it?  
**Ans:** CORS (Cross-Origin Resource Sharing) controls which domains can access your API. In Express, it can be enabled using the `cors` middleware: `app.use(cors())`.

---

### Q26. What are worker threads in Node.js?  
**Ans:** Worker threads allow running CPU-intensive tasks in parallel to the main thread, preventing blocking of the event loop. They communicate via message passing.

---

### Q27. How does garbage collection work in Node.js?  
**Ans:** Node.js relies on V8’s garbage collector, which uses **mark-and-sweep** and generational algorithms to reclaim memory occupied by objects no longer in use.

---

### Q28. How do you monitor and debug performance issues in Node.js apps?  
**Ans:** Tools like `Node.js --inspect`, Chrome DevTools, `clinic.js`, or APM solutions (NewRelic, Datadog) can profile memory, CPU usage, event loop delays, and I/O bottlenecks.

---

### Q29. Explain the difference between process.nextTick() and queueMicrotask().  
**Ans:**  
- `process.nextTick()`: Runs callbacks **before the next event loop phase**.  
- `queueMicrotask()`: Runs callbacks at the end of the current synchronous execution but before the next event loop tick.  

---

### Q30. If an API is slow in Node.js, how would you debug and optimize it?  
**Ans:**  
- Profile with tools like `clinic.js` or `Node.js inspector`.  
- Check for blocking operations in the event loop.  
- Optimize database queries and use caching.  
- Offload CPU-intensive tasks to worker threads or microservices.

