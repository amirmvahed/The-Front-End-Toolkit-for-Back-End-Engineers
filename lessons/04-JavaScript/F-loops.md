# Loops in JavaScript

JavaScript provides several types of loops, each with its own use cases. The most commonly used loops are for, while,
and do...while. Additionally, there are special loops like for...in and for...of for iterating over objects and arrays.

## The `for` Loop

The for loop is one of the most commonly used loops in JavaScript. It runs a block of code a specific number of times,
based on a condition.

```js
let fruits = ["apple", "banana", "orange"];

for (let i = 0; i < fruits.length; i++) {
  console.log(fruits[i]);
}
```

This loop iterates over the fruits array and prints each fruit name.

**Common Use Case:** Iterating Over Arrays

## The `while` Loop

The while loop runs as long as a specified condition is true. It is useful when the number of iterations is not known
ahead of time.

```js
let i = 0;

while (i < 5) {
  console.log("Iteration number: " + i);
  i++;
}
```

* The loop continues running as long as this condition is true
* This loop behaves similarly to the for loop example above, but here the loop counter i is defined outside the loop and
  incremented manually inside the loop.

## The `for...in` Loop

The for...in loop is used to iterate over the properties of an object. It is primarily used for objects rather than
arrays.

```js
let user = {
  name: "Amir",
  city: "Tehran"
};

for (let key in user) {
  console.log(key + ": " + user[key]);
}
```

* **Key:** Represents the property name (or key) of the object.
* This loop iterates over the properties of the user object and prints each property name and its corresponding value.

## The `for...of` Loop

The for...of loop is used to iterate over iterable objects like arrays, strings, and more. It is often preferred over
the for loop for arrays because it is simpler and avoids off-by-one errors.

```js
let fruits = ["apple", "banana", "orange"];

// element
for (let fruit of fruits) {
  console.log(fruit);
}
```

* **Element:** Represents the current element in the iterable (e.g., array).
* This loop iterates over the fruits array and prints each fruit name. It is more concise and easier to read than a
  traditional for loop.

## The `forEach` method

The forEach method executes a provided function once for each array element. This method takes a callback function as an
argument, and this callback function is executed with each element in the array, one at a time.

```js
let fruits = ['apple', 'banana', 'orange'];

fruits.forEach(function(fruit) {
  console.log(fruit);
});
```

* The forEach method iterates through the fruits array, and for each element, it calls the provided function, printing
  the element to the console.
