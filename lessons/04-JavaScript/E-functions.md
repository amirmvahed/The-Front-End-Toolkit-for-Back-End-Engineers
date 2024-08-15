# Functions in JavaScript

Functions are fundamental building blocks in JavaScript. They allow you to group code into reusable blocks that perform
specific tasks. Understanding how functions work will help you write modular, maintainable, and efficient code.

## Function Declarations

Function declarations define a named function that can be called from anywhere in the code, as long as it appears before
the call.

```js
function calculateSum(a, b) {
  return a + b;
}

let result = calculateSum(5, 3);  // Calling the function with arguments 5 and 3
console.log(result);             // Output: 8
```

* **`function calculateSum(a, b)`**: Declares a function named calculateSum with two parameters a and b.
* **`return a + b`**: The function returns the sum of a and b.

## Function Expressions

Function expressions define a function and assign it to a variable. This type of function is anonymous (i.e., it doesn't
have a name) but can be named if assigned to a variable.

```js
const multiply = function(x, y) {
  return x * y;
};

let result = multiply(4, 5);   // Calling the function with arguments 4 and 5
console.log(result);          // Output: 20
```

* **`const multiply = function(x, y)`**: Assigns an anonymous function to the variable multiply.
* **`return x * y`**: The function returns the product of x and y.

## Arrow Functions

Arrow functions provide a shorter syntax for writing function expressions. They are especially useful for simple
operations.

```js
const divide = (a, b) => a / b;

let result = divide(10, 2);   // Calling the function with arguments 10 and 2
console.log(result);         // Output: 5
```

* **`const divide = (a, b) => a / b`**: Defines an arrow function that divides a by b and returns the result.
* For functions with a single expression, the curly braces and return keyword can be omitted.
