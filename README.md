# Scroll Car Animation

A scroll-based hero section recreated using only vanilla HTML, CSS and JavaScript.
As the user scrolls, a top-view car drives across the screen and uncovers the
"WELCOME ITZFIZZ" headline behind it. The road lines rush past, and four
statistics rise into view and count up.

## Features
- Pinned hero section driven entirely by scroll position
- Car movement with a headline reveal that stays in sync via `clip-path`
- Moving road lane markings for a sense of speed
- Staggered stat cards with count-up numbers
- Live speed readout and scroll progress bar
- Smooth, eased motion that is independent of frame rate
- Responsive layout and `prefers-reduced-motion` support

## Tech
HTML5, CSS3, JavaScript (ES6). No libraries or frameworks.

## How it works
Scroll distance is converted to a progress value between 0 and 1. That value is
smoothed with linear interpolation inside a `requestAnimationFrame` loop, and
each effect reads its own slice of it. Animations use `transform` and `opacity`
to stay smooth.

## Run locally
Open `index.html` in any modern browser. No build step is needed.

## Live demo
https://YOUR-USERNAME.github.io/car-scroll-animation/
