### Assignment: Enhance Your Portfolio: Apply Display and Positioning Properties

#### Trainee Goal:
1. Utilize display and positioning properties to improve the layout of your portfolio.
2. Implement visual hierarchy by adjusting the placement of elements on the page.
3. Apply the approach to layout to create a cohesive and aesthetically pleasing design.

#### Duration:
1 - 2 hours

#### Difficulty:
Intermediate

#### Instructions:
1. Open your existing **first_last_profile_css.zip** file and locate your **first_last_profile2.html** and **styles.css** files.
2. In your **styles.css** file, apply the following:
   - Utilize display properties (e.g., `block`, `inline`, `inline-block`, `none`) to control how elements are presented.
   - Use positioning properties (`static`, `relative`, `absolute`, `fixed`) to arrange elements on the page effectively.
   - Enhance the visual hierarchy by ensuring important content is more prominent.
3. Pay attention to the overall layout and make adjustments to improve the flow and readability of your content.
4. **Submission**: Once you are satisfied with your updates, compress the folder containing your HTML and CSS files, and rename it to **first_last_profile_css_updated.zip** before submitting.

#### Bonus Task:
- Experiment with positioning elements to create an interesting layout that draws attention to specific areas of your portfolio.

#### Criteria for Success:
- **Layout**: Effective use of display and positioning properties to create a visually appealing layout.
- **Visual Hierarchy**: Clear distinction between headings, subheadings, and body text.
- **Consistency**: Uniform styling applied across all sections of the portfolio.
- **Creativity**: Unique design choices that reflect your personal style and enhance the overall presentation.

---

### HTML Code

Here’s an example of how your HTML file could be structured (including the "Contact Us" section):

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Your Portfolio</title>
    <link rel="stylesheet" href="styles.css"> <!-- Link to external CSS -->
</head>
<body>
    <header>
        <h1>Your Name</h1>
        <p>A brief introduction about yourself.</p>
    </header>
    <section>
        <h2>About Me</h2>
        <p>Write something about yourself here.</p>
    </section>
    <section>
        <h2>My Skills</h2>
        <ul>
            <li>HTML</li>
            <li>CSS</li>
            <li>JavaScript</li>
        </ul>
    </section>
    <section>
        <h2>Contact Us</h2>
        <form action="#" method="post">
            <label for="name">Name:</label>
            <input type="text" id="name" name="name" required>
            
            <label for="email">Email:</label>
            <input type="email" id="email" name="email" required>
            
            <label for="message">Message:</label>
            <textarea id="message" name="message" rows="4" required></textarea>
            
            <button type="submit">Submit</button>
        </form>
    </section>
    <footer>
        <p>&copy; 2024 Your Name</p>
    </footer>
</body>
</html>
```

### CSS Code

Here’s an example of how your CSS file (`styles.css`) could look, including styles for the contact form:

```css
body {
    font-family: Arial, sans-serif;
    margin: 0;
    padding: 0;
    background-color: #f4f4f4;
}

header {
    text-align: center;
    padding: 20px;
    background-color: #333;
    color: white;
}

h1 {
    font-size: 2.5em;
}

h2 {
    font-size: 2em;
    margin-top: 20px;
}

section {
    margin: 20px;
    padding: 15px;
    background-color: white;
    border-radius: 8px;
    box-shadow: 0 0 10px rgba(0, 0, 0, 0.1);
}

/* Example of display property usage */
ul {
    list-style-type: none;
    padding: 0;
}

ul li {
    display: inline-block; /* Align skills horizontally */
    margin-right: 10px;
}

/* Contact form styles */
form {
    display: flex;
    flex-direction: column;
}

label {
    margin: 10px 0 5px;
}

input, textarea {
    padding: 10px;
    border: 1px solid #ccc;
    border-radius: 4px;
}

button {
    margin-top: 10px;
    padding: 10px;
    background-color: #333;
    color: white;
    border: none;
    border-radius: 4px;
    cursor: pointer;
}

button:hover {
    background-color: #555;
}

/* Example of positioning */
footer {
    position: relative;
    text-align: center;
    margin-top: 20px;
}
```