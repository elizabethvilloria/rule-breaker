# Rule Breaker

A pixel-art temple dungeon whack-a-mole game for your phone. Creatures and relics pop out of the floor, and an AI Oracle keeps changing the rule for what you're allowed to smash.

## How to play

- Read the law on the stone tablet, then smash only what it names.
- **Right smash:** gold, and combos multiply it.
- **Wrong smash:** lose a whole heart.
- **Let a target escape:** lose a quarter heart.
- **Skull bombs:** never smash them. The blast costs 2 hearts.
- A new law appears every 12 seconds, with a short pause to read it.

## The AI

**The Oracle writes the rules.** Claude invents new laws every game, decides which items fit each one, and aims new laws at the ones you keep breaking. The game starts instantly with built-in laws while the AI writes in the background.

**The Oracle studies you.** A live model on your device tracks your speed, accuracy, reaction time per hole, and which decoys fool you. It speeds up when you're fast, slows down when you struggle, shows you more of what tricks you, and puts targets in the spots you reach slowest.

## Run it

Open `index.html` in a browser, or host it with GitHub Pages. It's a single file with no build step.

Note: the AI-written laws only work when the game is opened inside Claude (as a Claude artifact). Anywhere else, the game automatically uses its built-in laws. The adaptive "studies you" AI works everywhere.

## Built with

Plain HTML, CSS and JavaScript. All sprites are hand-made pixel art drawn to canvas at load time.
