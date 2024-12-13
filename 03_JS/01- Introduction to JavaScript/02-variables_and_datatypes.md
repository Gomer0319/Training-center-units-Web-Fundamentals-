## Demystifying JavaScript Variables and Data Types

### Developmental Outcomes
By the end of this lesson, students should be able to:
1. Define and declare variables in JavaScript.
2. Identify and differentiate between various data types in JavaScript.
3. Understand how to use variables and data types effectively in programming.

### What Are JavaScript Variables?

In JavaScript, variables are used to store data values. They act as containers for data that can be changed during the execution of a program. Variables are essential because they allow developers to reference and manipulate data dynamically.

#### Declaring Variables

You can declare variables in JavaScript using three keywords: `var`, `let`, and `const`.

- **`var`**: Declares a variable that can be re-assigned. It has function scope or global scope, depending on where it is declared.
- **`let`**: Declares a block-scoped variable that can also be re-assigned. It is preferred over `var` for modern JavaScript development.
- **`const`**: Declares a block-scoped variable that cannot be re-assigned. It is used for constants that should not change.

- **Example:**
  ```javascript
  var name = "Alice";
  let age = 25;
  const pi = 3.14;
  ```

### Understanding JavaScript Data Types

JavaScript has several built-in data types that define the kind of data that can be stored in a variable. The main data types include:

1. **Primitive Data Types**:
   - **String**: Represents a sequence of characters. Strings are enclosed in quotes.
     - **Example:**
       ```javascript
       let greeting = "Hello, World!";
       ```
   - **Number**: Represents numeric values, both integers and floating-point numbers.
     - **Example:**
       ```javascript
       let count = 10;
       let price = 99.99;
       ```
   - **Boolean**: Represents a logical entity and can be either `true` or `false`.
     - **Example:**
       ```javascript
       let isAvailable = true;
       ```
   - **Null**: Represents an intentional absence of any object value. It is assigned explicitly.
     - **Example:**
       ```javascript
       let user = null;
       ```
   - **Undefined**: Represents a variable that has been declared but not assigned a value.
     - **Example:**
       ```javascript
       let result;
       ```

2. **Complex Data Types**:
   - **Object**: A collection of key-value pairs. Objects can store multiple values and can be modified.
     - **Example:**
       ```javascript
       let person = {
           name: "Alice",
           age: 25
       };
       ```
   - **Array**: A special type of object used for storing ordered collections of values. Arrays can hold items of different types.
     - **Example:**
       ```javascript
       let scores = [90, 85, 88];
       ```

---

### Key Takeaways
- Variables are containers for storing data that can be manipulated in JavaScript.
- The three keywords for declaring variables are `var`, `let`, and `const`, each with its own scope and re-assignment rules.
- JavaScript has several data types, including strings, numbers, booleans, null, undefined, objects, and arrays, each serving different purposes.

Understanding variables and data types is fundamental for effective programming in JavaScript, enabling students to create dynamic and interactive web applications.