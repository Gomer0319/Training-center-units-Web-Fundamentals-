## Create Your Anime Survey Form: Gather Insights!

### Trainee Goal
By completing this assignment, trainees will:
1. Construct a functional survey form using HTML `<form>` and input elements.
2. Implement various input types such as text fields, radio buttons, and text areas.
3. Organize and structure form data effectively.

### Duration
30 minutes to 1 hour

### Difficulty
Beginner

### Instructions
Your task is to create a survey form that collects information about your favorite anime. Follow these steps:

1. **Create a new HTML file** named `first_last_survey.html`, replacing `first` and `last` with your actual first and last name (e.g., `john_doe_survey.html`).
2. **Structure your form** using the `<form>` element and appropriate `<input>` types. Include the following fields:
   - **Name**: A text input for the respondent's name.
   - **Email Address**: A text input for the respondent's email.
   - **Gender**: A set of radio buttons for the respondent to select their gender.
   - **Selection of Anime**: A section where respondents can choose an anime to be surveyed. You may use links to images or upload images of the anime options.
   - **Reason for Choosing the Anime**: A text area for respondents to provide their reason for choosing the selected anime.
   - **Submit Button**: A button to submit the form.
3. Use appropriate labels for each input field to enhance accessibility.
4. **Local Assets**: If you use images, place the HTML file and any local image assets in one folder. Ensure the images are properly linked in your HTML code.
5. **Submission**: Compress the folder containing your HTML file and any local assets into a .zip file, renaming the zip file to match your HTML file (e.g., `john_doe_survey.zip`). Submit it via the designated submission portal.

### Bonus Task: Effective Labeling
For extra points:
- Ensure that all input fields are well-labeled, and consider how using `<fieldset>` and `<legend>` can enhance the organization of your form.

### Criteria for Success
Your submission will be evaluated based on:
- **Effective use of form elements**: Proper implementation of the `<form>` tag and input types.
- **Content organization**: Clear structure of the form, with each input element appropriately labeled.
- **Inclusion of images**: Correctly adding images related to the anime options using links or uploaded files.
- **Proper formatting**: Ensure proper indentation and cleanliness of code.

---

### Solution

Here’s an example solution for your reference. You can modify the content as per your requirements:

```html
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Anime Survey Form</title>
</head>
<body>
  <h1>Anime Survey Form</h1>
  <form action="#" method="post">
    <label for="name">Name:</label>
    <input type="text" id="name" name="name" required>
    <br>
    
    <label for="email">Email Address:</label>
    <input type="email" id="email" name="email" required>
    <br>
    
    <label>Gender:</label>
    <input type="radio" id="male" name="gender" value="male">
    <label for="male">Male</label>
    <input type="radio" id="female" name="gender" value="female">
    <label for="female">Female</label>
    <input type="radio" id="other" name="gender" value="other">
    <label for="other">Other</label>
    <br>
    
    <label>Select Your Favorite Anime:</label>
    <fieldset>
      <legend>Choose one:</legend>
      <label for="anime1">
        <img src="path/to/anime1.jpg" alt="Anime 1" width="100">
        <input type="radio" id="anime1" name="anime" value="anime1"> Anime Title 1
      </label>
      <br>
      <label for="anime2">
        <img src="path/to/anime2.jpg" alt="Anime 2" width="100">
        <input type="radio" id="anime2" name="anime" value="anime2"> Anime Title 2
      </label>
      <br>
      <label for="anime3">
        <img src="path/to/anime3.jpg" alt="Anime 3" width="100">
        <input type="radio" id="anime3" name="anime" value="anime3"> Anime Title 3
      </label>
    </fieldset>
    <br>
    
    <label for="reason">Reason for Choosing the Anime:</label>
    <textarea id="reason" name="reason" rows="4" cols="50" required></textarea>
    <br>
    
    <input type="submit" value="Submit">
  </form>
</body>
</html>
```