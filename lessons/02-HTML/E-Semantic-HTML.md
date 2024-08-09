# Understanding Semantic HTML

## What is Semantic HTML?

Semantic HTML refers to the use of HTML elements that convey the meaning of the content they contain. These elements not
only describe how the content should appear on the page but also provide context about the content to browsers, search
engines, and assistive technologies like screen readers.

## Example of Non-Semantic vs. Semantic HTML

### Non-Semantic HTML:

```html

<div id="header">Welcome to My Website</div>
<div id="content">
  <p>This is my website where I share my projects and blog posts.</p>
</div>
<div id="footer">Contact me at email@example.com</div>
```

### Semantic HTML:

```html

<header>Welcome to My Website</header>
<main>
  <p>This is my website where I share my projects and blog posts.</p>
</main>
<footer>Contact me at email@example.com</footer>
```

In the semantic example, elements like **`<header>`**, **`<main>`**, and **`<footer>`** provide clear context about the
structure and content of the page.

## Why Use Semantic HTML?

1. Improves Accessibility
2. Enhances SEO
3. Improves Code Maintainability

## Common Semantic HTML Elements

### **1. `<header>` and `<nav>`**

**`<header>`** Represents the introductory content and **`<nav>`** defines a set of navigational links for a section or
page.

```html

<header>
  <h1>Welcome to My Portfolio</h1>
  <nav>
    <ul>
      <li><a href="#about">About</a></li>
      <li><a href="#projects">Projects</a></li>
      <li><a href="#contact">Contact</a></li>
    </ul>
  </nav>
</header>
```

### **2. `<main>`**

Represents the main content of the document. There should only be one <main> element per page.

```html
<main>
  <section id="about">
    <h2>About Me</h2>
    <p>I am a web developer with a passion for creating beautiful and functional websites.</p>
  </section>
</main>
```

### **3. `<section>`**

Defines a thematic grouping of content, typically with a heading. Sections are used to group related content together.
```html
<section id="services">
  <h2>Our Services</h2>
  <p>We offer web development, design, and SEO services.</p>
</section>
```

### **4. `<footer>`**

Represents the footer of a document or section, typically containing metadata, author information, or links to related content.

```html

<footer>
  <p>&copy; 2024 My Portfolio. All rights reserved.</p>
</footer>
```


Using semantic HTML is an essential practice for building modern, accessible, and SEO-friendly websites. By using the right semantic elements, you make your code more meaningful, easier to maintain, and better understood by both humans and machines.