## Expand Your Portfolio: Add a Contact Us Form!

### Trainee Goal
By completing this assignment, trainees will:
1. Integrate a functional Contact Us form into their existing personal profile portfolio.
2. Utilize various HTML input elements effectively to collect user information.
3. Enhance their understanding of form validation.

### Duration
30 minutes to 1 hour

### Difficulty
Intermediate

### Instructions
Your task is to add a Contact Us form to your existing personal profile portfolio. Follow these steps:

1. **Open your existing HTML file** for the personal profile that you created earlier (e.g., `first_last_profile.html`).
2. **Add a new section** for the Contact Us form below your profile information.
3. **Structure your Contact Us form** using the `<form>` element and appropriate `<input>` types. Include the following fields:
   - **Email**: A text input for the respondent's email address.
   - **Name**: A text input for the respondent's name.
   - **Message**: A text area for the respondent to leave a message.
   - **Submit Button**: A button to submit the form.
4. **Submission**: Place your updated HTML file in a folder along with any local assets, compress it, and submit. **Rename the HTML file to `first_last_profile2.html`** before zipping.

### Bonus Task: Make the Email Field Required
For extra points:
- **Implement the `required` attribute on the email input field** to enforce validation, ensuring that users cannot submit the form without entering an email address.

### Criteria for Success
Your submission will be evaluated based on:
- **Effective use of form elements**: Proper implementation of the `<form>` tag and input types.
- **Content organization**: Clear structure of the form with appropriate labels for each input element.
- **Inclusion of required fields**: Correctly using the `required` attribute for the email input field.
- **Proper formatting**: Ensure proper indentation and cleanliness of code.

---

### Solution


```html
<!-- Assuming this is added to your existing profile HTML file -->
<section id="contact">
  <h2>Contact Us</h2>
  <form action="#" method="post">
    <label for="email">Email:</label>
    <input type="email" id="email" name="email" required>
    <br>
    
    <label for="name">Name:</label>
    <input type="text" id="name" name="name" required>
    <br>
    
    <label for="message">Message:</label>
    <textarea id="message" name="message" rows="4" cols="50" required></textarea>
    <br>
    
    <input type="submit" value="Submit">
  </form>
</section>
```