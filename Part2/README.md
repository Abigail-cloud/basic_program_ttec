# Week 2: Deeper into HTML & Introduction to CSS

## Objective:
Learn semantic HTML and apply basic styling with CSS.

## Topics Covered:

### Semantic HTML:
- **`<header>`**: Defines the header section of a webpage or a section within the page.
- **`<footer>`**: Represents the footer of a webpage or a section, typically containing copyright information, links, or contact details.
- **`<nav>`**: Used to define a navigation menu, containing links to other pages or sections.
- **`<section>`**: Represents a standalone section of content, such as a chapter, tab, or group of related content.
- **`<article>`**: Defines independent, self-contained content, such as a blog post, news article, or comment.

### Forms:
- **`<input>`**: Creates input fields for user data, such as text, email, password, etc.
- **`<textarea>`**: Provides a multi-line text input field, often used for comments or messages.
- **`<button>`**: Defines a clickable button, which can submit forms or trigger actions.
- **`<label>`**: Associates a label with an input field, improving accessibility and usability.
- **`<select>`**: Creates a dropdown list for users to select from predefined options.

### Introduction to CSS:
- **CSS Syntax**: CSS rules consist of a selector and a declaration block. For example:
  ```css
  h1 {
      color: blue;
      font-size: 24px;
  }


  >>>>>>>>>>>>>>>>>>>>>>>>>>
  ## CSS Selectors:
Used to target HTML elements for styling. Examples include:

- **Element selectors**: Target HTML elements directly. For example:
  ```css
  h1 {
      color: blue;
  }
  p {
      font-size: 16px;
  }
  div {
      background-color: #f4f4f4;
  }

 - **Class selectors:** Target elements with a specific class attribute. For example:
  .class-name {
    font-weight: bold;
}

- **ID selectors:** Target a single element with a specific ID attribute. For example:
#id-name {
    text-align: center;
}

- **Styling Text:**
Properties like font-family, font-size, font-weight, and text-align are used to style text. For example:

h1 {
    font-family: Arial, sans-serif;
    font-size: 24px;
    font-weight: bold;
    text-align: center;
}

- **Colors and Backgrounds**
Use color for text color, background-color for background color, and background-image for adding images to backgrounds. For example:

body {
    color: #333;
    background-color: #f4f4f4;
    background-image: url('background.jpg');
}

- ** Hands-on Practice:**
✅ Build a simple webpage with a form and basic CSS styles.

Example Code:

<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Simple Webpage with Form</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            background-color: #f4f4f4;
            margin: 0;
            padding: 0;
        }
        header {
            background-color: #333;
            color: white;
            padding: 10px 0;
            text-align: center;
        }
        form {
            margin: 20px;
            padding: 20px;
            background-color: white;
            border-radius: 5px;
        }
        label {
            display: block;
            margin-bottom: 5px;
        }
        input, textarea, select {
            width: 100%;
            padding: 10px;
            margin-bottom: 10px;
            border: 1px solid #ccc;
            border-radius: 5px;
        }
        button {
            background-color: #333;
            color: white;
            padding: 10px 20px;
            border: none;
            border-radius: 5px;
            cursor: pointer;
        }
        button:hover {
            background-color: #555;
        }
    </style>
</head>
<body>
    <header>
        <h1>Welcome to My Webpage</h1>
    </header>
    <form>
        <label for="name">Name:</label>
        <input type="text" id="name" name="name" required>

        <label for="email">Email:</label>
        <input type="email" id="email" name="email" required>

        <label for="message">Message:</label>
        <textarea id="message" name="message" rows="5" required></textarea>

        <label for="country">Country:</label>
        <select id="country" name="country">
            <option value="usa">USA</option>
            <option value="canada">Canada</option>
            <option value="uk">UK</option>
        </select>

        <button type="submit">Submit</button>
    </form>
</body>
</html>
