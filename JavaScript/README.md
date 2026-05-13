## 📋 JavaScript Interview Questions

1. [What are the different data types in JavaScript?](#q1-what-are-the-different-data-types-in-javascript)
2. [Explain the difference between var, let, and const.](#q2-explain-the-difference-between-var-let-and-const)
3. [What is hoisting in JavaScript?](#q3-what-is-hoisting-in-javascript)
4. [What are closures?](#q4-what-are-closures)
5. [Explain event bubbling and event capturing.](#q5-explain-event-bubbling-and-event-capturing)
6. [What are Promises and how do they work?](#q6-what-are-promises-and-how-do-they-work)
7. [What is async/await and how does it relate to Promises?](#q7-what-is-asyncawait-and-how-does-it-relate-to-promises)
8. [What is the Event Loop in JavaScript?](#q8-what-is-the-event-loop-in-javascript)
9. [What is callback hell in JavaScript?](#q9-what-is-callback-hell-in-javascript)
10. [Explain destructuring assignment in JavaScript.](#q10-explain-destructuring-assignment-in-javascript)
11. [What is the spread operator and rest parameters?](#q11-what-is-the-spread-operator-and-rest-parameters)
12. [Explain the concept of currying in JavaScript.](#q12-explain-the-concept-of-currying-in-javascript)

---

### **Q1: What are the different data types in JavaScript?**

JavaScript has two types of data types: Primitive and Non-Primitive.
Primitive types include string, number, boolean, null, undefined, bigint, and symbol — they store values directly and are immutable.
Non-primitive types like objects, arrays, and functions store data by reference and are mutable.

---

### **Q2: Explain the difference between var, let, and const.**

`var` is function-scoped and can be re-declared and updated, which can cause bugs.
`let` and `const` are block-scoped. `let` can be updated but not re-declared, while `const` cannot be updated or re-declared.
Due to better scoping and safety, `let` and `const` are preferred over `var`.

---

### **Q3: What is hoisting in JavaScript?**

Hoisting is JavaScript's behavior where variable and function declarations are moved to the top of their scope during the compilation phase.
Variables declared with `var` are initialized with `undefined`, while `let` and `const` are hoisted but remain in the Temporal Dead Zone until initialized. Function declarations are fully hoisted.

---

### **Q4: What are closures?**

A closure is a function that retains access to its outer scope variables even after the outer function has executed. It allows functions to maintain state and is commonly used for data encapsulation and callbacks.

---

### **Q5: Explain event bubbling and event capturing.**

Event bubbling is when an event propagates from the target element up to its ancestors, while event capturing is when the event travels from the root down to the target element. By default, JavaScript uses bubbling, but capturing can be enabled using the third parameter in addEventListener.

---

### **Q6: What are Promises and how do they work?**

A Promise is an object in JavaScript that represents the eventual completion or failure of an asynchronous operation. It has three states: pending, fulfilled, and rejected. Promises are handled using `.then()`, `.catch()`, or `async/await` for better readability and error handling.

---

### **Q7: What is async/await and how does it relate to Promises?**

`async/await` is a modern syntax built on top of Promises that allows writing asynchronous code in a synchronous style. An `async` function always returns a Promise, and `await` pauses execution until the Promise resolves or rejects. It improves readability and simplifies error handling using try/catch.

---

### **Q8: What is the Event Loop in JavaScript?**

The Event Loop is a mechanism in JavaScript that manages asynchronous operations by continuously checking the call stack and callback queues. It ensures that the call stack is empty before pushing queued tasks. Microtasks like Promises are executed before macrotasks like setTimeout.

---

### **Q9: what is callback hell in javascript?**

Callback hell is a situation in JavaScript where multiple nested callbacks make the code difficult to read and maintain. It usually occurs in asynchronous operations. It can be avoided by using `Promises` or `async/await` for better structure and readability.

---

### **Q10: Explain destructuring assignment in JavaScript.**

Destructuring assignment in JavaScript is a syntax that allows extracting values from arrays or properties from objects into separate variables in a concise way. It improves readability and reduces repetitive code.

---

### **Q11: What is the spread operator and rest parameters?**

The spread operator `(...)` is used to expand arrays or objects into individual elements, while rest parameters collect multiple values into a single array. Spread is commonly used for copying and merging, whereas rest is mainly used in function parameters.

---

### **Q12: Explain the concept of currying in JavaScript.**

Currying is a functional programming technique in JavaScript where a function with multiple arguments is converted into a series of nested functions, each accepting one argument at a time. It helps in code reusability, partial application, and creating more flexible functions.
