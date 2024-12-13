## JavaScript Functions: Problem-Solving Challenges

### Trainee Goal
1. Write and test JavaScript functions to solve a variety of common problems.
2. Practice working with parameters, return values, loops, and conditionals.
3. Strengthen understanding of basic algorithmic logic.

### Duration
45 minutes to 1 hour

### Difficulty
Intermediate

---

### Instructions

In this task, you’ll create 10 JavaScript functions to solve different coding challenges. Write your solutions in a Markdown (.md) file and save the file as `first_last_function1.md`. Compress the file into a `.zip` folder, renaming it to `first_last_function1.zip` before submission.

#### Challenge 1: Create a Function to Find Maximum Value
Write a function `findMax` that takes three numbers as parameters and returns the largest among them using comparison operators.

```js
function findMax(a, b, c) {
  // Your code here
}
```

#### Challenge 2: Reversing a String
Create a function `reverseString` that takes a string as a parameter and returns the reversed version without using array methods like `.reverse()`.

```js
function reverseString(str) {
  // Your code here
}
```

#### Challenge 3: Odd or Even Function
Write a function `isEven` that takes a number as a parameter and returns `true` if it’s even, and `false` if it’s odd.

```js
function isEven(num) {
  // Your code here
}
```

#### Challenge 4: Summing an Array
Create a function `sumArray` that takes an array of numbers and returns the sum of all elements.

```js
function sumArray(numbers) {
  // Your code here
}
```

#### Challenge 5: Convert Celsius to Fahrenheit
Write a function `convertToFahrenheit` that converts Celsius to Fahrenheit using the formula: `F = (C * 9/5) + 32`.

```js
function convertToFahrenheit(celsius) {
  // Your code here
}
```

#### Challenge 6: Factorial of a Number
Create a function `factorial` that returns the factorial of a number. For example, `factorial(5)` returns `120`.

```js
function factorial(n) {
  // Your code here
}
```

#### Challenge 7: Check for Palindrome
Write a function `isPalindrome` that checks if a given string is a palindrome (reads the same backward and forward).

```js
function isPalindrome(word) {
  // Your code here
}
```

#### Challenge 8: Grade Calculator
Create a function `calculateGrade` that takes a number (0-100) and returns the letter grade based on the scale provided.

```js
function calculateGrade(score) {
  // Your code here
}
```

#### Challenge 9: Count Vowels in a String
Write a function `countVowels` that returns the number of vowels (a, e, i, o, u) in a string.

```js
function countVowels(str) {
  // Your code here
}
```

#### Challenge 10: Shopping Cart Total
Create a function `cartTotal` that takes an array of item prices and returns the total price. Apply a 10% discount if the total exceeds $100.

```js
function cartTotal(prices) {
  // Your code here
}
```

### Bonus Task
Refactor some of your functions to handle edge cases or input validation where applicable. For example, modify `isPalindrome` to handle case sensitivity and spaces in the string.

---

### Criteria for Success
- Each function is correctly implemented with proper syntax.
- Functions return the expected results based on the problem requirements.
- The bonus task shows thoughtful improvements in handling edge cases.
- The file is correctly named as `first_last_function1.md`, compressed into `first_last_function1.zip`, and submitted successfully.

---

## JavaScript Functions: Solutions

#### Challenge 1: Create a Function to Find Maximum Value

```js
function findMax(a, b, c) {
  if (a >= b && a >= c) {
    return a;
  } else if (b >= a && b >= c) {
    return b;
  } else {
    return c;
  }
}
```

#### Challenge 2: Reversing a String

```js
function reverseString(str) {
  let reversed = '';
  for (let i = str.length - 1; i >= 0; i--) {
    reversed += str[i];
  }
  return reversed;
}
```

#### Challenge 3: Odd or Even Function

```js
function isEven(num) {
  return num % 2 === 0;
}
```

#### Challenge 4: Summing an Array

```js
function sumArray(numbers) {
  let sum = 0;
  for (let i = 0; i < numbers.length; i++) {
    sum += numbers[i];
  }
  return sum;
}
```

#### Challenge 5: Convert Celsius to Fahrenheit

```js
function convertToFahrenheit(celsius) {
  return (celsius * 9/5) + 32;
}
```

#### Challenge 6: Factorial of a Number

```js
function factorial(n) {
  let result = 1;
  for (let i = 1; i <= n; i++) {
    result *= i;
  }
  return result;
}
```

#### Challenge 7: Check for Palindrome

```js
function isPalindrome(word) {
  let normalizedWord = word.toLowerCase().replace(/\s+/g, '');
  let reversedWord = '';
  for (let i = normalizedWord.length - 1; i >= 0; i--) {
    reversedWord += normalizedWord[i];
  }
  return normalizedWord === reversedWord;

  if (normalizedWord === reversedWord) {
    console.log('The word ${word} is a palindrome');
    return true;
  } else {
    console.log('The word ${word} is not a palindrome');
    return false;
  }
}
```

#### Challenge 8: Grade Calculator

```js
function calculateGrade(score) {
  if (score >= 90) {
    return 'A';
  } else if (score >= 80) {
    return 'B';
  } else if (score >= 70) {
    return 'C';
  } else if (score >= 60) {
    return 'D';
  } else {
    return 'F';
  }
}
```

#### Challenge 9: Count Vowels in a String

```js
function countVowels(str) {
  let count = 0;
  let vowels = 'aeiouAEIOU';
  for (let i = 0; i < str.length; i++) {
    if (vowels.includes(str[i])) {
      count++;
    }
  }
  return count;
}
```

#### Challenge 10: Shopping Cart Total

```js
function cartTotal(prices) {
  let total = 0;
  for (let i = 0; i < prices.length; i++) {
    total += prices[i];
  }
  if (total > 100) {
    total *= 0.9; // Apply 10% discount
  }
  return total;
}
```

---

### Bonus Task Solution (Edge Case Handling for `isPalindrome`)

Here’s how we can improve the `isPalindrome` function to ignore case and spaces:

```js
function isPalindrome(word) {
  let normalizedWord = word.toLowerCase().replace(/[^a-zA-Z0-9]/g, '');
  let reversedWord = '';
  for (let i = normalizedWord.length - 1; i >= 0; i--) {
    reversedWord += normalizedWord[i];
  }
  return normalizedWord === reversedWord;
}
```

This version removes all non-alphanumeric characters and converts the string to lowercase before checking for palindrome status.
