# JavaScript Documentation

## Table of Contents
1. [What is JavaScript?](#what-is-javascript)
2. [Why is JavaScript Important?](#why-is-javascript-important)
3. [Variables and Data Types](#variables-and-data-types)
   - [Declaring Variables](#declaring-variables)
   - [Data Types](#data-types)
   - [Type Coercion](#type-coercion)
4. [Operators and Expressions](#operators-and-expressions)
   - [Arithmetic Operators](#arithmetic-operators)
   - [Comparison Operators](#comparison-operators)
   - [Logical Operators](#logical-operators)
   - [Assignment Operators](#assignment-operators)
   - [Expressions](#expressions)
5. [Functions and Scope](#functions-and-scope)
   - [Defining Functions](#defining-functions)
   - [Function Parameters and Return Values](#function-parameters-and-return-values)
   - [Scope in JavaScript](#scope-in-javascript)
   - [Closures](#closures)

## What is JavaScript?

JavaScript (often abbreviated as JS) is a high-level, interpreted programming language primarily used for adding interactivity to web pages. It was created by Brendan Eich in 1995 while he was working at Netscape.

JavaScript is one of the core technologies of the web, alongside HTML and CSS:
- **HTML** provides the structure of a webpage.
- **CSS** handles the styling and layout.
- **JavaScript** adds dynamic behavior, such as responding to user inputs, manipulating the DOM, and fetching data from servers.

### JavaScript Characteristics:
- **Interpreted**: Code is executed line-by-line by the JavaScript engine.
- **Client-Side**: Typically runs in the browser.
- **Versatile**: Can also run on the server-side using Node.js.
- **Event-Driven**: Handles user interactions like clicks and keystrokes.
- **Object-Oriented and Functional**: Supports multiple programming paradigms.

## Why is JavaScript Important?

JavaScript is a cornerstone of modern web development due to:

- **Interactivity on the Web**: Enables dynamic user experiences (e.g., form validation, animations, real-time updates).
- **Universal Browser Support**: Works across all major browsers.
- **Full-Stack Development**: With Node.js, JavaScript can be used on both frontend and backend.
- **Rich Ecosystem**: Extensive libraries and frameworks like React, Angular, and Vue.js.
- **Community and Adoption**: One of the most widely used programming languages worldwide.

## Variables and Data Types

### Declaring Variables
Variables store data and are declared using `var`, `let`, or `const`:

```javascript
var name = "Alice"; // Function-scoped
let age = 25; // Block-scoped
const pi = 3.14; // Constant value
```

### Data Types
JavaScript supports **primitive** and **non-primitive** data types:

#### Primitive Data Types:
- **Number**: `let num = 42;`
- **String**: `let greeting = "Hello";`
- **Boolean**: `let isActive = true;`
- **Undefined**: `let x; // undefined`
- **Null**: `let y = null;`
- **Symbol**: `let id = Symbol("id");`
- **BigInt**: `let bigNumber = 12345678901234567890n;`

#### Non-Primitive Data Types:
- **Object**: `let person = { name: "Alice", age: 25 };`
- **Array**: `let numbers = [1, 2, 3, 4];`
- **Function**:

```javascript
function sayHello() {
    return "Hello!";
}
```

### Type Coercion
JavaScript automatically converts data types in certain operations:

```javascript
console.log("5" + 3); // "53" (String Concatenation)
console.log("5" - 3); // 2 (String converted to Number)
```

## Operators and Expressions

### Arithmetic Operators
| Operator | Description | Example |
|----------|------------|---------|
| + | Addition | `5 + 3` → `8` |
| - | Subtraction | `5 - 3` → `2` |
| * | Multiplication | `5 * 3` → `15` |
| / | Division | `6 / 2` → `3` |
| % | Modulus | `7 % 3` → `1` |
| ** | Exponentiation | `2 ** 3` → `8` |

### Comparison Operators
| Operator | Description | Example |
|----------|------------|---------|
| == | Loose equality | `5 == "5"` → `true` |
| === | Strict equality | `5 === "5"` → `false` |
| > | Greater than | `5 > 3` → `true` |

### Logical Operators
```javascript
console.log(true && false); // false
console.log(true || false); // true
console.log(!true); // false
```

### Assignment Operators
```javascript
let num = 10;
num += 5; // num = 15
num *= 2; // num = 30
```

### Expressions
Expressions evaluate to a single value:
```javascript
let result = (5 + 3) * 2; // 16
```

## Functions and Scope

### Defining Functions
```javascript
function add(a, b) {
    return a + b;
}
```

Arrow Function:
```javascript
const multiply = (a, b) => a * b;
```

### Function Parameters and Return Values
```javascript
function greet(name) {
    return `Hello, ${name}!`;
}
console.log(greet("Alice"));
```

### Scope in JavaScript

#### Global Scope
```javascript
let globalVar = "I'm global!";
function checkScope() {
    console.log(globalVar);
}
```

#### Function Scope
```javascript
function testFunctionScope() {
    var localVar = "I'm local!";
    console.log(localVar);
}
```

#### Block Scope (ES6)
```javascript
if (true) {
    let blockVar = "I'm block-scoped!";
}
```

### Closures
Closures retain access to variables even after the outer function executes:
```javascript
function outerFunction() {
    let outerVar = "I'm from outer!";
    return function innerFunction() {
        console.log(outerVar);
    };
}

const closure = outerFunction();
closure();
```

Closures are useful for:
- **Data Privacy** (creating private variables)
- **Event Handlers** (maintaining state across events)

## Conclusion
This documentation covers JavaScript fundamentals, including variables, data types, operators, functions, and scope. JavaScript is essential for web development and supports both client-side and server-side programming. For further learning, explore advanced topics like asynchronous programming, the DOM, and frameworks like React and Node.js.

