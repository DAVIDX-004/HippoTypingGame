# HippoType

A typing speed game that measures how fast and accurately you can type under a 30 second timer.

![HippoType screenshot](final.png)

## Try it

**[Play HippoType here](https://davidx-004.github.io/HippoTypingGame/)** — no install needed.

## Features

- 30 second timed typing rounds
- Live feedback: correct letters turn green, mistakes turn red as you type
- Automatic WPM (words per minute) score at the end of each round
- New game button to instantly restart and chase a better score
- Backspace support so you can fix mistakes mid-word
- Neon cyberpunk themed UI with a glowing typing cursor

## Run it locally

1. Clone or download this repo
2. Open `index.html` in any browser
3. Click the text area to focus, and start typing

There are no dependencies, no build step, and no server required. Everything runs in the browser with plain HTML, CSS and JavaScript.

## How it works

The word list is rendered as individual letter spans inside each word, which lets the game track keystrokes at the letter level instead of comparing whole strings. On every keypress the game compares the typed character against the expected letter, marks it correct or incorrect, and moves the cursor. Words only count toward your WPM if every letter in them was typed correctly.

The timer starts on your first keystroke rather than when the page loads, so your score reflects your actual typing time. Scrolling works by measuring the current word's position and shifting the word container upward one line at a time, which keeps the cursor always on a visible line.

## Credits

- Fonts: [Orbitron](https://fonts.google.com/specimen/Orbitron) and [JetBrains Mono](https://fonts.google.com/specimen/JetBrains+Mono) via Google Fonts
- Hippo icon from [Font Awesome](https://fontawesome.com)

