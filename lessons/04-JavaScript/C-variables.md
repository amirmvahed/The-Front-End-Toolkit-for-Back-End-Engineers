# Variables

Variables are fundamental to programming. In JavaScript, variables act like containers that store data values. Imagine
them as labeled boxes in which you can keep different pieces of information, whether that’s a number, a string of text,
or more complex data types. This allows you to store, manipulate, and reuse data throughout your code.

## Declaring Variables

To declare a variable in JavaScript, you can use `var`, `let`, or `const`. Each of these keywords has its specific use
cases:

1. **`var`:** This is the traditional way to declare variables. However, it's less commonly used in modern JavaScript
   because it has some quirks regarding scope and hoisting.
2. **`let`:** Introduced in ES6 (ECMAScript 2015), `let` is now the preferred way to declare variables that might change
   their
   value over time. It has block-level scope, meaning it's only accessible within the block where it’s defined.
3. **`const`:** Also introduced in ES6, `const` is used to declare variables that shouldn’t change. Once you assign a
   value
   to a const variable, it can’t be reassigned.

```js
var myVar = "Hello, world!"; // Using var
let myLet = 42;              // Using let
const myConst = 3.14;        // Using const
```

* **myVar:** This variable is declared with var and can be updated or redeclared within its scope.
* **myLet:** This variable is declared with let and can be updated but not redeclared within the same scope.
* **myConst:** This variable is declared with const and cannot be updated or redeclared.

## Variable Scope

Scope refers to where a variable is accessible within your code. There are mainly two types of scope in JavaScript:

1. **Global Scope:** If you declare a variable outside any function, it’s in the global scope and can be accessed
   anywhere in your code.
2. **Local (Block) Scope:** If you declare a variable inside a function, it’s only accessible within that function or
   block.

```js
let globalVar = "I am global";

function myFunction() {
  let localVar = "I am local";
  console.log(globalVar);  // Accessible
  console.log(localVar);   // Accessible
}

myFunction();

console.log(globalVar);  // Accessible
console.log(localVar);   // Error: localVar is not defined
```

In this example, `globalVar` is accessible everywhere, but `localVar` only exists within myFunction.

## Variable Naming Rules
When naming your variables, follow these guidelines:

* Names can contain letters, digits, underscores (_), and dollar signs ($).
* Names must begin with a letter, underscore, or dollar sign.
* Names are case-sensitive (myVar and myvar are different).
* Names cannot be reserved keywords (e.g., let, class, return, function).

## Best Practices for Variable Naming

* **Use descriptive names:** Instead of x, y, or z, use names like userName, totalAmount, or isComplete.
* **Camel case convention:** Start with a lowercase letter and capitalize subsequent words, e.g., userScore or firstName.
* **Avoid short, unclear names:** Short names like a, b, or c should be avoided unless in loops or very limited contexts.