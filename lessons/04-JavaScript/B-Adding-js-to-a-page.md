# Adding JavaScript to a Web Page

JavaScript can be added to a web page in three main ways:

1. **Inline JavaScript:** Placing JavaScript code directly within HTML tags.
2. **Internal JavaScript:** Writing JavaScript inside a `<script>` tag within the HTML document.
3. **External JavaScript:** Linking to an external JavaScript file using the `<script>` tag.

> For maintainability and best practices, we usually use **external JavaScript** files.

## Linking an External JavaScript File

**`<script src="script.js" defer></script>`:** This line links to an external JavaScript file named script.js. The defer
attribute ensures that the script is executed after the HTML document has been fully parsed.

**index.html:**
```html
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>My Web Page</title>
  <script src="script.js" defer></script>
</head>
<body>
<h1>Welcome to My Web Page</h1>
</body>
</html>
```

**script.js:**
```js
console.log("Hey Guys");
```