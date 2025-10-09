# Python Interview Questions & Answers

## Q1. Explain the difference between list and tuple in Python.  
**Ans:** Lists are mutable (modifiable) sequences of elements, defined using square brackets `[ ]`. Tuples are immutable (unchangeable) sequences defined using parentheses `( )`. Tuples are typically used for fixed data and faster access, whereas lists allow modification.

---

## Q2. What is PEP 8?  
**Ans:** PEP 8 is the Python Enhancement Proposal that provides guidelines for writing clean, readable Python code. It covers coding conventions, indentation, naming conventions, and more to enhance code consistency and readability.

---

## Q3. How does Python handle memory management?  
**Ans:** Python uses an automatic memory management system with a private heap for storing objects. The memory manager handles allocation and deallocation, while a built-in garbage collector recycles unused memory.

---

## Q4. What is the difference between `str` and `repr` methods in Python?  
**Ans:** Both `str` and `repr` represent objects as strings.  
- `str` is used when `print()` or `str()` is called, focusing on readability.  
- `repr` is used for debugging and in the interpreter, focusing on unambiguous representation.

---

## Q5. What are lambda functions in Python?  
**Ans:** Lambda functions are small, anonymous functions defined using the `lambda` keyword. They can take any number of arguments but have only one expression. They are often used for short, throwaway operations.

---

## Q6. How do you handle exceptions in Python?  
**Ans:** Exceptions are handled using `try-except` blocks. Code that might raise an exception is placed in `try`, errors are caught in `except`, and `finally` executes cleanup code regardless of success or failure.

---

## Q7. What is the Global Interpreter Lock (GIL) in Python?  
**Ans:** The GIL ensures only one thread executes Python bytecode at a time. It limits true parallelism for CPU-bound tasks but still allows concurrency for I/O-bound operations.

---

## Q8. How can you share global variables across modules in Python?  
**Ans:** Create a separate module to hold global variables and import it wherever needed. This ensures a single source of truth across multiple modules.

---

## Q9. Explain the usage of `__init__` method in Python.  
**Ans:** The `__init__` method is a constructor that initializes object attributes when a class instance is created. It allows instance-specific setup during object creation.

---

## Q10. What are iterators and generators in Python?  
**Ans:**  
- **Iterators** implement `__iter__()` and `__next__()` to allow sequential access.  
- **Generators** are iterators created with `yield`, producing values lazily and saving memory.

---

## Q11. Differentiate between `range()` and `xrange()` in Python 2.x.  
**Ans:** In Python 2.x, `range()` generates a list in memory, while `xrange()` returns an object that generates numbers on-the-fly. In Python 3, `range()` behaves like `xrange()`.

---

## Q12. How do you handle file operations in Python?  
**Ans:** File operations use functions like `open()`, `read()`, `write()`, and `close()`. The `with` statement is recommended as it ensures files are automatically closed after use.

---

## Q13. What are the benefits of using Python for web development?  
**Ans:** Python offers rapid development, readability, and frameworks like Django and Flask. It has strong community support, scalability, and integration with databases and APIs.

---

## Q14. Explain the difference between `getattr` and `getattribute`.  
**Ans:**  
- `getattribute` is called for **every attribute access**.  
- `getattr` is called **only when an attribute does not exist**, providing a fallback mechanism.

---

## Q15. How can you perform multithreading in Python?  
**Ans:** Python’s `threading` module allows multithreading, enabling concurrent execution. However, due to the GIL, multithreading is best suited for I/O-bound tasks, not CPU-bound ones.

---

## Q16. What is the use of `__doc__` and `__annotations__` attributes?  
**Ans:**  
- `__doc__` holds the documentation string of a function, class, or module.  
- `__annotations__` stores type hints for function arguments and return values.

---

## Q17. How do you manage packages in Python?  
**Ans:** Python uses tools like `pip` and `conda` to install, upgrade, and remove packages. They manage dependencies and ensure consistency across projects.

---

## Q18. Explain the purpose of `pass`, `break`, and `continue`.  
**Ans:**  
- `pass`: Placeholder that does nothing.  
- `break`: Terminates the loop.  
- `continue`: Skips the current iteration and moves to the next one.

---

## Q19. What are the benefits of virtual environments in Python?  
**Ans:** Virtual environments isolate dependencies for each project, preventing conflicts and allowing different projects to use different package versions.

---

## Q20. How can you handle JSON data in Python?  
**Ans:** Python’s `json` module allows converting JSON to Python objects with `json.loads()` and Python objects to JSON with `json.dumps()`.

---

## Q21. Explain the usage of `__slots__` in Python classes.  
**Ans:** `__slots__` defines a fixed set of attributes for a class, reducing memory usage by avoiding per-instance dictionaries. It also restricts dynamic attribute creation.

---
## Q22. What is monkey patching in Python?

**Ans:** Monkey patching means modifying or extending code at runtime without altering the original source. For example, replacing a method of a class dynamically. While powerful, it should be used cautiously as it can cause unexpected behavior.

---

## Q23. What is the difference between deep copy and shallow copy?

**Ans:**

- **Shallow Copy**: Copies only the outer object but references the same nested objects.
    
- **Deep Copy**: Recursively copies everything, making a completely independent copy.  
    Python’s `copy` module provides both options.
    

---

## Q24. What is the difference between `@classmethod`, `@staticmethod`, and instance methods?

**Ans:**

- **Instance method**: Takes `self` and works with object data.
    
- **Class method**: Takes `cls` and works with class-level data.
    
- **Static method**: Doesn’t take `self` or `cls`, works like a regular function inside a class.
    

---

## Q25. What is the difference between Python’s `is` and `==` operators?

**Ans:**

- `==` checks **value equality**.
    
- `is` checks **object identity** (whether two variables point to the same memory location).
    

---

## Q26. Explain Python’s garbage collection mechanism.

**Ans:** Python primarily uses **reference counting**. When an object’s reference count drops to zero, memory is freed. It also includes a **cyclic garbage collector** to handle reference cycles.

---

## Q27. What is the difference between mutable and immutable data types in Python?

**Ans:**

- **Mutable**: Can be changed after creation (e.g., lists, dictionaries, sets).
    
- **Immutable**: Cannot be changed after creation (e.g., strings, tuples, integers).
    

---

## Q28. What is the purpose of the `with` statement in Python?

**Ans:** The `with` statement simplifies resource management. It ensures proper cleanup (like closing files or releasing locks) by using context managers, even if errors occur.

---

## Q29. What are Python metaclasses?

**Ans:** A metaclass is the **class of a class**. Just as classes define how objects are created, metaclasses define how classes are created. They allow customization of class behavior at creation time.

---

## Q30. Explain the difference between multithreading and multiprocessing in Python.

**Ans:**

- **Multithreading**: Multiple threads run within the same process. Limited by the GIL, best for I/O-bound tasks.
    
- **Multiprocessing**: Multiple processes run independently with separate memory, suitable for CPU-bound tasks.
    

---

## Q31. What is the purpose of the `__name__ == "__main__"` statement?

**Ans:** It ensures code inside that block runs **only when the script is executed directly**, not when imported as a module. It’s used to control the script’s entry point.

---

## Q32. What are Python’s built-in data serialization options?

**Ans:** Python supports **JSON, Pickle, Marshal, and CSV** for data serialization. JSON is most common for data exchange, while Pickle is Python-specific for object persistence.

---

## Q33. What are Python descriptors?

**Ans:** Descriptors are objects that define how attribute access is managed in a class using methods like `__get__`, `__set__`, and `__delete__`. They form the basis of properties and methods like `@property`.

---

## Q34. What is duck typing in Python?

**Ans:** Duck typing means Python focuses on **behavior, not type**. If an object behaves like the expected type (e.g., supports iteration), it can be used, regardless of its actual class.

---

## Q35. What are Python’s common use cases?

**Ans:** Python is widely used for web development, data science, machine learning, automation, scripting, testing, DevOps, and cloud computing due to its simplicity and vast ecosystem.

---

## Q36. What is break, continue and pass in Python?

Ans:

|   |   |
|---|---|
|Break|The break statement terminates the loop immediately and the control flows to the statement after the body of the loop.|
|Continue|The continue statement terminates the current iteration of the statement, skips the rest of the code in the current iteration and the control flows to the next iteration of the loop.|
|Pass|As explained above, the pass keyword in Python is generally used to fill up empty blocks and is similar to an empty statement represented by a semi-colon in languages such as Java, C++, Javascript, etc.|

---

## Q37. 
