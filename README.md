# make-game

A **Pacman-inspired game** featuring characters and elements from *The Simpsons*, built in **pure JavaScript** without any framework or canvas, running at **60 frames per second** using `requestAnimationFrame()`.

## Features

- Classic Pacman-style gameplay
- Characters and visuals inspired by *The Simpsons*
- Smooth 60 FPS rendering using `requestAnimationFrame()`
- No external libraries or frameworks required
- Pure HTML, CSS, and JavaScript
- Dynamic game loop and collision detection

## How It Works

The game grid is built entirely with HTML elements (`div`) and styled via CSS. Each game object (player, enemies, walls, pellets) is represented by DOM elements manipulated directly through JavaScript.

### Game Loop
The game uses `requestAnimationFrame()` to maintain a consistent **60 FPS** rendering loop.
```js
function gameLoop() {
    update();  // Update game logic (player movement, collisions, etc.)
    render();  // Render DOM elements to reflect new game state
    requestAnimationFrame(gameLoop);
}
gameLoop();
```

### Controls
- Arrow keys: Move player
- Escape: Pause game

## Installation
Clone the repository:
```bash
git clone https://github.com/22101986/make-game.git
```


