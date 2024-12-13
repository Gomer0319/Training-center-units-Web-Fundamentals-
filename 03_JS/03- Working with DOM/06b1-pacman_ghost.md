## Ghostly Moves: Animate Your Pacman Ghost with JavaScript

### Developmental Outcomes
1. Understand how to implement movement using JavaScript.
2. Learn to control element positioning with CSS.
3. Gain familiarity with event handling for keyboard inputs.

### Introduction to Ghostly Movement
Imagine your Pacman ghost is like a puppet on strings, waiting for your command to move. In this lesson, we will learn how to control the ghost's movements using JavaScript, making it dance around the screen based on keyboard input!

### Understanding Movement Logic
To make the ghost move, we will use simple `if-else` statements that respond to keyboard events. The ghost will move up, down, left, or right based on the arrow keys pressed.

### Main Content

#### HTML Structure
We will set up a basic HTML structure to house our ghost.

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
    <div class="game-area">
        <img id="ghost" src="ghost.png" alt="Pacman Ghost" />
    </div>
    <script src="script.js"></script>
</body>
</html>
```

#### CSS Styles
Now, let's add some CSS to style the game area and the ghost.

```css
body {
    margin: 0;
    display: flex;
    justify-content: center;
    align-items: center;
    height: 100vh;
    background-color: black;
}

.game-area {
    width: 500px;
    height: 500px;
    position: relative;
    border: 2px solid white;
}

#ghost {
    position: absolute;
    width: 50px; /* Adjust size as needed */
    height: auto;
    transition: transform 0.1s; /* Smooth movement */
}
```

#### JavaScript for Movement
Here's the JavaScript that handles the ghost's movement based on keyboard inputs.

```javascript
const ghost = document.getElementById('ghost');
let ghostPosition = { top: 0, left: 0 };

document.addEventListener('keydown', (event) => {
    const step = 10; // Movement step in pixels

    if (event.key === 'ArrowUp') {
        ghostPosition.top -= step;
    } else if (event.key === 'ArrowDown') {
        ghostPosition.top += step;
    } else if (event.key === 'ArrowLeft') {
        ghostPosition.left -= step;
    } else if (event.key === 'ArrowRight') {
        ghostPosition.left += step;
    }

    ghost.style.transform = `translate(${ghostPosition.left}px, ${ghostPosition.top}px)`;
});
```

### Key Points
- **Keyboard Input**: We used `keydown` event listeners to detect when the arrow keys are pressed.
- **Movement**: The ghost moves in response to the keys pressed, adjusting its position with CSS transforms.
- **Smooth Animation**: The transition property in CSS allows for a smooth visual movement of the ghost.
