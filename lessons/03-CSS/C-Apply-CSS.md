# How to Apply CSS to HTML

## Inline CSS

Inline CSS is applied directly to HTML elements using the style attribute. This method is useful for quick, one-off
styles that you want to apply to a specific element without affecting the rest of the page.

Example:

  ```html
<p style="color: red; font-size: 18px;">This paragraph is styled using inline CSS.</p>
  ```

## Internal CSS

Internal CSS is applied within the `<style>` tag inside the <head> section of your HTML document. This method is great for
styling a single page without affecting other pages.

Example:

 ```html
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>My Portfolio</title>
  <style>
    body {
      font-family: Arial, sans-serif;
    }

    h1 {
      color: blue;
    }

    p {
      color: gray;
      font-size: 16px;
    }
  </style>
</head>
<body>
<h1>Welcome to My Portfolio</h1>
<p>This paragraph is styled using internal CSS.</p>
</body>
</html>
  ```

## External CSS

External CSS involves linking a separate .css file to your HTML document. This is the most common method, especially for
larger projects, as it allows you to apply consistent styling across multiple pages.

Example:

**HTML File (index.html):**

  ```html
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>My Portfolio</title>
  <link rel="stylesheet" href="styles.css">
</head>
<body>
<h1>Welcome to My Portfolio</h1>
<p>This paragraph is styled using external CSS.</p>
</body>
</html>
  ```

**CSS File (styles.css):**
  ```css
body {
    font-family: Arial, sans-serif;
}

h1 {
    color: blue;
}

p {
    color: gray;
    font-size: 16px;
}
  ```
