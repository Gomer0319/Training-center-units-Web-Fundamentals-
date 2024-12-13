## Ghostly Moves: Animate Your Pacman Ghost with JavaScript

### Developmental Outcomes
By the end of this lesson, students should be able to:
1. Understand how to manipulate HTML elements using JavaScript to create animations.
2. Learn basic CSS styling for positioning elements.
3. Implement event listeners for user interactions to control movements.

### Get Ready to Move Your Ghost!

In this lesson, we will create a fun demo where a Pacman ghost image moves around the screen. We will use HTML to structure our page, CSS for styling and positioning, and JavaScript to handle the movements. By the end of this demo, you'll be able to control the ghost's movements using the arrow keys on your keyboard!

### Building the Stage: Setting Up HTML

We'll start by creating the HTML file that will contain our ghost image and provide a basic layout.

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Pacman Ghost Movement</title>
    <link rel="stylesheet" href="styles.css">
</head>
<body>
    <div class="container">
        <img id="ghost" src="pacman_ghost.png" alt="Pacman Ghost">
    </div>
    <script src="script.js"></script>
</body>
</html>
```

### Setting the Scene: Understanding Our HTML Structure

- The `<div class="container">` element serves as the boundary for our ghost movement, ensuring that the ghost stays within a defined area.
- The `<img>` tag displays the ghost image (make sure you have a file named `pacman_ghost.png` in your project folder).
- The script tag at the bottom links our external JavaScript file, `script.js`.

### Dressing Up: Adding CSS for Style

Next, we'll create a CSS file to style the container and position the ghost image.

**`styles.css`**

```css
body {
    display: flex;
    justify-content: center;
    align-items: center;
    height: 100vh;
    margin: 0;
    background-color: #f0f0f0;
}

.container {
    position: relative;
    width: 400px;
    height: 400px;
    border: 2px solid #000;
    overflow: hidden; /* Prevent the ghost from moving outside the container */
}

#ghost {
    position: absolute;
    width: 50px; /* Adjust size as needed */
    height: 50px; /* Adjust size as needed */
    top: 175px; /* Initial position */
    left: 175px; /* Initial position */
}
```

### Making It Look Good: CSS Styling Explained

- The `body` styles center the container in the viewport and set a light gray background.
- The `.container` class creates a square area for the ghost to move in and adds a border.
- The `#ghost` ID styles the ghost image, setting its initial position in the center of the container and preventing overflow.

### Time to Move: Implementing JavaScript for Action

Now, let’s add the JavaScript code to handle the ghost's movement based on keyboard input.

**`script.js`**

```javascript
const ghost = document.getElementById('ghost');
let position = { top: 175, left: 175 }; // Initial position of the ghost

// Function to move the ghost
function moveGhost(direction) {
    const step = 10; // Number of pixels to move
    switch (direction) {
        case 'ArrowUp':
            if (position.top > 0) {
                position.top -= step;
            }
            break;
        case 'ArrowDown':
            if (position.top < 350) { // 400 - 50 (ghost height)
                position.top += step;
            }
            break;
        case 'ArrowLeft':
            if (position.left > 0) {
                position.left -= step;
            }
            break;
        case 'ArrowRight':
            if (position.left < 350) { // 400 - 50 (ghost width)
                position.left += step;
            }
            break;
    }
    updateGhostPosition();
}

// Function to update the ghost's position in the CSS
function updateGhostPosition() {
    ghost.style.top = position.top + 'px';
    ghost.style.left = position.left + 'px';
}

// Event listener for keydown events
document.addEventListener('keydown', (event) => {
    moveGhost(event.key);
});
```

### Making the Magic Happen: JavaScript Code Explained

- **Position Object:** The `position` object tracks the ghost's current coordinates.
- **moveGhost Function:** This function moves the ghost based on the arrow key pressed:
  - **ArrowUp** and **ArrowDown** adjust the `top` position.
  - **ArrowLeft** and **ArrowRight** adjust the `left` position.
  - Boundary checks ensure the ghost doesn't move outside the container.
- **updateGhostPosition Function:** This updates the ghost's CSS `top` and `left` properties to reflect the new position.
- **Event Listener:** The `keydown` event listens for arrow key presses to trigger the movement.

---

### Key Points

- We created an interactive demo that allows a ghost image to move around the screen using JavaScript.
- HTML provided the structure, CSS styled the elements, and JavaScript handled the logic for movement.
- This exercise illustrates how to combine these three languages to create dynamic web applications.

### Final Thoughts on Your Ghostly Project

Feel free to experiment with different images, step sizes, and container sizes to customize your ghost movement demo! This foundation will help you build more complex animations and interactions in your web projects.