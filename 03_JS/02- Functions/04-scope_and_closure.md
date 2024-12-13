## Understanding Scope and Closures

### Developmental Outcomes
By the end of this lesson, students should be able to:
1. Understand the concept of scope in JavaScript, including global and local scopes.
2. Learn how closures work and how they retain access to variables in their parent scope.
3. Apply the knowledge of scope and closures to avoid common coding pitfalls.

### The Concept of Scope

**Scope** refers to the accessibility of variables in different parts of your code. JavaScript has two main types of scope:
- **Global scope**: Variables declared outside of any function or block are globally scoped, meaning they are accessible anywhere in the program.
- **Local scope**: Variables declared within a function or block are locally scoped, meaning they can only be accessed within that specific function or block.

#### Example of Global and Local Scope

```javascript
let globalVar = "I'm global!";

function testScope() {
  let localVar = "I'm local!";
  console.log(globalVar);  // Accessible
  console.log(localVar);   // Accessible
}

testScope();
// console.log(localVar);  // Error: localVar is not defined
```

In this example:
- `globalVar` is globally scoped and can be accessed both inside and outside the function.
- `localVar` is locally scoped and is only accessible within the `testScope` function.

### Closures: Functions Inside Functions

A **closure** is created when a function retains access to variables in its outer (parent) scope, even after the parent function has finished executing. Closures are useful for creating functions that "remember" values, even when called later in the program.

#### Example of a Closure

```javascript
function outerFunction(outerVar) {
  return function innerFunction(innerVar) {
    return outerVar + innerVar;
  };
}

const newFunction = outerFunction(10);
console.log(newFunction(5));  // Output: 15
```

In this example:
- `outerFunction` returns `innerFunction`, and `innerFunction` has access to `outerVar`, even after `outerFunction` has executed. This is a closure.

### Practical Uses of Closures

Closures are often used in:
1. **Callback functions**: When functions are passed as arguments to other functions, they retain access to their outer variables.
2. **Data encapsulation**: Closures allow you to create private variables that can only be accessed through specific functions, useful for securing data.
3. **Stateful functions**: You can store and update values across multiple function calls.

---

### Key Takeaways
- **Scope** determines where variables can be accessed in your code, with global scope being accessible everywhere and local scope limited to specific blocks or functions.
- **Closures** occur when a function retains access to its parent scope, allowing it to "remember" values even after the parent function has finished executing.
- Mastering scope and closures helps prevent common errors and allows for more advanced JavaScript patterns, like callbacks and data encapsulation.

Understanding these concepts is essential for writing clean, efficient, and powerful JavaScript code.