# Conditional Statements in JavaScript

JavaScript provides several types of conditional statements, including if, else and
ternary operators (`condition ? expressionIfTrue : expressionIfFalse`)

## if, else

```js
let score = 85;

if (score >= 90) {
  console.log("Grade: A");
} else if (score >= 80) {
  console.log("Grade: B");
} else if (score >= 70) {
  console.log("Grade: C");
} else {
  console.log("Grade: F");
}
```

The code evaluates multiple conditions in sequence. It checks if score is 90 or higher, then 80 or higher, and so on,
assigning a grade based on the range the score falls into.

## The Ternary Operator

The ternary operator is a shorthand way to write simple if-else statements. It is often used to assign a value to a
variable based on a condition.

* condition ? expressionIfTrue : expressionIfFalse

```js
let age = 20;
let canVote = age >= 18 ? "Yes" : "No";
console.log(canVote);  // Output: Yes
```

The ternary operator checks if age is greater than or equal to 18. If true, it assigns "Yes" to canVote; otherwise, it
assigns "No".

## && (AND) Operator

The `&&` operator checks if both conditions are true.

```js
let age = 25;
let hasLicense = true;

if (age >= 18 && hasLicense) {
  console.log("You can drive.");
}
```

The message "You can drive" is printed only if both age is 18 or older and hasLicense is true.

## || (OR) Operator

The `||` operator checks if at least one of the conditions is true.

```js
let isWeekend = true;
let isHoliday = false;

if (isWeekend || isHoliday) {
  console.log("You can relax today.");
}
```

The message "You can relax today" is printed if either isWeekend or isHoliday is true.

## `!` (NOT) Operator

The `!` operator inverts a condition, making true become false and vice versa.

```js
let isRaining = false;

if (!isRaining) {
  console.log("You don't need an umbrella.");
}
```

The message "You don't need an umbrella" is printed if isRaining is false (because !isRaining is true).
