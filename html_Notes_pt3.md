# HTML Forms

HTML forms are an essential component of web pages that allow users to submit data to a server. This document covers the basic structure and attributes of HTML forms.

## Basic Form Structure

A basic HTML form consists of the `<form>` element and various input elements like text fields, checkboxes, radio buttons, submit buttons, etc.

**Example**:
```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Basic Form Example</title>
</head>
<body>
    <h1>Basic HTML Form</h1>
    <form action="/submit_form" method="post">
        <label for="name">Name:</label>
        <input type="text" id="name" name="name" required>
        <br><br>
        
        <label for="email">Email:</label>
        <input type="email" id="email" name="email" required>
        <br><br>
        
        <label for="password">Password:</label>
        <input type="password" id="password" name="password" required>
        <br><br>
        
        <input type="submit" value="Submit">
    </form>
</body>
</html>
```

### Key Elements

- `<form>`: The container for the form elements.
- `<label>`: Defines a label for an `<input>` element.
- `<input>`: Defines an input field.

## Form Attributes

### `action`
The `action` attribute specifies the URL where the form data will be sent upon submission.

**Syntax**:
```html
<form action="submit_form.php">
    <!-- form elements -->
</form>
```

### `method`
The `method` attribute specifies the HTTP method to use when sending form data. The two most common methods are `GET` and `POST`.

- **GET**: Appends form data to the URL.
- **POST**: Sends form data as part of the HTTP request body.

**Syntax**:
```html
<form method="post">
    <!-- form elements -->
</form>
```

### `enctype`
The `enctype` attribute specifies how the form data should be encoded when submitted to the server. This attribute is used only when `method="post"`.

- `application/x-www-form-urlencoded`: Default encoding.
- `multipart/form-data`: Used for forms that include file uploads.
- `text/plain`: Sends data without any encoding.

**Syntax**:
```html
<form enctype="multipart/form-data">
    <!-- form elements -->
</form>
```

### `target`
The `target` attribute specifies where to display the response that is received after submitting the form.

- `_self`: Default. Opens in the same frame as it was submitted.
- `_blank`: Opens in a new window or tab.
- `_parent`: Opens in the parent frame.
- `_top`: Opens in the full body of the window.

**Syntax**:
```html
<form target="_blank">
    <!-- form elements -->
</form>
```

## Input Types

### Text Input
Used to get free-form text input from the user.

**Syntax**:
```html
<input type="text" id="name" name="name">
```

### Email Input
Used to get email addresses from the user. Includes validation for email format.

**Syntax**:
```html
<input type="email" id="email" name="email">
```

### Password Input
Used to get password input from the user. The characters are hidden.

**Syntax**:
```html
<input type="password" id="password" name="password">
```

### Submit Button
Used to submit the form data to the server.

**Syntax**:
```html
<input type="submit" value="Submit">
```

## Example: Complete Basic Form

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Basic Form Example</title>
</head>
<body>
    <h1>Basic HTML Form</h1>
    <form action="/submit_form" method="post">
        <label for="name">Name:</label>
        <input type="text" id="name" name="name" required>
        <br><br>
        
        <label for="email">Email:</label>
        <input type="email" id="email" name="email" required>
        <br><br>
        
        <label for="password">Password:</label>
        <input type="password" id="password" name="password" required>
        <br><br>
        
        <input type="submit" value="Submit">
    </form>
</body>
</html>
```

This form captures a user's name, email, and password, and submits the data to the specified `action` URL using the `POST` method.