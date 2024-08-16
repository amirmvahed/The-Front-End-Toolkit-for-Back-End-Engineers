# Solution: Contact Form

Let`s interact with our contact form.

## Step 1: Event Listener for Form Submission

```js
document.getElementById("form").addEventListener("submit", function(event) {
  event.preventDefault();
})
```

* This line attaches an event listener to the form with the ID `form`. Specifically, it listens for the submit event,
  which occurs when the user clicks the submit button.
* The purpose is to execute a function when the form is submitted, allowing us to handle the submission process in a
  customized way.
* `event.preventDefault()` stops the form from submitting in the traditional way, which would typically cause the page
  to reload.

## Step 2: Collect Form Data

```js
let firstName = document.getElementById("fname").value;
let lastName = document.getElementById("lname").value;
let email = document.getElementById("email").value;
let queryType = document.querySelector("input[name=\"queryType\"]:checked");
let message = document.getElementById("message").value;
let consent = document.getElementById("consent").checked;
```

* **`fname`, `lName`, `email,` and `message`:** These variables capture the values entered the respective input fields.
* **`queryType`:** This captures the selected radio button value under queryType.
  The `document.querySelector('input[name="queryType"]:checked')` finds the radio button that is currently selected (
  checked).
* **`consent`:** This captures whether the checkbox for consent is checked or not (returns `true` if checked, `false` if
  not).

## Step 3: Log the Form Data to the Console

```js
console.log("First Name:", firstName);
console.log("Last Name:", lastName);
console.log("Email Address:", email);
console.log("Query Type:", queryType.value);
console.log("Message:", message);
console.log("Consent:", consent);
```

## Step 4: Show an Alert and Optionally Reset the Form

```js
alert("Thank you for contacting us!");
```

This line triggers an alert box with the message "Thank you for contacting us!" when the form is successfully submitted.

## Step 5: Clearing all input fields.

```js
document.getElementById("form").reset();
```

This line resets the form, clearing all input fields.


> 💡 [Here](https://github.com/amirmvahed/front-end-for-back-end-engineers-tasks/tree/main/contact-form) you can see the
> source
> code 
