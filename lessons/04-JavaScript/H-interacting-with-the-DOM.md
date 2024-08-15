# Interacting with the DOM (Document Object Model)

## What is the DOM?

The DOM (Document Object Model) is a programming interface provided by the browser that allows JavaScript to interact
with the HTML and CSS of a webpage. It represents the structure of a webpage as a tree of objects, where each element in
the HTML document is a node in this tree. This model allows developers to programmatically manipulate web content,
style, and structure.

**Document:** The root of the DOM tree, representing the entire webpage.
**Elements:** Individual HTML elements (`<div>`, `<p>`, `<h1>`, etc.) are nodes in the DOM.

## Selecting Elements

Before you can manipulate an element, you need to select it from the DOM. JavaScript provides several methods for
selecting elements, each with its own use cases.

**1. getElementById:**
This method selects a single element based on its `id` attribute. Since IDs are unique within a page, this method
returns
one element.

```js
let element = document.getElementById('element-id');
```

**2. getElementsByClassName:**
This method selects all elements that share the same class name and returns an HTMLCollection (an array-like object).

```js
// Selecting all <p> (paragraph) elements on the page.
let paragraphs = document.getElementsByTagName("p");
```

**3. querySelector:**
This method selects the first element that matches a CSS selector. It’s versatile and can select elements based on ID,
class, tag name, or any complex CSS selector.

```js
let element = document.querySelector('selector');

// Selecting the first element with the class list-item.
let firstItem = document.querySelector('.list-item');
```

**4. querySelectorAll:**
This method selects all elements that match a CSS selector and returns a NodeList (a static collection of elements that
can be iterated over).

```js
// Selecting all elements with the class list-item.
let allItems = document.querySelectorAll('.list-item');
```

## Manipulating Content

Once you’ve selected an element, you can manipulate its content, and style.

**a. Changing Text Content:**
You can change the text content of an element using the `textContent`property.

```js
let title = document.getElementById("main-title");
title.textContent = "Welcome to My Web Page!";  // Changes the text content
```

The `textContent` property sets or returns the text content of the specified element.

**b. Changing HTML Content:**
You can change the inner HTML of an element using the `innerHTML` property.

```js
let content = document.getElementById('content');
content.innerHTML = "<p>This is a new paragraph!</p>";  // Changes the HTML content
```

The `innerHTML` property allows you to add or modify the HTML inside an element.

**c. Changing Styles:**
You can directly manipulate an element’s CSS styles using the `style` property.

```js
let header = document.querySelector('h1');
header.style.color = "blue";    // Changes the text color to blue
header.style.fontSize = "24px"; // Changes the font size to 24px
```

The `style` property allows you to set or return the inline style of an element.

## Creating and Removing Elements

JavaScript also allows you to create new elements and add them to the DOM or remove existing elements from the DOM.

**a. Creating New Elements:**
You can create a new element using `document.createElement` and add it to the DOM using a method like `appendChild`.

```js
let newParagraph = document.createElement('p');
newParagraph.textContent = "This is a dynamically added paragraph.";
document.body.appendChild(newParagraph);  // Adds the new paragraph to the end of the body
```

`createElement` creates a new element, and `appendChild` adds it to the DOM as the last child of the specified parent
element.

**b. Removing Elements:**
You can remove an element from the DOM using the removeChild or remove method.

```js
let paragraph = document.querySelector("p");
paragraph.remove();  // Removes the selected paragraph from the DOM
```

The `remove` method removes the selected element from the DOM.

## Manipulating Classes

Classes are essential for applying CSS styles. JavaScript provides methods to add, remove, and toggle CSS classes on
elements dynamically.

**a. Adding Classes:**
`classList.add` adds the specified class to the element's class list.

```js
let button = document.querySelector('.my-button');
button.classList.add('active');  // Adds the 'active' class to the button
```

**b. Removing Classes:**
`classList.remove` removes the specified class from the element's class list.

```js
let button = document.querySelector('.my-button');
button.classList.remove('inactive');  // Removes the 'inactive' class from the button
```

**c. Toggling Classes:**
Toggling a class means adding the class if it’s not already present, or removing it if it is.

```js
let button = document.querySelector('.my-button');
button.classList.toggle('highlight');  // Toggles the 'highlight' class on the button
```

`classList.toggle` adds the class if it doesn’t exist, or removes it if it does.
