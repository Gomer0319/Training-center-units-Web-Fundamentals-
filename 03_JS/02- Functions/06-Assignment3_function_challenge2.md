## JavaScript Functions: Problem-Solving Challenges 2

### Trainee Goal
1. Strengthen your understanding of function creation and execution in JavaScript.
2. Learn to work with nested functions, recursive functions, and advanced property extraction in objects.
3. Practice working with arrays and prime number logic.

### Duration
1 hour

### Difficulty
Advanced

---

### Instructions

1. Complete the following challenges by creating functions and demonstrating their usage. Save your work in a Markdown file (.md).  
2. **Submission**: Once completed, save your file as `first_last_function2.md`. Compress this file into a `.zip` folder and rename it to `first_last_function2.zip` before submitting.

### Challenge 11:
**Function Hoisting and Nested Function**  
Create a function `createMultiplier` that takes a number `n` as a parameter and returns another function. The returned function should take a parameter `x` and multiply it by `n`. Demonstrate how this works by calling the inner function.

```js
function createMultiplier(n) {
  // Your code here
}
```

Example usage:

```js
const double = createMultiplier(2);
console.log(double(5));  // Output: 10

const triple = createMultiplier(3);
console.log(triple(4));  // Output: 12
```

---

### Challenge 12:
**Recursive Function: Fibonacci Sequence**  
Write a recursive function `fibonacci` that takes a number `n` and returns the `n`-th number in the Fibonacci sequence. The Fibonacci sequence is defined as:

```
fib(0) = 0
fib(1) = 1
fib(n) = fib(n-1) + fib(n-2) (for n > 1)
```

```js
function fibonacci(n) {
  // Your code here
}
```

Example usage:

```js
console.log(fibonacci(6));  // Output: 8
```

---

### Challenge 13:
**Deep Object Property Extraction**  
Write a function `getNestedProperty` that takes an object and a "path" (a string of properties separated by dots, e.g., `"a.b.c"`) as parameters and returns the value at that path in the object. If the path doesn’t exist, return `undefined`.

```js
function getNestedProperty(obj, path) {
  // Your code here
}
```

Example usage:

```js
const data = { a: { b: { c: 42 } } };
console.log(getNestedProperty(data, 'a.b.c'));  // Output: 42
console.log(getNestedProperty(data, 'a.b.d'));  // Output: undefined
```

---

### Challenge 14:
**Prime Numbers within a Range**  
Create a function `findPrimes` that takes two numbers `start` and `end` as parameters and returns an array of all prime numbers between `start` and `end` (inclusive). A prime number is only divisible by 1 and itself.

```js
function findPrimes(start, end) {
  // Your code here
}
```

Example usage:

```js
console.log(findPrimes(10, 30));  // Output: [11, 13, 17, 19, 23, 29]
```

---

### Challenge 15:
**Flatten an Array of Arrays**  
Write a function `flattenArray` that takes an array of arrays (e.g., `[[1, 2], [3, 4], [5, 6]]`) as a parameter and returns a single array with all the elements (e.g., `[1, 2, 3, 4, 5, 6]`).

```js
function flattenArray(arr) {
  // Your code here
}
```

Example usage:

```js
console.log(flattenArray([[1, 2], [3, 4], [5, 6]]));  // Output: [1, 2, 3, 4, 5, 6]
```

---

### Bonus Task:
For an extra challenge, modify your `fibonacci` function to use memoization for performance improvement, especially when calculating larger Fibonacci numbers.

---

### Criteria for Success:
- Functions are correctly implemented and meet the challenge requirements.
- All test cases return the expected output.
- Nested function behavior, recursion, and object property extraction are handled correctly.
- The solution is correctly submitted as a `.md` file and compressed into a `.zip` file.

---

### Solutions

```js
// Challenge 11: Function Hoisting and Nested Function
function createMultiplier(n) {
  return function (x) {
    return x * n;
  };
}

// Usage example:
const double = createMultiplier(2);
console.log(double(5));  // Output: 10

const triple = createMultiplier(3);
console.log(triple(4));  // Output: 12
```

```js
// Challenge 12: Recursive Function: Fibonacci Sequence
function fibonacci(n) {
  if (n === 0) return 0;
  if (n === 1) return 1;
  return fibonacci(n - 1) + fibonacci(n - 2);
}

// Example usage:
console.log(fibonacci(6));  // Output: 8
```

```js
// Challenge 13: Deep Object Property Extraction
function getNestedProperty(obj, path) {
  return path.split('.').reduce((acc, key) => (acc && acc[key] !== undefined ? acc[key] : undefined), obj);
}

// Example usage:
const data = { a: { b: { c: 42 } } };
console.log(getNestedProperty(data, 'a.b.c'));  // Output: 42
console.log(getNestedProperty(data, 'a.b.d'));  // Output: undefined
```

```js
// Challenge 14: Prime Numbers within a Range
function findPrimes(start, end) {
  function isPrime(num) {
    if (num <= 1) return false;
    for (let i = 2; i < num; i++) {
      if (num % i === 0) return false;
    }
    return true;
  }
  
  const primes = [];
  for (let i = start; i <= end; i++) {
    if (isPrime(i)) primes.push(i);
  }
  return primes;
}

// Example usage:
console.log(findPrimes(10, 30));  // Output: [11, 13, 17, 19, 23, 29]
```

```js
// Challenge 15: Flatten an Array of Arrays
function flattenArray(arr) {
  return arr.reduce((flat, toFlatten) => flat.concat(toFlatten), []);
}

// Example usage:
console.log(flattenArray([[1, 2], [3, 4], [5, 6]]));  // Output: [1, 2, 3, 4, 5, 6]
```