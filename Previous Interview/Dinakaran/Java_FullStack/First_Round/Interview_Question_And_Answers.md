Here’s your **complete Markdown (.md)** document including **all interview + coding + MCQ questions with correct answers**, formatted for clean reading or documentation use.

---

# 💼 **Java Full Stack Developer — Interview Q&A (Dinakaran Ramadass)**

---

## 🧑‍💻 **1. Brief Introduction**

Hi, I’m **Dinakaran Ramadass**, a **Java Full Stack Developer** with around **12 years of experience** in designing and developing scalable, secure, and cloud-ready enterprise applications.

Currently, I’m working as a **Lead Full Stack Java Developer** at **Infyni**, leading the architecture and end-to-end development of EdTech solutions using **Spring Boot, Angular 16+, AWS, Docker, and Kubernetes**.
I also implement **event-driven systems** using **Kafka and RabbitMQ**, and manage CI/CD pipelines using **GitHub Actions and Jenkins**.

Before this, I worked at **KPMG (Finance domain)**, **Cotocus (Telecom domain)**, and **NTT DATA (IT services)**, focusing on microservices, secure API integration, and performance optimization.

I’m passionate about building **high-performance, secure, and scalable applications** while following **clean code and agile practices**.

---

## ⚙️ **2. Core Principles in Java OOPs**

| OOP Concept       | Description                                                 | Example/Notes                                             |
| ----------------- | ----------------------------------------------------------- | --------------------------------------------------------- |
| **Encapsulation** | Binding data and methods into a single class                | Achieved using private fields with public getters/setters |
| **Inheritance**   | Reusing code by deriving new classes from existing ones     | `class Employee extends Person {}`                        |
| **Polymorphism**  | One action, multiple forms                                  | Overloading (compile-time) / Overriding (runtime)         |
| **Abstraction**   | Hiding implementation details, exposing only necessary info | Achieved using abstract classes/interfaces                |

---

## 🧩 **3. HashMap vs ConcurrentHashMap vs Hashtable**

| Feature          | HashMap              | Hashtable                   | ConcurrentHashMap                |
| ---------------- | -------------------- | --------------------------- | -------------------------------- |
| **Thread Safe**  | ❌ No                | ✅ Yes (full map lock)      | ✅ Yes (bucket-level / CAS lock) |
| **Null Allowed** | ✅ Yes               | ❌ No                       | ❌ No                            |
| **Performance**  | Fast (single-thread) | Slow (full synchronization) | Fast (concurrent threads)        |
| **Iterator**     | Fail-fast            | Fail-fast                   | Fail-safe                        |

✅ **Fastest:** `ConcurrentHashMap`
❌ **Slowest:** `Hashtable`

---

## 🧾 **4. Checked vs Unchecked Exceptions**

| Checked Exceptions                       | Unchecked Exceptions                                    |
| ---------------------------------------- | ------------------------------------------------------- |
| Checked at **compile-time**              | Checked at **runtime**                                  |
| Must handle with `try-catch` or `throws` | Not required to handle                                  |
| Examples: `IOException`, `SQLException`  | Examples: `NullPointerException`, `ArithmeticException` |
| Usually **recoverable**                  | Usually **logic/programming errors**                    |

**One-liner:**

> Checked exceptions are compile-time; unchecked exceptions are runtime.

---

## 🔐 **5. How Do You Secure REST APIs Using JWT?**

### Steps:

1. User logs in → sends credentials to `/authenticate`.
2. Server validates credentials.
3. Server generates a JWT (signed using secret key).
4. Client stores token (localStorage/sessionStorage).
5. Client sends token with every request:

   ```
   Authorization: Bearer <jwt-token>
   ```

6. Backend validates token and authorizes request.

### Example:

```java
http.csrf().disable()
    .authorizeRequests()
    .anyRequest().authenticated()
    .and()
    .addFilterBefore(jwtFilter, UsernamePasswordAuthenticationFilter.class);
```

**One-liner:**

> JWT secures REST APIs by validating signed tokens in every request header.

---

## ⚡ **6. How Do You Handle Exceptions Globally in Spring Boot?**

### Using `@ControllerAdvice` and `@ExceptionHandler`:

```java
@ControllerAdvice
public class GlobalExceptionHandler {

    @ExceptionHandler(ResourceNotFoundException.class)
    public ResponseEntity<?> handleResourceNotFound(ResourceNotFoundException ex) {
        return new ResponseEntity<>(ex.getMessage(), HttpStatus.NOT_FOUND);
    }

    @ExceptionHandler(Exception.class)
    public ResponseEntity<?> handleGlobalException(Exception ex) {
        return new ResponseEntity<>("Internal Server Error", HttpStatus.INTERNAL_SERVER_ERROR);
    }
}
```

✅ Centralized error handling
✅ Clean controller logic
✅ Consistent JSON error responses

---

## 🧱 **7. Valid Way to Define a Standalone Component in Angular 16**

```ts
import { Component } from "@angular/core";

@Component({
  selector: "app-dashboard",
  standalone: true,
  templateUrl: "./dashboard.component.html",
  styleUrls: ["./dashboard.component.css"],
})
export class DashboardComponent {}
```

**With Imports:**

```ts
@Component({
  selector: "app-login",
  standalone: true,
  imports: [CommonModule],
  template: `<h1>Login</h1>`,
})
export class LoginComponent {}
```

✅ Use `standalone: true`
✅ No `NgModule` needed
✅ Use `imports` inside component metadata

---

## 🌐 **8. How Do You Enable Routing in Angular Standalone Applications?**

### Step 1: Define Routes (`app.routes.ts`)

```ts
import { Routes } from "@angular/router";
import { HomeComponent } from "./home/home.component";
import { LoginComponent } from "./login/login.component";

export const routes: Routes = [
  { path: "", component: HomeComponent },
  { path: "login", component: LoginComponent },
];
```

### Step 2: Configure Routing in `main.ts`

```ts
import { bootstrapApplication } from "@angular/platform-browser";
import { AppComponent } from "./app/app.component";
import { provideRouter } from "@angular/router";
import { routes } from "./app/app.routes";

bootstrapApplication(AppComponent, {
  providers: [provideRouter(routes)],
});
```

### Step 3: Add Router Outlet in AppComponent

```ts
@Component({
  selector: "app-root",
  standalone: true,
  template: `<router-outlet></router-outlet>`,
})
export class AppComponent {}
```

✅ Uses `provideRouter()`
✅ No `AppRoutingModule` required
✅ Bootstrapped using `bootstrapApplication()`

---

## 💻 **Coding Questions**

### **1. Find the Second Highest Number Without Sorting**

**Question:**
Find the second highest number in a list without sorting.

**Input:**

```
[5, 2, 9, 1, 7, 9]
```

**Answer:**

```java
public class SecondHighest {
    public static void main(String[] args) {
        int[] numbers = {5, 2, 9, 1, 7, 9};
        Integer first = null, second = null;

        for (int n : numbers) {
            if (first == null || n > first) {
                second = first;
                first = n;
            } else if ((second == null || n > second) && n != first) {
                second = n;
            }
        }

        System.out.println("Second highest number: " + second);
    }
}
```

**Output:**

```
Second highest number: 7
```

---

### **2. SQL Query: Find the Highest Paid Employee in Each Department**

**Table:** `Employee(id, name, dept, salary)`

**Answer (Subquery):**

```sql
SELECT e.dept, e.name, e.salary
FROM Employee e
WHERE e.salary = (
    SELECT MAX(salary)
    FROM Employee
    WHERE dept = e.dept
);
```

**Alternative (Using Window Function):**

```sql
SELECT dept, name, salary
FROM (
    SELECT dept, name, salary,
           RANK() OVER (PARTITION BY dept ORDER BY salary DESC) AS rnk
    FROM Employee
) ranked
WHERE rnk = 1;
```

**Output:**

| Dept | Name | Salary |
| ---- | ---- | ------ |
| IT   | Alex | 90000  |
| HR   | Mona | 75000  |

---

## 🧠 **MCQ Questions**

### **Q1. Which of the following statements about Java Streams API is TRUE?**

✅ **B. Streams provide lazy evaluation**

**Explanation:**
Intermediate operations in Streams are lazy and only execute when a terminal operation is called.

---

### **Q2. What will be the output of this code?**

```java
int x = 10, y = 0;

try {
    int result = x / y;
} catch (ArithmeticException e) {
    System.out.println("Error");
} finally {
    System.out.println("Finally");
}
```

**Output:**

```
Error
Finally
```

---

### **Q3. Which collection is thread-safe without manual synchronization?**

✅ **C. ConcurrentHashMap**

**Explanation:**
`ConcurrentHashMap` allows concurrent read/write using fine-grained locking.

---

### **Q4. What annotation defines a REST controller in Spring Boot?**

✅ **B. @RestController**

**Explanation:**
`@RestController` = `@Controller` + `@ResponseBody`

---

### **Q5. What is the default scope of a Spring Bean?**

✅ **C. Singleton**

**Explanation:**
Spring beans are singleton by default — one instance per container.

---

### **Q6. Which annotation maps HTTP GET requests in Spring Boot?**

✅ **C. @GetMapping**

**Explanation:**
`@GetMapping` handles GET HTTP requests to fetch data.

---

## 🏁 **Prepared for**

**Candidate:** Dinakaran Ramadass
**Position:** Lead Full Stack Java Developer (Cloud & Enterprise Domain)
**Client:** Wells Fargo
**Vendor:** Digital iTechnology

---

Would you like me to generate a **downloadable `.md` file** or a **PDF version** for submission?
ds
