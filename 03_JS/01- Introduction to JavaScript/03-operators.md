## Uncovering JavaScript Operators

### Developmental Outcomes
By the end of this lesson, students should be able to:
1. Understand the role of operators in JavaScript for performing various operations.
2. Identify and apply different types of JavaScript operators, such as arithmetic, comparison, logical, and assignment operators.
3. Use operators effectively to manipulate and evaluate data in JavaScript programs.

### What Are JavaScript Operators?

Operators in JavaScript are symbols used to perform specific tasks on data values (operands). They are essential for making calculations, comparing values, and controlling the flow of your program. JavaScript provides various operators to handle different operations such as arithmetic, comparison, logical, and assignment.

### Types of JavaScript Operators

#### 1. **Arithmetic Operators**

Used for performing mathematical calculations.

- **Addition (`+`)**: Adds two numbers together.
  ```javascript
  let sum = 5 + 3;
  ```

- **Subtraction (`-`)**: Subtracts the second number from the first.
  ```javascript
  let difference = 10 - 4;
  ```

- **Multiplication (`*`)**: Multiplies two numbers.
  ```javascript
  let product = 6 * 2;
  ```

- **Division (`/`)**: Divides the first number by the second.
  ```javascript
  let quotient = 20 / 4;
  ```

- **Modulus (`%`)**: Returns the remainder when one number is divided by another.
  ```javascript
  let remainder = 9 % 4;
  ```

#### 2. **Comparison Operators**

Used to compare two values and return a boolean (`true` or `false`).

- **Equal to (`==`)**: Checks if two values are equal, ignoring their data type.
  ```javascript
  let isEqual = 5 == "5"; // true
  ```

- **Strict equal to (`===`)**: Checks if two values and their data types are equal.
  ```javascript
  let isStrictEqual = 5 === "5"; // false
  ```

- **Not equal (`!=`)**: Checks if two values are not equal.
  ```javascript
  let notEqual = 5 != 3;
  ```

- **Greater than (`>`)**: Checks if the first value is greater than the second.
  ```javascript
  let isGreater = 7 > 5;
  ```

- **Less than (`<`)**: Checks if the first value is less than the second.
  ```javascript
  let isLess = 2 < 4;
  ```

#### 3. **Logical Operators**

Used to combine multiple conditions or negate them.

- **AND (`&&`)**: Returns `true` if both conditions are true.
  ```javascript
  let result = (5 > 2) && (10 > 5);
  ```

- **OR (`||`)**: Returns `true` if at least one condition is true.
  ```javascript
  let result = (5 > 2) || (10 < 5);
  ```

- **NOT (`!`)**: Negates the logical value of its operand (true becomes false, and vice versa).
  ```javascript
  let isFalse = !(5 > 10);
  ```

#### 4. **Assignment Operators**

Used to assign values to variables.

- **Equal (`=`)**: Assigns a value to a variable.
  ```javascript
  let x = 10;
  ```

- **Add and Assign (`+=`)**: Adds a value to a variable and assigns the result to the variable.
  ```javascript
  let x = 5;
  x += 3; // x becomes 8
  ```

- **Subtract and Assign (`-=`)**: Subtracts a value from a variable and assigns the result to the variable.
  ```javascript
  let x = 10;
  x -= 2; // x becomes 8
  ```

---

### Key Takeaways
- Operators in JavaScript are symbols that enable you to perform calculations, compare values, and assign data to variables.
- JavaScript provides arithmetic operators for math operations, comparison operators for evaluating expressions, logical operators for combining conditions, and assignment operators for storing values.
- Mastering operators is key to controlling the flow of data and logic in your JavaScript programs.

These operators serve as essential building blocks for developing more complex programs.