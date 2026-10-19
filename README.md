# JS DOM & Async Demos

A small collection of vanilla JavaScript demos covering DOM events, timers, and asynchronous flows.

## Features

- **Color switcher** — changes the page background color every second while active; Start/Stop buttons toggle the interval
- **Countdown timer** — pick a date/time with a `flatpickr` date picker and count down to it, updating every second
- **Promise generator** — generates a configurable number of promises with incrementally increasing delays and reports each resolution/rejection via `izitoast` notifications

## Technology

- Vanilla JavaScript (ES modules)
- Vite build tooling
- flatpickr for date selection
- izitoast for notifications
- GitHub Actions workflow deploying the production build to GitHub Pages

## Project structure

```
src/
  01-color-switcher.html / js/01-color-switcher.js
  02-timer.html          / js/02-timer.js
  03-promises.html       / js/03-promises.js
  css/common.css
  index.html             Links to all three demos
```

## Commands

```
npm install     # install dependencies
npm run dev     # start the Vite dev server
npm run build   # build for production (GitHub Pages base path)
npm run preview # preview the production build
```

## Deployment

Pushes to `main` trigger a GitHub Actions workflow that builds the project and deploys the `dist` output to the `gh-pages` branch for GitHub Pages.
