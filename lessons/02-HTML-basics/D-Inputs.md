# Introduction to HTML Input Elements
HTML input elements are crucial for gathering information from users. They are used within forms and allow users to enter data in various formats, such as text, numbers, dates, and more.

## Basic Syntax
The basic syntax for an input element is:

```html
  <input type="text" id="inputId" name="inputName" value="defaultValue">
  ```
* **type**: Specifies the type of input (e.g., text, email, number).
* **id**: Provides a unique identifier for the input element.
* **name**: Specifies the name of the input, which is used when sending form data to a server.
* **value**: Sets the default value for the input.

## Common Input Types

### 1. Text Input
Used for single-line text input.
```html
  <label for="name">Name:</label>
  <input type="text" id="name" name="name" placeholder="Enter your name" required>
  ```

* **placeholder**: Shows a hint inside the input field.
* **required**: Makes the field mandatory.

### 2. Password Input
Used for passwords, where characters are hidden.
```html
  <label for="password">Password:</label>
  <input type="password" id="password" name="password" placeholder="Enter your password" required>
  ```
### 3. Email Input
Validates that the input is a properly formatted email address.
```html
  <label for="email">Email:</label>
  <input type="email" id="email" name="email" placeholder="Enter your email" required>
  ```
### 4. Number Input
Allows users to enter numeric values. You can specify a range.
```html
  <label for="age">Age:</label>
  <input type="number" id="age" name="age" min="0" max="120" placeholder="Enter your age">
  ```
### 5. Date Input
Enables users to select a date from a calendar.
```html
  <label for="dob">Date of Birth:</label>
  <input type="date" id="dob" name="dob">
  ```
### 6. Checkbox
Allows users to select one or more options.
```html
  <label for="subscribe">
  <input type="checkbox" id="subscribe" name="subscribe" value="newsletter">
  Subscribe to newsletter
</label>
  ```
### 7. Radio Buttons
Allows users to select one option from a set.
```html
  <p>Gender:</p>
<label for="male">
  <input type="radio" id="male" name="gender" value="male">
  Male
</label>
<label for="female">
  <input type="radio" id="female" name="gender" value="female">
  Female
</label>
  ```
### 8. File Input
Allows users to upload files.
```html
  <label for="resume">Upload Resume:</label>
  <input type="file" id="resume" name="resume">
  ```
### 9. Textarea
For multi-line text input.
```html
  <label for="message">Message:</label>
  <textarea id="message" name="message" rows="4" cols="50" placeholder="Enter your message here"></textarea>
 ```

* **rows and cols**: Define the size of the textarea.

### 10. Submit Button
Sends the form data to the server.
```html
  <button type="submit">Submit</button>
 ```

## Example Form
Here’s how you can put all these inputs together in a complete form:

```html
  <!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Contact Form</title>
</head>
<body>
<h1>Contact Us</h1>
<form action="/submit" method="post">
  <label for="name">Name:</label>
  <input type="text" id="name" name="name" placeholder="Enter your name" required><br><br>

  <label for="email">Email:</label>
  <input type="email" id="email" name="email" placeholder="Enter your email" required><br><br>

  <label for="password">Password:</label>
  <input type="password" id="password" name="password" placeholder="Enter your password" required><br><br>

  <label for="age">Age:</label>
  <input type="number" id="age" name="age" min="0" max="120" placeholder="Enter your age"><br><br>

  <label for="dob">Date of Birth:</label>
  <input type="date" id="dob" name="dob"><br><br>

  <label for="subscribe">
    <input type="checkbox" id="subscribe" name="subscribe" value="newsletter">
    Subscribe to newsletter
  </label><br><br>

  <p>Gender:</p>
  <label for="male">
    <input type="radio" id="male" name="gender" value="male">
    Male
  </label>
  <label for="female">
    <input type="radio" id="female" name="gender" value="female">
    Female
  </label><br><br>

  <label for="resume">Upload Resume:</label>
  <input type="file" id="resume" name="resume"><br><br>

  <label for="message">Message:</label>
  <textarea id="message" name="message" rows="4" cols="50" placeholder="Enter your message here"></textarea><br><br>

  <button type="submit">Submit</button>
</form>
</body>
</html>
 ```