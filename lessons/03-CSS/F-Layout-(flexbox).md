# Layout (flexbox)

## What is Flexbox?

Flexbox makes it easy to create flexible and responsive layouts. It works on a parent-child basis, aligning child
elements within a parent container.

## The Flexbox Model

Flexbox works with two main components:

1. **Flex Container:** The parent element that holds the flex items. It’s the element on which you apply display: flex;.
2. **Flex Items:** The child elements within the flex container. These items are automatically aligned according to the
   rules defined by Flexbox.

Example:
**HTML:**

```html

<div class="container">
  <div class="item">Item 1</div>
  <div class="item">Item 2</div>
  <div class="item">Item 3</div>
</div>
```

**CSS:**

```css
.container {
    display: flex; /* Turns the container into a flex container */
    background-color: #f4f4f4;
    align-items: center; /* Centers the elements vertically  */
    justify-content: center; /* Centers the elements horizontally  */
    height: 100vh;
}

.item {
    background-color: #333;
    color: white;
    padding: 20px;
    margin: 10px;
}
```

## Key Flexbox Properties

Let’s break down some of the most important Flexbox properties you'll use to create layouts.

### **1. display: flex**

This property is applied to the container to enable Flexbox. It turns the container into a flex container and its
children into flex items.

Example:

```css
.container {
    display: flex;
}
```

### **2. justify-content**

This property controls the alignment of flex items along the main axis (horizontal by default). It’s useful for
distributing space between items.

**Common Values:**

* **flex-start:** Items align to the start of the container (default).
* **flex-end:** Items align to the end of the container.
* **center:** Items are centered in the container.
* **space-between:** Items are evenly distributed, with the first item at the start and the last item at the end.
* **space-around:** Items are evenly distributed with space around them.

Example:

```css
    .container {
    display: flex;
    justify-content: space-between;
}
```

### **3. align-items**

This property controls the alignment of flex items along the cross axis (vertical by default).

**Common Values:**

* **stretch**: Items stretch to fill the container (default).
* **flex-start**: Items align to the start of the cross axis.
* **flex-end**: Items align to the end of the cross axis.
* **center**: Items are centered along the cross axis.

Example:

```css
.container {
    display: flex;
    align-items: center;
}
```

### **4. flex-direction**

This property defines the direction of the main axis along which the items are placed.

**Common Values:**

* **row**: Items are placed horizontally (default).
* **row-reverse**: Items are placed horizontally in reverse order.
* **column**: Items are placed vertically.
* **column-reverse**: Items are placed vertically in reverse order.

Example:

```css
.container {
    display: flex;
    flex-direction: column;
}
```

### **5. flex-wrap**

This property controls whether the flex items should wrap onto multiple lines.

**Common Values:**

* **nowrap**: All items will be on one line (default).
* **wrap**: Items are placed horizontally in reverse order.
* **wrap-reverse**: Items will wrap onto multiple lines in reverse order.

Example:

```css
.container {
    display: flex;
    flex-wrap: wrap;
}
```

> 💡 use [this tool](https://angrytools.com/css-flex/) to fully understand the flexbox, and generate its code. 