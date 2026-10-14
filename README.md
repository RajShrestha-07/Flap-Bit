# Flap Bit

Flap Bit is a small web game. Tap the board, click, or press Space to flap a square "bit" upward, and fly it through the gaps in the pipes without touching them, the ground or the ceiling. Each pipe you pass scores a point, and your best score is saved on your device.

Live demo: https://rajshrestha-07.github.io/Flap-Bit/

Built with: HTML, CSS and JavaScript.

What this project shows: The game is a loop that redraws the screen about 60 times a second using `requestAnimationFrame`. Each frame applies gravity, which adds to the bit's downward speed, and a flap, which sets its speed upward. Then it moves the pipes left and checks for collisions by comparing the bit's position to each pipe's gap. Because frame rates differ between devices, the code scales movement by the time since the last frame, so the game feels the same speed everywhere. The game is drawn on an HTML canvas, and it has states: ready, playing and dead.

What I'm learning from it: I'm studying how the `update` function applies gravity and flaps, how the collision check compares the bit to the pipe gaps, and how the loop uses the time between frames.
