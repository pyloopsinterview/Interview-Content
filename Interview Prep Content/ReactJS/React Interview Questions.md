# React Interview Questions & Answers

---

## Section 1: React Basics

### Q1. What is React?  
**Ans:** React is a JavaScript library for building user interfaces. It focuses on creating reusable UI components and efficiently updating the DOM using a virtual DOM.  

---

### Q2. What is JSX?  
**Ans:** JSX is a syntax extension for JavaScript that allows writing HTML-like code inside JavaScript. It makes UI code more readable and React components easier to write.  

---

### Q3. What is Virtual DOM and why is it faster?  
**Ans:** Virtual DOM is an in-memory representation of the real DOM. React updates the virtual DOM first, compares it with the previous version (diffing), and only applies the minimal changes to the real DOM. This reduces unnecessary re-renders and improves performance.  

---

### Q4. What are React components?  
**Ans:** Components are reusable, independent building blocks of a React application. They can be **functional** (using functions) or **class-based**, and they manage UI and state.  

---

### Q5. Difference between props and state?  
**Ans:**  
- **Props**: Read-only data passed from parent to child components. Cannot be modified by the component receiving them.  
- **State**: Mutable data managed within a component. Changes to state trigger re-renders.  

---

## Section 2: Core Concepts

### Q6. Controlled vs Uncontrolled components?  
**Ans:**  
- **Controlled components**: Form elements whose values are controlled by React state.  
- **Uncontrolled components**: Form elements that manage their own state internally, typically accessed using refs.  

---

### Q7. Why use key in React lists?  
**Ans:** Keys help React identify which items have changed, added, or removed. This allows efficient re-rendering and ensures consistent UI updates.  

---

### Q8. What are React Fragments?  
**Ans:** Fragments let you group multiple elements without adding extra nodes to the DOM. They are written as `<React.Fragment>` or `<>...</>`.  

---

### Q9. What is prop drilling and how to avoid it?  
**Ans:** Prop drilling occurs when data is passed through multiple intermediate components unnecessarily. It can be avoided using **Context API**, Redux, or other state management libraries.  

---

### Q10. What is reconciliation?  
**Ans:** Reconciliation is React’s process of updating the DOM by comparing the previous virtual DOM with the new one and applying only necessary changes.  

---

## Section 3: React Hooks

### Q11. What is useState hook?  
**Ans:** `useState` is a hook that lets functional components have local state. It returns the current state value and a function to update it.  

---

### Q12. What is useEffect hook?  
**Ans:** `useEffect` is used to perform side effects in functional components, like fetching data, subscribing to events, or manipulating the DOM. It runs after the render cycle.  

---

### Q13. What is useContext hook?  
**Ans:** `useContext` allows functional components to access context values directly, avoiding prop drilling and making state sharing easier across components.  

---

### Q14. What is useReducer hook?  
**Ans:** `useReducer` is an alternative to `useState` for complex state logic. It uses a reducer function to update state based on dispatched actions.  

---

### Q15. Difference between useMemo and useCallback?  
**Ans:**  
- `useMemo` memoizes a **computed value** to avoid expensive recalculations.  
- `useCallback` memoizes a **function definition** to prevent unnecessary re-creations on re-renders.  

---

## Section 4: Advanced React

### Q16. What is useRef hook?  
**Ans:** `useRef` creates a mutable object which persists across renders. It’s commonly used to access DOM elements or store mutable values without triggering re-renders.  

---

### Q17. What are Higher-Order Components (HOCs)?  
**Ans:** HOCs are functions that take a component and return a new enhanced component. They are used for code reuse, logic abstraction, and injecting props.  

---

### Q18. What are Pure Components / React.memo?  
**Ans:**  
- **PureComponent** (class-based) and **React.memo** (functional) prevent unnecessary re-renders by doing a shallow comparison of props.  

---

### Q19. What are the Rules of Hooks?  
**Ans:**  
1. Only call hooks at the top level of a component or custom hook.  
2. Only call hooks from React functional components or custom hooks.  

---

### Q20. Why should you not mutate state directly?  
**Ans:** Direct mutation can cause unpredictable behavior and prevent React from detecting changes, leading to rendering bugs. Always use setState or state updater functions.  

---

## Section 5: Routing & State Management

### Q21. What is React Router?  
**Ans:** React Router is a library for handling routing in React applications. It allows navigation between different views without full page reloads.  

---

### Q22. Context API vs Redux?  
**Ans:**  
- **Context API**: Best for small to medium apps, sharing state between components without prop drilling.  
- **Redux**: Centralized state management with strict patterns, suitable for complex apps with large state and multiple data flows.  

---

### Q23. What is conditional rendering in React?  
**Ans:** Conditional rendering allows components to render different UI based on conditions using `if` statements, ternary operators, or logical &&.  

---

### Q24. What is idempotency in APIs (React usage)?  
**Ans:** Idempotency ensures that making the same API request multiple times produces the same result without additional side effects. React uses it in API calls to avoid duplicate state updates.  

---

### Q25. What are controlled forms in React?  
**Ans:** Controlled forms are form elements whose values are controlled by React state. They make validation, submission, and state management easier.  

---

## Section 6: Performance & Deployment

### Q26. How do you optimize React performance?  
**Ans:** Techniques include:  
- Using PureComponent or React.memo  
- Avoiding anonymous functions in props  
- Using useMemo and useCallback  
- Code splitting and lazy loading  
- Minimizing unnecessary re-renders  

---

### Q27. What is Server-Side Rendering (SSR)?  
**Ans:** SSR renders React components on the server, sending fully rendered HTML to the client. This improves performance, SEO, and initial load speed.  

---

### Q28. What is lazy loading in React?  
**Ans:** Lazy loading is a technique to load components or modules only when needed. React provides `React.lazy()` and `Suspense` to implement it.  

---

### Q29. Common mistakes React devs make?  
**Ans:**  
- Directly mutating state  
- Forgetting dependency arrays in useEffect  
- Overusing props drilling  
- Rendering unnecessary components  
- Not using keys properly in lists  

---

### Q30. What are PropTypes in React?  
**Ans:** PropTypes provide type-checking for component props. They help catch bugs by validating prop types at runtime, ensuring correct usage of components.  
