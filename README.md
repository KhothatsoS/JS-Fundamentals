# JavaScript Programming Overview

## 📘 Why JavaScript Programming is Amazing
JavaScript is an essential language for web development. It allows developers to make websites interactive and dynamic. It runs in all major browsers, making it one of the most versatile and widely used languages. You can use JavaScript for **frontend, backend (Node.js), mobile apps**, and even **game development**.

---

## ▶️ How to Run a JavaScript Script
You can run JavaScript in several ways:
- **In the browser console:**  
  Open Developer Tools → Console → Type JavaScript code and press **Enter**.
- **In an HTML file:**  
  ```html
  <script>
    console.log("Hello, JavaScript!");
  </script>
- **Using Node.js:**
  Create a file named "script.js" in Node.js and run the code below in the terminal
  ```html
  node script.js ```
  
### 🧮 How to Create Variables and Constants
Variables store data values. You can create them using var, let, or const:
```html
let age = 25;
const name = "Khothatso";
var country = "South Africa";
```

### 🔁 Differences Between var, const, and let
| Keyword | Scope           | Reassignment | Redeclaration | Hoisted | Common Use                    |
| ------- | --------------- | ------------ | ------------- | ------- | ----------------------------- |
| `var`   | Function-scoped | ✅ Yes        | ✅ Yes         | ✅ Yes   | Legacy code                   |
| `let`   | Block-scoped    | ✅ Yes        | ❌ No          | ⚠️ No   | Modern variable declaration   |
| `const` | Block-scoped    | ❌ No         | ❌ No          | ⚠️ No   | For constants or fixed values |

## 🔢 Data Types in JavaScript
JavaScript has several data types divided into primitive and non-primitive.

### Primitive Types

- String – "Hello"
- Number – 42
- Boolean – true or false
- Undefined – declared but not assigned
- Null – intentional empty value
- Symbol – unique and immutable identifier
- BigInt – for very large numbers

### Non-Primitive Type
Object – collection of key-value pairs, including arrays and functions.

### ⚙️ How to Use if and if...else Statements
Conditional statements allow you to execute different code depending on conditions:
```html 
let age = 18;

if (age >= 18) {
  console.log("You are an adult");
} else {
  console.log("You are a minor");
}
```
### 💬 How to Use Comments

Comments help explain code and are ignored by the program.

#### Single-line comment:
```html
// this is a single line comment
```
#### Multi-line comment:
```html
/* this is a
multi-line comment
*/
```
### 🧠 How to Affect Values to Variables
You assign (or affect) values using the = operator:
```html
let x = 10;
x = 20; // reassign a new value
```
### 🔄 How to Use while and for Loops
Loops allow you to execute a block of code multiple times.

#### While loop:
```html
let i = 0;
while (i < 5) {
  console.log(i);
  i++;
}
```
#### For loop:
```html
for (let i = 0; i < 5; i++) {
  console.log(i);
}
```
### ⏹ How to Use break and continue Statements
- `break` → exits the loop completely.
- `continue` → skips the current iteration and moves to the next one.
Example:
```html
for (let i = 0; i < 5; i++) {
  if (i === 2) continue; // skips 2
  if (i === 4) break;    // stops loop
  console.log(i);
}
```
### 🧩 What is a Function and How to Use It
A function is a block of code designed to perform a task. It can take inputs (parameters) and return an output.

Example:
```html
function greet(name) {
  return `Hello, ${name}!`;
}
console.log(greet("Khothatso"));
```
### ❌ What Does a Function Without return Return?
If a function does not include a return statement, it automatically returns undefined.

Example:
```html
function sayHi() {
  console.log("Hi!");
}
let result = sayHi(); // prints "Hi!"
console.log(result);  // undefined
```
### 🌍 Scope of Variables
Scope defines where a variable can be accessed in your code.

- **Global Scope:** Accessible everywhere.
- **Function Scope:** Accessible only inside a function.
- **Block Scope:** Accessible only within {} when using let or const.

Example:
```html
let a = 10; // global

function test() {
  let b = 20; // function scope
  if (true) {
    let c = 30; // block scope
    console.log(a, b, c);
  }
}
test();
```
### ➕ Arithmetic Operators
Arithmetic operators are used for mathematical calculations.
| Operator | Description         | Example  | Result |
| -------- | ------------------- | -------- | ------ |
| `+`      | Addition            | `5 + 3`  | 8      |
| `-`      | Subtraction         | `5 - 3`  | 2      |
| `*`      | Multiplication      | `5 * 3`  | 15     |
| `/`      | Division            | `6 / 3`  | 2      |
| `%`      | Modulus (remainder) | `5 % 2`  | 1      |
| `**`     | Exponentiation      | `2 ** 3` | 8      |

### 📚 How to Manipulate a Dictionary (Object)
In JavaScript, a dictionary is known as an object — a collection of key-value pairs.
Example:
```html
let person = {
  name: "Khothatso",
  age: 25,
  country: "South Africa"
};

// Access a property
console.log(person.name);

// Add or modify a property
person.job = "Developer";
person.age = 26;

// Delete a property
delete person.country;

console.log(person);
```
### 📥 How to Import a File
You can import JavaScript files in different ways depending on the environment.
**In HTML**
```html
<script src="main.js"></script>
```
**In Node.js**
```html
const myModule = require('./myModule.js');
```
