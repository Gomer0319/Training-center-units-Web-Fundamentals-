## Enhance Your Portfolio: DOM Selection and Basic Manipulation

### Trainee Goal
By completing this assignment, trainees will:
1. Practice using various DOM selection methods to manipulate elements in their HTML.
2. Learn how to modify text content and attributes of existing elements.
3. Understand how to access and update elements in the DOM using JavaScript.

### Duration
1 hour

### Difficulty
Intermediate

### Instructions
You will update your existing `first_last_profile2.html` file to practice DOM selection and basic manipulation. Follow these steps:

1. **Open Your Files**: Use the existing HTML file from your previous assignment.
2. **DOM Selection**:
   - Use `getElementById` to select the profile name and change its text.
   - Use `getElementsByClassName` to select the bio and modify its content.
   - Use `getElementsByTagName` to select the profile image and change its `src` attribute.
3. **Review**: Check the changes in the browser to see the updated profile information.
4. **Submission**: Once you are satisfied with your updates, compress the folder containing your HTML file and rename it to `first_last_profile2_updated.zip` before submitting.

### Bonus Task
For extra points, use `querySelector` to select the profile name and modify its text. 

### Criteria for Success
Evaluation will be based on:
- Effective use of DOM selection methods to manipulate content.
- Successful modification of the profile name, bio, and image.
- Clean and organized code demonstrating understanding of DOM selection.

### Solution
**HTML (profile2.html)**:
```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>John Doe Portfolio</title>
    <link rel="stylesheet" href="styles.css">
</head>
<body>
    <header>
        <h1 id="profile-name">John Doe</h1>
        <p>Web Developer</p>
    </header>

    <section>
        <h2>About Me</h2>
        <p class="profile-bio">Hello! I'm a passionate web developer with skills in HTML, CSS, and JavaScript.</p>
    </section>

    <section>
        <h2>Technologies I Use</h2>
        <ul>
            <li><img src="html_logo.png" alt="HTML Logo" width="100"></li>
            <li><img src="css_logo.png" alt="CSS Logo" width="100"></li>
            <li><img src="js_logo.png" alt="JavaScript Logo" width="100"></li>
        </ul>
    </section>

    <section>
        <h2>Contact Us</h2>
        <form action="#" method="post">
            <label for="email">Email:</label>
            <input type="email" id="email" name="email" required>
            
            <label for="name">Name:</label>
            <input type="text" id="name" name="name">
            
            <label for="message">Message:</label>
            <textarea id="message" name="message"></textarea>

            <button type="submit">Submit</button>
        </form>
    </section>

    <script>
        // JavaScript for DOM Selection and Manipulation
        const nameElement = document.getElementById('profile-name');
        const bioElement = document.getElementsByClassName('profile-bio')[0];
        const imageElement = document.getElementsByTagName('img')[0];

        // Change content
        nameElement.textContent = "Jane Doe";
        bioElement.textContent = "A short bio about Jane.";
        imageElement.src = "new-image.jpg";
    </script>
</body>
</html>
```