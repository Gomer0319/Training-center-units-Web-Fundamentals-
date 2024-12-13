## Defining Functions: Declarations vs Expressions

### Developmental Outcomes
By the end of this lesson, students should be able to:
1. Understand the difference between function declarations and function expressions.
2. Identify the syntax and use cases of each.
3. Recognize the importance of function hoisting in JavaScript.

### What Are Function Declarations and Expressions?

In JavaScript, there are two main ways to define a function: using a **function declaration** or a **function expression**. Both achieve the same goal—defining a function—but they differ in how and when the function is available for use in your code.

### Function Declaration

A **function declaration** defines a named function using the `function` keyword. This is the most common way to define a function. One important characteristic of function declarations is **hoisting**—the function can be called before it is declared in the code.

#### Example of Function Declaration

```javascript
function sayHello() {
  console.log("Hello!");
}

sayHello();  // Output: "Hello!"
```

- **Function Name**: `sayHello`.
- **Availability**: Due to **hoisting**, you can call this function anywhere in the code, even before the declaration.

### Function Expression

A **function expression** defines a function as part of a larger expression, usually assigning it to a variable. Unlike declarations, function expressions are **not hoisted**. This means the function is only available after it is defined.

#### Example of Function Expression

```javascript
const sayHi = function() {
  console.log("Hi!");
};

sayHi();  // Output: "Hi!"
```

- **Function Name**: The function is anonymous but is assigned to the variable `sayHi`.
- **Availability**: The function is only available after the line where it’s defined. If you try to call it before its definition, you’ll get an error.

### Key Differences Between Declarations and Expressions

| Aspect                 | Function Declaration                | Function Expression                   |
|------------------------|-------------------------------------|---------------------------------------|
| **Definition**          | Named function using `function`.    | Can be anonymous or named, often assigned to a variable. |
| **Hoisting**            | Hoisted; can be called before declaration. | Not hoisted; can only be called after definition. |
| **Use Cases**           | General function definitions, especially when hoisting is needed. | Useful for defining functions as part of a larger statement or block. |

### Hoisting in JavaScript

Hoisting is JavaScript's behavior of moving function declarations to the top of their scope before code execution. This allows you to call declared functions anywhere in your code, even if the actual function definition appears later. However, hoisting does not apply to function expressions.

#### Example of Hoisting with Function Declaration

```javascript
sayGoodbye();

function sayGoodbye() {
  console.log("Goodbye!");
}
```

The code runs without issues because of hoisting, even though `sayGoodbye` is called before its definition.

---

### Key Takeaways
- A **function declaration** defines a named function and is hoisted, meaning it can be called anywhere in the code.
- A **function expression** is often anonymous, assigned to a variable, and is not hoisted.
- Understanding the difference between declarations and expressions is crucial for writing clear and predictable code.

Function declarations are best when you need flexibility with hoisting, while function expressions are useful for more controlled, block-level function definitions.