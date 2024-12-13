## Ghostly Moves: Animate Your Pacman Ghost with JavaScript

### Developmental Outcome
1. Understand how to move elements dynamically using JavaScript.
2. Learn how to structure HTML, CSS, and JavaScript files separately.
3. Implement basic movement functionality using keyboard events in JavaScript.

### Introduction: Moving with Code
Imagine having control over a Pacman ghost—making it move up, down, left, and right just by using the arrow keys! With JavaScript, you can easily bring such animations to life by interacting with HTML and CSS.

In this lesson, you’ll use JavaScript to animate a Pacman ghost image inside a container, learning how HTML, CSS, and JavaScript work together to create movement.

### Main Content

#### 1. HTML Structure

The HTML file contains the structure of the game. It creates the container in which the ghost will move and includes the image of the ghost.

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Ghostly Moves: Animate Your Pacman Ghost with JavaScript</title>
    <link rel="stylesheet" href="styles.css">
</head>
<body>
    <h1>Ghostly Moves: Animate Your Pacman Ghost with JavaScript</h1>
    <div id="game-container">
        <img id="ghost" src="ghost.png" alt="Pacman Ghost">
    </div>

    <script src="script.js"></script>
</body>
</html>
```

- The `<link>` tag connects the CSS file (`styles.css`), while the `<script>` tag at the bottom includes the JavaScript file (`script.js`). 
- The ghost image (`ghost.png`) is added using the `<img>` tag.

#### 2. CSS Styling

The CSS file defines how the container and the ghost image look and behave.

```css
/* styles.css */
#game-container {
    width: 400px;
    height: 400px;
    border: 2px solid black;
    position: relative;
    overflow: hidden;
    background-color: black;
}

#ghost {
    width: 50px;
    position: absolute;
    top: 175px;
    left: 175px;
}
```

- The container has a fixed width and height with a border to represent the game area.
- The ghost image is positioned absolutely within the container so that it can move freely.

#### 3. JavaScript Functionality

The JavaScript file controls the ghost's movements based on keyboard input.

```javascript
// script.js
let ghost = document.getElementById('ghost');
let ghostPosition = { top: 175, left: 175 };

document.addEventListener('keydown', function (event) {
    const step = 10;
    
    if (event.key === 'ArrowUp') {
        ghostPosition.top = Math.max(0, ghostPosition.top - step); // Move up
    } else if (event.key === 'ArrowDown') {
        ghostPosition.top = Math.min(350, ghostPosition.top + step); // Move down
    } else if (event.key === 'ArrowLeft') {
        ghostPosition.left = Math.max(0, ghostPosition.left - step); // Move left
    } else if (event.key === 'ArrowRight') {
        ghostPosition.left = Math.min(350, ghostPosition.left + step); // Move right
    }

    ghost.style.top = ghostPosition.top + 'px';
    ghost.style.left = ghostPosition.left + 'px';
});
```

- **Event Listener**: Listens for keydown events and moves the ghost in the corresponding direction (up, down, left, right).
- **Position Updates**: Ensures the ghost doesn’t move outside the container by limiting its position with `Math.max()` and `Math.min()`.

### Key Points
- The ghost image is moved using JavaScript by altering its `top` and `left` CSS properties.
- The arrow keys are mapped to move the ghost in different directions.
- Separation of HTML, CSS, and JavaScript files improves organization and maintainability.