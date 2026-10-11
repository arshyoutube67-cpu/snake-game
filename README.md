A polished, dependency-free take on the classic Snake game — built in a single self-contained index.html with vanilla HTML, CSS, and JavaScript. No frameworks, no build step, no external assets.

▶ Play it by opening index.html in any modern browser.

Features
Start / pause / game-over flow — a clean overlay-driven menu system instead of just dropping the player into the game.
Ramping difficulty — the game speeds up smoothly as your score climbs, capped at a sensible maximum so it never becomes unplayable.
Persistent high score — stored in localStorage, so your best run survives page reloads and browser restarts.
Pause / resume — via spacebar, the on-screen pause button, or the menu.
Synthesized sound effects — short "eat" and "game over" tones generated live with the Web Audio API. No audio files, ever.
Particle burst on eat — a subtle glow/particle effect fires each time food is eaten.
Fully responsive controls — arrow keys / WASD on desktop, an on-screen d-pad and swipe gestures on mobile/touch.
Accessibility basics — visible focus states for keyboard navigation, and full support for prefers-reduced-motion.
Neon aesthetic — glowing snake and food, soft grid, gradient title, all rendered on <canvas>.
Controls
Input	Action
Arrow keys / WASD	Move
Space	Pause / resume
Esc	Return to menu
On-screen d-pad / swipe	Move (touch devices)
Tech stack
HTML5 Canvas for rendering the game board.
Vanilla JavaScript (ES6+) for all game logic — no frameworks or libraries.
Web Audio API for procedurally generated sound effects.
localStorage for persisting the high score.
CSS for layout, the neon theme, and responsive/accessible styling.
The entire game — markup, styles, and script — lives in one file, organized into clearly separated concerns: config/constants, persistence, audio, game state & logic, rendering, input handling, and bootstrapping.

Run it
No build tools, no installs, no server required:

# Clone the repo
git clone https://github.com/ecomsagar/neon-snake.git
cd neon-snake

# Open it
open index.html   # macOS
start index.html  # Windows
Or just double-click index.html. It runs entirely client-side and is safe to host as a static page (e.g. GitHub Pages).

Project structure
.
├── index.html   # Everything: markup, styles, and game logic
└── README.md
License
Free to use, modify, and learn from.
