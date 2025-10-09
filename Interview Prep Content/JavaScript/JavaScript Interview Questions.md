# JavaScript Interview Questions & Answers

---

### Q1. What is JavaScript?  
**Ans:** JavaScript is a high-level, interpreted programming language used primarily for web development to create interactive web pages. It supports event-driven, functional, and object-oriented programming and can run both in browsers and on servers.

---

### Q2. What are the data types supported by JavaScript?  
**Ans:** JavaScript has primitive types: `string`, `number`, `boolean`, `null`, `undefined`, `symbol`, and non-primitive types like `object`, which includes arrays, functions, and general objects.

---

### Q3. What is the difference between `let`, `const`, and `var`?  
**Ans:**  
- `var` is function-scoped, can be redeclared, and is hoisted with `undefined`.  
- `let` is block-scoped, cannot be redeclared in the same scope, and avoids hoisting issues.  
- `const` is block-scoped, must be initialized, and cannot be reassigned.

---

### Q4. Explain how `==` and `===` differ.  
**Ans:** `==` compares values with type coercion, while `===` compares values without type coercion and also checks data type equality.

---

### Q5. What is a closure?  
**Ans:** A closure is a function that remembers variables from its outer scope, even after the outer function has finished execution, allowing encapsulation and data privacy.

---

### Q6. What is hoisting?  
**Ans:** Hoisting is JavaScript's behavior of moving variable and function declarations to the top of their scope during compilation. Variables declared with `var` are hoisted with `undefined`, while `let` and `const` are hoisted but not initialized.

---

### Q7. Explain the concept of "this" in JavaScript.  
**Ans:** `this` refers to the context object within which a function is executed. Its value depends on whether the function is called globally, as a method, or as a class method.

---

### Q8. What are JavaScript prototypes?  
**Ans:** Every JavaScript object has a prototype, which is another object from which it can inherit properties and methods. Prototypes enable prototypal inheritance.

---

### Q9. What is the difference between `null` and `undefined`?  
**Ans:** `undefined` is the default value of variables that have been declared but not assigned. `null` represents an intentional absence of any value.

---

### Q10. How does JavaScript handle asynchronous operations?  
**Ans:** JavaScript handles asynchronous operations using event-driven mechanisms, including callbacks, promises, async/await, and the event loop, allowing non-blocking execution.

---

### Q11. What is a promise?  
**Ans:** A Promise is an object representing the eventual completion or failure of an asynchronous operation. It can be in one of three states: pending, fulfilled, or rejected.

---

### Q12. What are async/await functions?  
**Ans:** `async` functions always return a promise. `await` is used to pause execution of an async function until a promise resolves, making asynchronous code easier to read and maintain.

---

### Q13. Explain event delegation in JavaScript.  
**Ans:** Event delegation is a technique where a parent element handles events for its child elements, leveraging event bubbling to reduce memory usage and improve performance.

---

### Q14. What are JavaScript modules?  
**Ans:** JavaScript modules allow code to be organized in separate files, enabling export and import of variables, functions, and objects to improve maintainability and modularity.

---

### Q15. How can you prevent a function from being called multiple times?  
**Ans:** Functions can be controlled using debouncing or throttling techniques to limit execution frequency and avoid repeated calls.

---

### Q16. What is the event loop?  
**Ans:** The event loop continuously monitors the call stack and task queue, ensuring that asynchronous callbacks are executed once the main execution stack is empty.

---

### Q17. What is the difference between `apply()` and `call()` methods?  
**Ans:** Both are used to invoke functions with a specified `this` context. `call()` passes arguments individually, whereas `apply()` passes arguments as an array.

---

### Q18. What is `bind()` method used for?  
**Ans:** `bind()` creates a new function with a permanently bound `this` context without executing it immediately.

---

### Q19. What is a JavaScript event loop?  
**Ans:** The event loop is a mechanism that allows JavaScript to perform non-blocking asynchronous operations by managing execution order between the call stack and task queue.

---

### Q20. Explain the concept of "event bubbling" and "event capturing".  
**Ans:** Event bubbling is the process where events propagate from the child element up to the parent. Event capturing is the reverse, where events propagate from the parent down to the child. Developers can choose the phase for event handling.

---

### Q21. What is the difference between deep copy and shallow copy?  
**Ans:** A shallow copy copies only the top-level properties, leaving nested objects linked to the original. A deep copy duplicates all levels, creating independent copies of nested objects.

---

### Q22. What are generator functions?  
**Ans:** Generators are functions that can pause and resume execution at any point, allowing the production of multiple values over time while maintaining state between yields.

---

### Q23. What is the `new` keyword used for?  
**Ans:** The `new` keyword is used to create an instance of an object from a constructor function, setting up the prototype chain and initializing the new object.

---

### Q24. How do JavaScript’s `setTimeout` and `setInterval` work?  
**Ans:** `setTimeout` schedules a function to execute once after a specified delay, whereas `setInterval` schedules repeated execution at a specified interval. Both are handled asynchronously via the event loop.

---

### Q25. What is a `WeakMap` and how is it different from a `Map`?  
**Ans:** A `WeakMap` only accepts objects as keys and holds weak references, allowing garbage collection of unused keys. `Map` can have keys of any type and holds strong references.

---

### Q26. What is a `Set` in JavaScript?  
**Ans:** A `Set` is a collection of unique values that automatically ignores duplicates, providing an efficient way to store and manipulate distinct elements.

---

### Q27. What is `Object.create()` used for?  
**Ans:** `Object.create()` creates a new object with a specified prototype, enabling inheritance and object composition without using constructor functions.

---

### Q28. How does JavaScript’s garbage collection work?  
**Ans:** JavaScript automatically frees memory occupied by objects that are no longer reachable from the root references, using algorithms like mark-and-sweep.

---

### Q29. What are "decorators" in JavaScript?  
**Ans:** Decorators are functions that modify the behavior of classes, methods, or properties at design time, allowing enhancements without altering the original code.

---

### Q30. Explain the difference between `prototype` and `__proto__`.  
**Ans:** `prototype` is the object associated with a constructor used when creating new instances. `__proto__` is the internal reference of an object pointing to its prototype for inheritance.
