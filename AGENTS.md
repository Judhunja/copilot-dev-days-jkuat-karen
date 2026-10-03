# AGENTS.md

## Project overview
This repository is a small static web app: a single-page space exploration quiz built in one HTML file, with no build step, no package installation, and no server requirement.

## Working conventions
- Keep the app self-contained in `index.html` unless a user explicitly asks for new files.
- Preserve the current visual design language: centered narrow card layout, accessible typography, and light/dark theme support through `prefers-color-scheme`.
- Prefer CSS variables for theme colors and polished control-panel styling over ad-hoc hard-coded values.
- Maintain accessibility: readable contrast, visible keyboard focus, and clear feedback states for correct and incorrect answers.
- Do not add dependencies or tooling unless explicitly requested.

## How to validate changes
- Open `index.html` directly in the browser for UI checks.
- Smoke-test the core flow: question rendering, answer selection, score updates, correct/incorrect feedback, and final results screen.
- If you make interaction updates, confirm keyboard navigation still works with Tab/Enter and that the results view still appears correctly.

## Common patterns
- Quiz state should live in simple JavaScript variables and DOM updates.
- Prefer progressive, user-friendly feedback messages rather than silent state changes.
- Keep the experience polished and compact: one narrow column, smooth transitions, and clear visual hierarchy.

## Notes for future agents
- This project is intentionally lightweight; avoid introducing framework or package-based structure unless the user specifically asks for it.
- Treat the quiz as a static front-end exercise, and keep changes minimal and cohesive with the current design.
