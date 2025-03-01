# Introduction to JavaScript

**Objective**: Understand the fundamentals of JavaScript and learn how to manipulate web pages dynamically.

**Date**: March 01, 2025  
**Instructor**: 

---

## 1. What is JavaScript? Why is it Important?

### Overview
- **Definition**: JavaScript is a high-level, interpreted programming language that adds interactivity to web pages. It’s executed by browsers like Chrome, Firefox, and Safari.
- **Core Role**: Alongside HTML (structure) and CSS (style), JavaScript provides behavior—think clicking buttons, submitting forms, or updating content live.
- **History**: Created in 1995 by Brendan Eich at Netscape in just 10 days. Originally named "Mocha," then "LiveScript," and finally "JavaScript." Today, it’s standardized as ECMAScript (ES6, ES11, etc.).
- **Why It Matters**:
  - Powers modern web apps: Gmail, Google Maps, Spotify.
  - Client-side execution: Runs in the browser, reducing server load.
  - Versatile: With Node.js, it’s used for backend development too.

### Key Takeaway
JavaScript is the engine of web interactivity—without it, websites would be static and lifeless.

---

## 2. Variables and Data Types

### Variables
- **Purpose**: Store data for use in your program.
- **Declaration Options**:
  - `var`: Function-scoped, hoisted, older style (e.g., `var x = 5;`).
  - `let`: Block-scoped, reassignable, preferred for modern JS (e.g., `let y = 10;`).
  - `const`: Block-scoped, constant value (e.g., `const z = 15;`), though object properties can still change.
- **Example**:
  ```javascript
  let name = "Alice";
  const age = 25;
  name = "Bob"; // Works
  // age = 26; // Error: Assignment to constant

## Data Types
# Primitive Types:
- string: Text, e.g., "Hello" or 'World'.
- number: Integers or decimals, e.g., 42, 3.14.
- boolean: true or false.
- undefined: Variable declared but not assigned.
- null: Intentional absence of value.
- symbol: Unique identifiers (ES6+), e.g., Symbol("id").
- bigint: Large integers, e.g., 123n.
- Complex Types:
- object: Key-value pairs, e.g., { name: "Alice", age: 25 }.
- array: Ordered list, e.g., [1, 2, 3].

- let str = "JavaScript";
- let num = 100;
- let obj = { course: "JS Intro", duration: "2 hours" };
- console.log(typeof str); // "string"

## Key Takeaway
Variables are how you store and manage data; choosing the right type and declaration method prevents bugs.

## 3. Operators and Expressions
# Operators
- Arithmetic: + (add), - (subtract), * (multiply), / (divide), % (remainder).
- Example: 5 + 3 = 8, 10 % 3 = 1.
- Comparison: Compare values.
- ==: Loose equality (converts types), e.g., "5" == 5 is true.
- ===: Strict equality (no conversion), e.g., "5" === 5 is false.
!=, !==, >, <, >=, <=.
# Logical: Combine conditions.
- && (and): Both true.
- || (or): Either true.
- ! (not): Inverts, e.g., !true = false.
## Expressions
# Definition: Code that evaluates to a value.
# Examples:
- 5 * 2 → 10.
- x > 0 && y < 10 → true or false.
