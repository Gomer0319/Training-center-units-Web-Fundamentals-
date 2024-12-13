## Passing Values and Getting Results with Functions

### Developmental Outcomes
By the end of this lesson, students should be able to:
1. Understand how to pass values to functions using parameters.
2. Learn how to return values from a function to use its output.
3. Apply the concept of parameters and return values to make reusable and dynamic functions.

### What Are Parameters and Return Values?

Functions often need external values to perform their tasks. These values are provided using **parameters**. Once the function processes those values, it can send back a result using the **return** statement. This ability to pass data in and get results out makes functions more flexible and reusable.

### Parameters: Input for Functions

**Parameters** are placeholders for values that are passed to a function when it is called. The actual values provided when calling the function are called **arguments**.

#### Example of a Function with Parameters

```javascript
function greetUser(name) {
  console.log("Hello, " + name);
}

greetUser("Alice");
greetUser("Bob");
```

In this example, the function `greetUser` accepts a parameter `name`, and when different arguments like "Alice" or "Bob" are passed, the function outputs a personalized greeting.

### Return Values: Getting Results from Functions

A **return value** is the result a function sends back to the calling code. Not all functions have to return a value, but when they do, the `return` keyword is used. This allows the result to be stored or further processed.

#### Example of a Function with a Return Value

```javascript
function add(a, b) {
  return a + b;
}

let sum = add(5, 7);
console.log(sum);
```

Here, the function `add` returns the sum of two numbers, and the result is stored in the `sum` variable, which is then printed.

### Using Parameters and Return Together

When you combine parameters and return values, you can create functions that process data dynamically and return meaningful results.

#### Example

```javascript
function calculateArea(length, width) {
  return length * width;
}

let area = calculateArea(5, 10);
console.log(area);
```

In this example, the function `calculateArea` calculates the area of a rectangle and returns the result.

---

### Key Takeaways
- **Parameters** allow you to pass values to functions, making them more flexible.
- The **return** statement allows a function to send a result back to where it was called.
- By combining parameters and return values, you can build powerful functions that are reusable and dynamic.

Understanding parameters and return values is essential for writing flexible and efficient functions in JavaScript.