## 📋 React Interview Questions

1. [What is React, and how is it different from other frameworks?](#q1-what-is-react-and-how-is-it-different-from-other-frameworks)
2. [What are key features of React?](#q2-what-are-key-features-of-react)
3. [Explain the Virtual DOM and how it works?](#q3-explain-the-virtual-dom-and-how-it-works)
4. [What are components? Difference between functional and class components?](#q4-what-are-components-difference-between-functional-and-class-components)
5. [What are props and state? How are they different?](#q5-what-are-props-and-state-how-are-they-different)
6. [Explain the component lifecycle](#q6-explain-the-component-lifecycle)
7. [What is JSX?](#q7-what-is-jsx)
8. [How do you handle events in React?](#q8-how-do-you-handle-events-in-react)
9. [What is conditional rendering?](#q9-what-is-conditional-rendering)
10. [What are React Hooks? Explain `useState` and `useEffect`](#q10-what-are-react-hooks-explain-usestate-and-useeffect)
11. [Rules of Hooks - what happens if you break them?](#q11-rules-of-hooks---what-happens-if-you-break-them)
12. [Why do we use keys in React lists?](#q12-why-do-we-use-keys-in-react-lists)
13. [What is prop drilling in React?](#q13-what-is-prop-drilling-in-react)
14. [What is the Context API and when would you use it?](#q14-what-is-the-context-api-and-when-would-you-use-it)
15. [Difference between `useEffect` and `useLayoutEffect`?](#q15-difference-between-useeffect-and-uselayouteffect)
16. [Controlled vs uncontrolled components](#q16-controlled-vs-uncontrolled-components)
17. [What Causes a React Component to Re-render?](#q17-what-causes-a-react-component-to-re-render)
18. [What is React.memo and how does it prevent unnecessary re-renders?](#q18-what-is-reactmemo-and-how-does-it-prevent-unnecessary-re-renders)
19. [Difference between useMemo and useCallback](#q19-difference-between-usememo-and-usecallback)
20. [What are higher-order components (HOCs)?](#q20-what-are-higher-order-components-hocs)
21. [Why does 0 && condition print 0 on screen during rendering?](#q21-why-does-0--condition-print-0-on-screen-during-rendering)
22. [What are error boundaries?](#q22-what-are-error-boundaries)
23. [Explain code splitting and lazy loading](#q23-explain-code-splitting-and-lazy-loading)

---

### **Q1: What is React, and how is it different from other frameworks?**

React is a JavaScript library developed by Facebook for building fast and interactive user interfaces using a component-based architecture. It uses a virtual DOM to efficiently update the UI and allows developers to create reusable components for scalable applications.

React is different because it is a library focused only on building the UI, while frameworks like Angular provide a complete solution including routing, state management, and form handling. React also uses a virtual DOM, which improves performance by updating only the necessary parts of the UI instead of re-rendering the entire page.

---

### **Q2: What are key features of React?**

**Key Features of React:**

- **Component-Based Architecture**
  - The UI is divided into independent, reusable pieces called components, making the code easier to manage and scale.
- **Virtual DOM**
  - React uses a lightweight representation of the real DOM to update only the parts of the page that actually change, which significantly boosts performance.
- **Declarative UI**
  - You describe what the UI should look like for any given state, and React handles the complex task of updating the DOM efficiently.
- **Reusable Components**
  - Because components are self-contained building blocks, they can be reused throughout the entire application, reducing development time.
- **Unidirectional Data Flow**
  - Data flows in a single direction (from parent to child via props), which makes debugging easier and the application state more predictable.

---

### **Q3: Explain the Virtual DOM and how it works?**

The Virtual DOM is a lightweight JavaScript representation of the real DOM. When the state of a React component changes, React creates a new Virtual DOM and compares it with the previous one using a diffing algorithm. It then updates only the changed parts in the real DOM, which improves performance.

---

### **Q4: What are components? Difference between functional and class components?**

Components are reusable and independent pieces of UI in React that help build applications by dividing the interface into smaller parts.

Functional components are simple JavaScript functions that return JSX and use React Hooks to manage state and lifecycle features. Class components are ES6 classes that extend React.Component and manage state using this.state and lifecycle methods. Today, functional components are preferred because they are simpler and support Hooks.

---

### **Q5: What are props and state? How are they different?**

Props are read-only data passed from a parent component to a child component, while state is data managed within a component that can change over time and trigger re-rendering.

---

### **Q6: Explain the component lifecycle**

The component lifecycle refers to the different phases a React component goes through from creation to removal. The three main phases are mounting (component is created and added to the DOM), updating (component re-renders when props or state change), and unmounting (component is removed from the DOM).

In React, these stages are called:

1. Mounting
2. Updating
3. Unmounting

---

### **Q7: What is JSX?**

JSX stands for JavaScript XML. It is a syntax extension used in React that allows developers to write HTML-like code inside JavaScript. React converts JSX into regular JavaScript using `React.createElement()`.

---

### **Q8: How do you handle events in React?**

In React, you handle events by assigning a function (event handler) to a specific, camel-cased prop on a JSX element. React uses a synthetic event system for consistent cross-browser behavior.

---

### **Q9: What is conditional rendering?**

Conditional rendering in React is the process of displaying different UI elements or components based on certain conditions (e.g., application state or props). It allows developers to create dynamic and interactive user interfaces using standard JavaScript logic.

---

### **Q10: What are React Hooks? Explain `useState` and `useEffect`**

React Hooks are functions that allow functional components to use state and lifecycle features. useState is used to manage state inside a component, while useEffect is used to perform side effects such as API calls, subscriptions, and DOM updates.

---

### **Q11: Rules of Hooks - what happens if you break them?**

React Hooks must follow two rules: they should only be called at the top level of a component and only inside React functional components or custom hooks. If these rules are broken, React may throw errors or cause incorrect state behavior because it relies on the order of hooks during rendering.

---

### **Q12: Why do we use keys in React lists?**

Keys are unique identifiers used by React to track elements in a list. They help React efficiently update the UI when items are added, removed, or reordered.

---

### **Q13: What is prop drilling in React?**

Prop drilling in React is the process of passing data (props) from a parent component down through multiple layers of nested components to reach a deeply nested component that actually needs the data.

---

### **Q14: What is the Context API and when would you use it?**

The Context API is a React feature that allows data to be shared across components without passing props manually through every level of the component tree.

---

### **Q15: Difference between `useEffect` and `useLayoutEffect`?**

`useEffect` runs after the browser paints the UI, while `useLayoutEffect` runs before the browser paints and blocks the rendering until it finishes.

---

### **Q16: Controlled vs uncontrolled components**

In controlled components, form data is handled by React state using `useState`. In uncontrolled components, form data is managed by the DOM and accessed using `useRef`.

---

### **Q17: What Causes a React Component to Re-render?**

A React component re-renders when its state changes, when its props change, when its parent component re-renders, or when the context value it consumes changes.

---

### **Q18: What is React.memo and how does it prevent unnecessary re-renders?**

React.memo is a higher-order component that prevents unnecessary re-rendering of a functional component by memoizing the result and re-rendering only when its props change.

---

### **Q19: Difference between useMemo and useCallback**

`useMemo` is used to memoize a computed value, while `useCallback` is used to memoize a function. Both are used for performance optimization to prevent unnecessary recalculations and re-renders.

---

### **Q20: What are higher-order components (HOCs)?**

A Higher-Order Component (HOC) is a function that takes a component as input and returns a new component with additional functionality.

---

### **Q21: Why does 0 && condition print 0 on screen during rendering?**

In JavaScript, `&&` returns the first falsy value. Since `0` is falsy but not ignored by React, it gets rendered on the screen instead of the component.

---

### **Q22: What are error boundaries?**

Error Boundaries are React components that catch JavaScript errors in their child components and display a fallback UI instead of crashing the entire application.

---

### **Q23: Explain code splitting and lazy loading**

Code splitting is the process of breaking a large JavaScript bundle into smaller chunks, and lazy loading is a technique where components are loaded only when they are needed using React.lazy and Suspense.
