# CSS Syntax and Selectors

CSS is all about targeting elements and applying styles. Here’s a basic rundown:

## CSS Syntax:

  ```css
  selector {
    property: value;
}
  ```

* **Selector**: Targets the HTML element you want to style.
* **Property**: The aspect of the element you want to change (like color, font-size).
* **Value**: The specific setting for the property (like blue, 16px).

Example:

  ```css
/* This is a comment in CSS */
h1 {
    color: blue; /* Text color */
    font-size: 24px; /* Size of the text */
}
  ```

## Selectors:

### **1. Element Selector**

Targets all instances of an element.

  ```css
p {
    color: gray;
}
  ```

### **2. Class Selector**

Targets elements with a specific class attribute.

  ```css
.highlight {
    background-color: yellow;
}
  ```

### **3. ID Selector**

Targets a single element with a specific ID.

```css
#header {
    background-color: #333;
    color: white;
}
```

> 💡 Understanding how to use these selectors is key to effectively applying styles to your web page.