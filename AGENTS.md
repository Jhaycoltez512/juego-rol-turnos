# Repository Guidelines

## Project Structure & Module Organization

This repository is a small, dependency-free browser game. The complete application lives in [`index.html`](index.html): semantic markup, visual styles, and the turn-based combat engine are currently embedded in one file. There are no separate source, test, or asset directories yet. Keep future static assets beside `index.html`; split CSS or JavaScript into `style.css` or `game.js` only when the file becomes difficult to maintain.

## Build, Test, and Development Commands

No compilation or package installation is required. Run the local server from the repository root:

```bash
python3 -m http.server 8000
```

Then open `http://localhost:8000`. For a quick syntax/runtime smoke test, load the page in a browser, choose three heroes, start an expedition, and complete at least one turn. GitHub Pages serves the root of `main` and should be checked after changes are pushed.

## Coding Style & Naming Conventions

Use four-space indentation in HTML, CSS, and JavaScript. Prefer semantic HTML, CSS custom properties for shared colors, and `camelCase` for JavaScript variables and functions (`startStage`, `selectedSkill`). Keep user-facing text in Spanish and escape dynamic names before inserting them into HTML. Preserve the current no-build, single-page architecture unless a structural change is justified.

## Testing Guidelines

There is no automated test framework or coverage requirement. Manually test hero selection, skill targeting, guard/end-turn actions, enemy turns, victory, defeat, restart, and responsive layouts after UI or combat changes. Check the browser console for errors.

## Commit & Pull Request Guidelines

Use short imperative commits in Spanish or English, such as `Añade habilidad de escudo` or `Fix target selection`. Keep each commit focused. Pull requests should describe gameplay/UI changes, include manual test steps, link an issue when applicable, and attach screenshots or a short recording for visual changes. Confirm the working tree is clean and that the local server smoke test passes before requesting review.
