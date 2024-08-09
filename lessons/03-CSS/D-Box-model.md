# Box Model
Every HTML element can be considered a box, and CSS lets you control this box’s dimensions and spacing. The box model consists of:

* **Content**: The actual content of the element (text, images).
* **Padding**: Space between the content and the border.
* **Border**: Surrounds the padding (if any) and content.
* **Margin**: Space outside the border, separating the element from other elements.

![box model diagram](/front-end-for-back-end-engineers/images/box_model.png)

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
<div class="box">Content</div>
</body>
</html>
  ```

**CSS File (styles.css):**
  ```css
.box {
    width: 300px; /* Width of the content area */
    padding: 20px; /* Space inside the box, around the content */
    border: 2px solid black; /* Border around the padding */
    margin: 10px; /* Space outside the border */
}
  ```
