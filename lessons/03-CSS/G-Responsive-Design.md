# Responsive Design with CSS

## What is Responsive Design?

Responsive design is the approach of creating web pages that look and function well on a variety of devices and screen
sizes. The goal is to provide an optimal viewing experience, with easy reading and navigation, minimal resizing,
panning, and scrolling.

## Media Queries

Media queries are the backbone of responsive design. They let you apply different styles based on the device's
characteristics, like screen width.

**Example:**

Let's add media queries to adjust the layout for different screen sizes.

**HTML:**

  ```html
    <!DOCTYPE html>
    <html lang="en">
    <head>
      <meta charset="UTF-8">
      <meta name="viewport" content="width=device-width, initial-scale=1.0">
      <title>Title</title>
    </head>
    <style>
      .container {
        display: flex;
        flex-wrap: wrap;
        justify-content: center;
      }
    
      .box {
        width: 25%;
        margin: 10px;
        background-color: #333;
        color: white;
        padding: 20px;
        text-align: center;
      }
    
      /* Styles for tablets (900px and down) */
      @media (max-width: 900px) {
        .box {
          background-color: green;
          width: 50%; /* Boxes take up more space on smaller screens */
        }
      }
    
      /* Styles for mobile phones (600px and down) */
      @media (max-width: 600px) {
        .box {
          background-color: red;
          width: 100%; /* Each box takes up the full width */
        }
      }
    </style>
    <body>
    <div class="container">
      <div class="box">Item 1</div>
      <div class="box">Item 2</div>
      <div class="box">Item 3</div>
    </div>
    </body>
    </html>
  ```

## Viewport Meta Tag

To ensure your responsive designs look good on mobile devices, include the viewport meta tag in your HTML <head>
section. This tag instructs the browser on how to adjust the page’s dimensions and scaling.

```html
<meta name="viewport" content="width=device-width, initial-scale=1.0">
  ```

This tag tells the browser to match the screen's width (device width) and set the initial zoom level to 1.
