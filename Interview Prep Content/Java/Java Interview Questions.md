# Java Interview Questions & Answers (Intermediate & Advanced)

---

### Q1. What are the main features of Java?  
**Ans:** Key features include object-oriented programming, platform independence via JVM, automatic memory management, multithreading, strong type checking, and a robust standard library.

---

### Q2. What is the difference between JDK, JRE, and JVM?  
**Ans:**  
- **JVM:** Executes Java bytecode.  
- **JRE:** Provides runtime environment including JVM and libraries.  
- **JDK:** Full development kit including JRE, compiler, and tools.

---

### Q3. What is the difference between `==` and `.equals()` for objects?  
**Ans:** `==` checks reference equality (memory address), whereas `.equals()` checks **content equality**, depending on its implementation.

---

### Q4. Explain the difference between abstract class and interface.  
**Ans:**  
- Abstract class: Can have concrete and abstract methods, constructors, and fields.  
- Interface: Defines abstract methods (plus default/static methods in Java 8+), cannot have constructors, supports multiple inheritance.

---

### Q5. Difference between `String`, `StringBuilder`, and `StringBuffer`.  
**Ans:**  
- `String`: Immutable.  
- `StringBuilder`: Mutable, not thread-safe.  
- `StringBuffer`: Mutable, thread-safe.

---

### Q6. Difference between checked and unchecked exceptions.  
**Ans:**  
- Checked exceptions must be handled or declared (`IOException`).  
- Unchecked exceptions are runtime exceptions (`NullPointerException`) that do not require explicit handling.

---

### Q7. Difference between `ArrayList` and `LinkedList`.  
**Ans:**  
- ArrayList: Uses dynamic array, fast random access, slow insertion/deletion in middle.  
- LinkedList: Uses doubly linked nodes, slower random access, faster insert/delete operations.

---

### Q8. Difference between `HashMap` and `HashTable`.  
**Ans:**  
- HashMap: Non-synchronized, allows null keys/values.  
- Hashtable: Synchronized, does not allow null keys/values.

---

### Q9. Difference between `Comparable` and `Comparator`.  
**Ans:**  
- Comparable: Defines natural ordering via `compareTo` in the class itself.  
- Comparator: Defines custom ordering externally via `compare`.

---

### Q10. What is the difference between deep copy and shallow copy?  
**Ans:**  
- Shallow copy copies only top-level fields; nested objects remain shared.  
- Deep copy creates independent copies of nested objects.

---

### Q11. Difference between `final`, `finally`, and `finalize()`.  
**Ans:**  
- `final`: Keyword to declare constants, prevent inheritance or overriding.  
- `finally`: Code block executed after try/catch for cleanup.  
- `finalize()`: Method called by garbage collector before object destruction.

---

### Q12. Difference between `Runnable` and `Thread`.  
**Ans:**  
- Runnable: Interface implemented by a class; run method executed via Thread object.  
- Thread: Class that can be extended to create threads directly.

---

### Q13. Difference between synchronized method and synchronized block.  
**Ans:**  
- Synchronized method: Locks entire method for a single thread.  
- Synchronized block: Locks only critical section, more efficient.

---

### Q14. Difference between process.env and dotenv package.  
**Ans:** In Node.js (analogous concept in Java): Environment variables are accessed via system properties, and dotenv loads environment variables from a file for configuration.

---

### Q15. Difference between `spawn`, `exec`, and `fork`.  
**Ans:**  
- spawn: Launches new process with streams for input/output.  
- exec: Launches new process and buffers the output.  
- fork: Creates child process specifically for Node/Java process communication.

---

### Q16. Difference between `apply()` and `call()` methods.  
**Ans:** Call invokes a method with `this` and arguments individually; apply passes arguments as an array.

---

### Q17. Difference between `HashMap` and `TreeMap`.  
**Ans:**  
- HashMap: Unordered, allows null keys/values, fast operations.  
- TreeMap: Sorted based on natural ordering or comparator, no null keys.

---

### Q18. Difference between composition and inheritance.  
**Ans:**  
- Composition: One object contains another, promotes flexibility.  
- Inheritance: One class extends another, promotes code reuse but less flexible.

---

### Q19. Difference between `wait()` and `sleep()`.  
**Ans:**  
- wait(): Releases the lock and waits until notified.  
- sleep(): Does not release lock, pauses execution for specified time.

---

### Q20. Difference between `volatile` and `synchronized`.  
**Ans:**  
- volatile: Ensures visibility of variable changes across threads.  
- synchronized: Ensures mutual exclusion, controlling access to critical section.

---

### Q21. Difference between `==` and `equals()` for strings.  
**Ans:** `==` checks reference equality, `.equals()` checks content equality of strings.

---

### Q22. Difference between abstract class and concrete class.  
**Ans:**  
- Abstract class: Cannot be instantiated, may contain abstract methods.  
- Concrete class: Can be instantiated, must implement all abstract methods of parent classes.

---

### Q23. Difference between stack and queue.  
**Ans:**  
- Stack: Follows LIFO (Last In First Out).  
- Queue: Follows FIFO (First In First Out).

---

### Q24. Difference between shallow copy and deep copy in objects.  
**Ans:** Shallow copy copies references; deep copy creates independent object clones.

---

### Q25. Difference between constructor and method.  
**Ans:** Constructor initializes new object instances; method defines object behavior.

---

### Q26. Difference between `instanceof` and `getClass()`.  
**Ans:**  
- instanceof: Checks if an object is an instance of a class or subclass.  
- getClass(): Returns the exact runtime class of the object.

---

### Q27. Difference between `try-with-resources` and `try-catch-finally`.  
**Ans:** try-with-resources automatically closes resources; try-catch-finally requires manual closing.

---

### Q28. Difference between `throw` and `throws`.  
**Ans:**  
- throw: Used to explicitly throw an exception.  
- throws: Declares exceptions a method might throw to the caller.

---

### Q29. Difference between `HashSet` and `TreeSet`.  
**Ans:**  
- HashSet: Unordered, allows null, fast operations.  
- TreeSet: Sorted, does not allow null, slower operations.

---

### Q30. Difference between `abstract class` and `interface` after Java 8.  
**Ans:** Interfaces can have default/static methods; abstract classes can have constructors, instance variables, and concrete methods.

---

# Java OOP Interview Questions

---

### Q31. What is Object-Oriented Programming (OOP) in Java?  
**Ans:** OOP is a programming paradigm that organizes software around **objects** containing data and behavior. Java supports **encapsulation, inheritance, polymorphism, and abstraction**.

---

### Q32. What is a class and an object?  
**Ans:**  
- Class: A blueprint defining attributes and behavior.  
- Object: An instance of a class with its own state.

---

### Q33. Explain encapsulation in Java.  
**Ans:** Encapsulation is **hiding internal data** and exposing only necessary methods via access modifiers to ensure controlled access.

---

### Q34. What is inheritance in Java?  
**Ans:** Inheritance allows a class to **reuse properties and methods** of another class, establishing an **“is-a” relationship**.

---

### Q35. What is polymorphism in Java?  
**Ans:** Polymorphism allows objects to **take multiple forms**:  
- Compile-time polymorphism (method overloading)  
- Runtime polymorphism (method overriding)

---

### Q36. What is abstraction in Java?  
**Ans:** Abstraction hides implementation details and shows only essential features. Achieved via **abstract classes and interfaces**.

---

### Q37. Difference between method overloading and overriding.  
**Ans:**  
- Overloading: Same method name, different parameters (compile-time).  
- Overriding: Subclass changes superclass method behavior (runtime).

---

### Q38. Difference between `super` and `this`.  
**Ans:**  
- super: Refers to parent class members.  
- this: Refers to current object members.

---

### Q39. Difference between `has-a` and `is-a` relationships.  
**Ans:**  
- is-a: Inheritance relationship.  
- has-a: Composition relationship.

---

### Q40. What is a constructor?  
**Ans:** Special method used to **initialize objects** when they are created.

---

### Q41. Difference between composition and aggregation.  
**Ans:**  
- Composition: Strong “has-a” relationship; lifetime bound to container.  
- Aggregation: Weak “has-a” relationship; contained object can exist independently.

---

### Q42. What is method hiding?  
**Ans:** Occurs when a **static method in subclass** has the same signature as in superclass. Resolved at compile-time.

---

### Q43. Difference between abstract method and interface method.  
**Ans:**  
- Abstract method: Defined in abstract class, must be implemented in subclass.  
- Interface method: Defined in interface, must be implemented; can have default/static methods (Java 8+).

---

### Q44. What is dynamic method dispatch?  
**Ans:** The runtime process of selecting which **overridden method** to execute based on the object type.

---

### Q45. What are access modifiers in Java?  
**Ans:**  
- private, default (package-private), protected, public; control visibility of classes, methods, and variables.

---

### Q46. Difference between multiple inheritance via classes and interfaces.  
**Ans:**  
- Java does **not allow multiple inheritance with classes**.  
- Multiple inheritance is possible via **interfaces**.

---

### Q47. Difference between constructor and method.  
**Ans:** Constructor initializes object; method defines behavior. Constructor has no return type.

---

### Q48. Difference between static and instance methods.  
**Ans:**  
- static: Belongs to class, can be called without object.  
- instance: Belongs to object, requires object to call.

---

### Q49. Difference between interface and marker interface.  
**Ans:**  
- Interface: Defines methods for classes to implement.  
- Marker interface: No methods; used to mark class for special behavior (e.g., Serializable).

---

### Q50. Difference between stack and heap in Java.  
**Ans:**  
- Stack: Stores local variables and method calls, LIFO, automatically managed.  
- Heap: Stores objects, shared across threads, managed by garbage collector.
