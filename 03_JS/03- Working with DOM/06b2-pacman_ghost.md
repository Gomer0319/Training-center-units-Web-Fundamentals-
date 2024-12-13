## Collision Detection: Keep Your Pacman Ghost in Check

### Developmental Outcomes
1. Understand how to detect collisions in a game environment.
2. Learn to implement boundary checks for element movement.
3. Gain familiarity with conditionals in JavaScript for game logic.

### Introduction to Collision Detection
Think of your ghost as a character in a video game. Just like in real life, it needs to be aware of its surroundings to avoid crashing into walls. In this lesson, we will implement collision detection to ensure that our ghost doesn’t wander out of bounds!

### Understanding Collision Logic
To ensure our ghost stays within the game area, we will check its position against the boundaries of the `game-area` div. If the ghost tries to move beyond the limits, we will prevent it from doing so.

### Main Content

#### Updating JavaScript for Collision Detection
We will modify our existing JavaScript code to include collision checks.

```javascript
const gameArea = document.querySelector('.game-area');
const ghost = document.getElementById('ghost');
let ghostPosition = { top: 0, left: 0 };

document.addEventListener('keydown', (event) => {
    const step = 10; // Movement step in pixels
    const gameAreaRect = gameArea.getBoundingClientRect();
    const ghostRect = ghost.getBoundingClientRect();

    if (event.key === 'ArrowUp' && ghostRect.top > gameAreaRect.top) {
        ghostPosition.top -= step;
    } else if (event.key === 'ArrowDown' && ghostRect.bottom < gameAreaRect.bottom) {
        ghostPosition.top += step;
    } else if (event.key === 'ArrowLeft' && ghostRect.left > gameAreaRect.left) {
        ghostPosition.left -= step;
    } else if (event.key === 'ArrowRight' && ghostRect.right < gameAreaRect.right) {
        ghostPosition.left += step;
    }

    ghost.style.transform = `translate(${ghostPosition.left}px, ${ghostPosition.top}px)`;
});
```

### Key Points
- **Collision Detection**: By using the `getBoundingClientRect()` method, we can determine the position and dimensions of the ghost and game area.
- **Boundary Checking**: Before moving the ghost, we check if its new position would fall outside the boundaries of the game area.
- **Gameplay Integrity**: Collision detection ensures a better gaming experience by preventing the ghost from moving off-screen.