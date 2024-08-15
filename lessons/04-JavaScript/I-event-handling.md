# Event Handling in JavaScript

Handling events in JavaScript is a crucial aspect of creating interactive and dynamic web pages. Events are actions or
occurrences that happen in the browser, such as clicking a button, typing in a form field, or hovering over an image.
JavaScript allows you to respond to these events by executing specific code when they occur. This is achieved through
event listeners.

## What are Events?

An event in JavaScript is anything that happens in the browser, usually triggered by user interaction or the browser
itself. Common events include:

* **click:** When an element is clicked.
* **mouseover:** When the mouse pointer is moved over an element.
* **keydown:** When a key is pressed on the keyboard.
* **submit:** When a form is submitted.
* **load:** When the browser has finished loading a page.

Each event has a corresponding event type, and JavaScript allows you to "listen" for these events and respond
accordingly.

## Adding Event Listeners

Event listeners are used to attach specific code (also known as event handlers) to an event on an element. When the
event occurs, the attached event handler is executed.

```js
let button = document.querySelector(".my-button");

button.addEventListener("click", function() {
  alert("Button was clicked!");
});
```

This code selects a button element with the class my-button and attaches a click event listener to it. When the button
is clicked, an alert box with the message "Button was clicked!" will appear.

## Commonly Used Events

**a. Click Event:**
The `click` event is one of the most frequently used events. It occurs when a user clicks on an element, such as a
button or a link.

```js
let button = document.querySelector(".my-button");

button.addEventListener("click", function() {
  console.log("Button clicked!");
});
```

When the button is clicked, the message "Button clicked!" is logged to the console.

**b. Mouseover Event:**
The `mouseover` event occurs when the mouse pointer is moved over an element.

```js
let image = document.querySelector('.my-image');

image.addEventListener('mouseover', function() {
  image.style.border = '2px solid red';
});
```

When the mouse pointer hovers over the image, a red border is added to the image.

**c. Keydown Event:**
The `keydown` event occurs when a key is pressed down.

```js
document.addEventListener("keydown", function(event) {
  console.log("Key pressed:", event.key);
});
```

When any key is pressed, the key's value is logged to the console. The event.key property gives you the value of the key
that was pressed.

**c. Submit Event:**
The submit event occurs when a form is submitted. It's commonly used to validate form data before submission.

```js
let form = document.querySelector("form");

form.addEventListener("submit", function(event) {
  event.preventDefault();  // Prevent the form from submitting
  console.log("Form submitted!");
});
```

When the form is submitted, the event listener prevents the default submission behavior and logs "Form submitted!" to
the console. The event.preventDefault() method stops the form from actually submitting, which is useful for validating
the form data before submission.
