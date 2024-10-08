# Solution: Building a Portfolio Webpage

In this project, you’ll create a simple portfolio webpage to showcase your work. We’ll break it down into easy-to-follow
steps.

## 1. Set Up Your HTML Document

Start with the basic HTML template:

```html
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>My Portfolio</title>
</head>
<body>
<!-- Your content will go here -->
</body>
</html>
```

## 2. Create the Header

Add a header section to include your name and navigation links:

```html

<header>
  <h1>Amir Vahed</h1>
  <nav>
    <ul>
      <li><a href="#about">About Me</a></li>
      <li><a href="#projects">Projects</a></li>
      <li><a href="#contact">Contact</a></li>
    </ul>
  </nav>
</header>
```

## 3. Add the About Me Section

Provide a brief introduction about yourself:

```html

<section id="about">
  <h2>About Me</h2>
  <p>Hello! I'm Amir Vahed, a front-end developer with a passion for creating engaging websites and applications.</p>
  <img src="profile.jpg" alt="Amir Vahed Picture">
</section>
```

## 4. Create the Projects Section

Showcase your projects with descriptions and links:

```html

<section id="projects">
  <h2>Projects</h2>
  <div>
    <h3>Project One</h3>
    <p>A brief description of the project, highlighting the key features and technologies used.</p>
    <a href="https://www.example.com/project-one">View Project</a>
  </div>
  <div>
    <h3>Project Two</h3>
    <p>A brief description of the project, highlighting the key features and technologies used.</p>
    <a href="https://www.example.com/project-two">View Project</a>
  </div>
</section>
```

## 5. Add a Contact Section

Provide a way for visitors to get in touch with you.

```html

<section id="contact">
  <h2>Contact Me</h2>
  <p>Feel free to reach out to me through the contact form below or via email.</p>
  <form action="#" method="post">
    <label for="name">Name:</label>
    <input type="text" id="name" name="name" required>

    <label for="email">Email:</label>
    <input type="email" id="email" name="email" required>

    <label for="message">Message:</label>
    <textarea id="message" name="message" rows="4" required></textarea>

    <button type="submit">Send Message</button>
  </form>
</section>
```

## 6. Put all together

```html
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>My Portfolio</title>
</head>
<body>
<header>
  <h1>Amir Vahed</h1>
  <nav>
    <ul>
      <li><a href="#about">About Me</a></li>
      <li><a href="#projects">Projects</a></li>
      <li><a href="#contact">Contact</a></li>
    </ul>
  </nav>
</header>

<section id="about">
  <h2>About Me</h2>
  <p>Hello! I'm Amir Vahed, a front-end developer with a passion for creating engaging websites and applications.</p>
  <img src="image.jpg" alt="Amir Vahed Picture">
</section>

<section id="projects">
  <h2>Projects</h2>
  <div>
    <h3>Project One</h3>
    <p>A brief description of the project, highlighting the key features and technologies used.</p>
    <a href="https://www.example.com/project-one">View Project</a>
  </div>
  <div>
    <h3>Project Two</h3>
    <p>A brief description of the project, highlighting the key features and technologies used.</p>
    <a href="https://www.example.com/project-two">View Project</a>
  </div>
</section>

<section id="contact">
  <h2>Contact Me</h2>
  <p>Feel free to reach out to me through the contact form below or via email.</p>
  <form action="#" method="post">
    <label for="name">Name:</label>
    <input type="text" id="name" name="name" placeholder="Enter your name" required><br><br>

    <label for="email">Email:</label>
    <input type="email" id="email" name="email" required><br><br>

    <label for="message">Message:</label>
    <textarea id="message" name="message" rows="4" required></textarea><br><br>

    <button type="submit">Send Message</button>
    <br><br>
  </form>
</section>

<footer>
  <p>&copy; 2024 Amir Vahed. All rights reserved.</p>
</footer>
</body>
</html>
```

> 💡 [Here](https://github.com/amirmvahed/front-end-for-back-end-engineers-tasks/tree/main/portfolio) you can see the
> source
> code
