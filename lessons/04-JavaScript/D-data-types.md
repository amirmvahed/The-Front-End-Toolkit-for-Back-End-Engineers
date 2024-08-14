# Data Types

JavaScript is a **dynamically typed** language, meaning you don't have to specify the data type of a variable when you
declare it. The data type is determined automatically based on the value assigned to the variable.

JavaScript has several basic data types that you’ll use frequently:

## String

Represents text data. Strings are sequences of characters enclosed in single quotes ('), double quotes ("), or
backticks (`).

```js
let greeting = "Hello, world!";
let anotherGreeting = "Hi there!";
let templateString = `Today is ${new Date().toDateString()}`;
```

## Number

Represents numeric data, including integers and floating-point numbers (decimals).

```js
let age = 25;       // Integer
let price = 19.99;  // Floating-point number
let largeNumber = 1e6; // Exponential notation (1 million)
```

## Boolean

Represents a logical value and can be either `true` or `false`. Booleans are typically used in conditions and loops to
control the flow of your program.

```js
let isLoggedIn = true;
let hasPermission = false;
```

## Undefined

A variable that has been declared but not assigned a value has the type `undefined`.

```js
let notAssigned;
console.log(notAssigned); // Output: undefined
```

## Null

Represents the intentional absence of any object value. It is often used to indicate that a variable should be empty.

```js
let emptyValue = null;
```

> **Undefined vs. Null:**
>
> **Undefined:** When a variable is declared but not assigned a value, it has the value undefined.
>
> **Null:** Null is an assignment value that represents "no value" or "nothing."

## Object

Objects are complex data types that can store collections of data and more complex entities. Arrays, functions, and
other objects are also considered objects in JavaScript.

```js
let person = {
  name: "Amir",
  age: 30,
  isEmployed: true
};
```

## Array

Arrays are special types of objects used to store multiple values in a single variable. Each item in an array is called
an element, and it is accessed by its index (position) within the array, starting from 0.

```js
let colors = ["Red", "Green", "Blue"];
console.log(colors[0]); // Output: "Red"
console.log(colors[2]); // Output: "Blue"
```

Some useful methods for Arrays:

**Adding elements:** You can add elements to an array using the push method (adds to the end) or unshift (adds to the
beginning).

```js
colors.push("Yellow"); // Adds "Yellow" to the end
colors.unshift("Purple"); // Adds "Purple" to the beginning
```

**Removing elements:** You can remove elements using the pop method (removes from the end) or shift (removes from the
beginning).

```js
colors.pop(); // Removes the last element ("Yellow")
colors.shift(); // Removes the first element ("Purple")
```

**Looping through an array:** You can loop through the elements of an array using a for loop or the more modern forEach
method.

```js
// Using a for loop
for (let i = 0; i < colors.length; i++) {
  console.log(colors[i]);
}

// Using forEach
colors.forEach(color => console.log(color));
```

**Checking the length:** The length property returns the number of elements in an array.

```js
console.log(colors.length); // Output: 3
```
