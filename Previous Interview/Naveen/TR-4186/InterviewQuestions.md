# Java Interview Questions and Answers

## 1. Difference between Spring and Spring Boot

Spring is a comprehensive framework that provides a wide range of features for building Java enterprise applications such as dependency injection, MVC, and security. However, it requires a lot of manual configuration through XML or annotations.  
Spring Boot is built on top of Spring and simplifies the development process by providing **auto-configuration**, **embedded servers** (like Tomcat), and **opinionated defaults**. It eliminates boilerplate configuration and allows applications to run quickly with minimal setup.

---

## 2. What is Auto-Configuration?

Auto-configuration is one of the main features of Spring Boot that automatically configures your application based on the dependencies you have added.  
For example, if you add `spring-boot-starter-web`, it automatically configures the web server (Tomcat) and DispatcherServlet.  
It works using the `@EnableAutoConfiguration` annotation and scans the classpath to determine what beans should be created, allowing developers to focus on writing business logic instead of setup.

---

## 3. HashMap Internal Implementation

A **HashMap** in Java stores key-value pairs in an array of buckets. Each bucket can hold multiple entries using a linked list or a balanced tree (after Java 8).  
When you put a key-value pair, Java calculates the hash code of the key and determines the bucket index using a hash function.  
If two keys have the same hash code, a **collision** occurs, and both entries are stored in the same bucket (as a linked list or tree).  
During retrieval, the key’s hash code is used again to find the right bucket and locate the value using `equals()`.

---

## 4. What happens internally when calling map.put()?

When you call `map.put(key, value)`:

1. The `hashCode()` of the key is calculated.
2. The bucket index is determined using `(hash & (n - 1))`.
3. If the bucket is empty, the entry is inserted.
4. If the bucket already contains entries, Java checks if the key already exists using `equals()`:
   - If it exists, the old value is replaced.
   - If not, the new key-value pair is appended.
5. If a bucket’s size exceeds 8 entries, it is converted into a balanced tree for faster lookups (since Java 8).

---

## 5. What is ConcurrentModificationException?

A **ConcurrentModificationException** occurs when you modify a collection (like ArrayList or HashMap) while iterating over it using a for-each loop or an iterator.  
It’s a **fail-fast mechanism** that prevents inconsistent data during iteration.  
To avoid it, use an iterator’s own `remove()` method or use concurrent collections like `CopyOnWriteArrayList` or `ConcurrentHashMap` when modifications during iteration are required.

---

## 6. How to avoid ConcurrentModificationException?

To avoid this exception:

- Use the **Iterator’s `remove()` method** instead of directly calling `list.remove()` inside the loop.
- Use **concurrent collections** such as `ConcurrentHashMap` or `CopyOnWriteArrayList`.
- Collect elements to be modified in a separate list and update after iteration.  
  These approaches ensure thread-safe and stable iteration.

---

## 7. Custom-Defined Exception Example

Yes, I have created custom exceptions in my applications.  
When standard Java exceptions weren’t enough to represent a specific business logic, I created my own by extending `Exception` or `RuntimeException`.  
For example:

```java
public class InvalidEmployeeDataException extends RuntimeException {
    public InvalidEmployeeDataException(String message) {
        super(message);
    }
}
```

This allows better error handling and makes code easier to maintain and debug.

---

## 8. What is an Exception?

An **Exception** in Java is an event that occurs during program execution that disrupts the normal flow of instructions.  
It is an object that represents an error or unexpected event.  
Types of exceptions:

- **Checked Exceptions:** Must be handled using try-catch or declared in the method (`IOException`, `SQLException`).
- **Unchecked Exceptions:** Occur during runtime (`NullPointerException`, `ArithmeticException`).
- **Errors:** Serious problems that cannot be recovered (`OutOfMemoryError`).  
  Exceptions help applications handle errors gracefully without crashing.

---

## 9. What are Packages in Java and their Purpose?

A **package** in Java is a namespace that groups related classes and interfaces. It’s like a folder structure for organizing code.  
**Purpose of Packages:**

- Organize related classes and interfaces.
- Avoid naming conflicts.
- Control access (default access within a package).
- Enable code reusability.

Example:

```java
package com.company.employee;

public class Employee {
    private String name;
}
```

To use it:

```java
import com.company.employee.Employee;
```

Packages make applications more modular and maintainable.

---

## 10. Abstraction in Java and How It’s Used

**Abstraction** is the process of hiding implementation details and showing only the essential features.  
It is achieved using **abstract classes** and **interfaces**.

Example:

```java
abstract class Employee {
    abstract double calculateSalary();
}

class FullTimeEmployee extends Employee {
    double calculateSalary() {
        return 50000;
    }
}
```

In my application, I used abstraction to define a common template (`Employee`) and let subclasses (`FullTimeEmployee`, `ContractEmployee`) define their specific logic. This made the code flexible and easier to extend.

---

## 11. What is a Private Resource?

A **private resource** is a class member (variable, method, or constructor) declared with the `private` access modifier. It can only be accessed within its own class.  
Private resources ensure **encapsulation** and **data security**, and are accessed through public getter and setter methods.

Example:

```java
public class Employee {
    private String name;

    public String getName() { return name; }
    public void setName(String name) { this.name = name; }
}
```

---

## 12. Reverse a String Example

To reverse a string in Java:

**Using Loop:**

```java
public class ReverseString {
    public static void main(String[] args) {
        String str = "Naveen";
        String reversed = "";
        for (int i = str.length() - 1; i >= 0; i--) {
            reversed += str.charAt(i);
        }
        System.out.println("Reversed String: " + reversed);
    }
}
```

**Using StringBuilder:**

```java
public class ReverseString {
    public static void main(String[] args) {
        String str = "Naveen";
        String reversed = new StringBuilder(str).reverse().toString();
        System.out.println("Reversed String: " + reversed);
    }
}
```

Output:

```
Reversed String: neevaN
```
