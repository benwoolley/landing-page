# CLAUDE.md

This file documents the codebase structure, conventions, and development workflows for AI assistants working in this repository.

## Project Overview

This is a static landing page built as part of [The Odin Project](https://www.theodinproject.com/) web development curriculum. The project is a pure HTML/CSS exercise — no build tools, no frameworks, no JavaScript required unless added intentionally.

## Repository Structure

```
landing-page/
├── README.md       # Project description
├── CLAUDE.md       # This file
├── index.html      # Main entry point (to be created)
└── style.css       # Stylesheet (to be created)
```

> The project is in its initial state. `index.html` and `style.css` are the expected deliverables.

## Tech Stack

- **HTML5** — semantic markup
- **CSS3** — layout via Flexbox or CSS Grid
- No JavaScript unless explicitly added
- No build pipeline, bundler, or package manager
- No external CSS frameworks (e.g. Bootstrap) unless explicitly requested

## Development Conventions

### HTML
- Use semantic elements (`<header>`, `<main>`, `<section>`, `<footer>`, etc.)
- One `index.html` at the root — no subdirectory routing
- Keep markup clean and minimal; avoid unnecessary wrapper `<div>`s
- Use lowercase element and attribute names

### CSS
- Single `style.css` file at the root (or linked from `index.html`)
- Prefer Flexbox for layout; CSS Grid is also appropriate for two-dimensional layouts
- Use CSS custom properties (`--variable-name`) for repeated values like colours and fonts
- Mobile-first responsive design is encouraged but not strictly required by the curriculum task
- No `!important` unless overriding third-party styles

### File Naming
- All lowercase, hyphens as separators (e.g. `style.css`, `hero-image.png`)
- Images go in an `images/` or `assets/` subdirectory if more than one or two assets are used

## Key Workflows

### Running Locally
Open `index.html` directly in a browser — no server required:
```bash
open index.html        # macOS
xdg-open index.html    # Linux
start index.html       # Windows
```

Or use any simple static server:
```bash
python3 -m http.server 8080
# then visit http://localhost:8080
```

### No Build Step
There is no compilation, transpilation, or bundling. Edit HTML/CSS and refresh the browser.

### No Tests
There is no test suite. Correctness is verified visually in a browser.

## Git Conventions

- Commit messages should be clear and descriptive (e.g. `Add hero section with flexbox layout`)
- Work on feature branches; merge to `main` via pull request
- Do not commit build artefacts or OS files (`.DS_Store`, `Thumbs.db`)

## AI Assistant Guidelines

- **Do not introduce a build tool, package manager, or framework** unless the user explicitly asks for one. This is a plain HTML/CSS project.
- **Do not add JavaScript** unless the user requests it.
- **Do not create new files** beyond `index.html`, `style.css`, and an `images/` directory unless asked.
- When generating HTML, use semantic elements and avoid empty structural `<div>`s.
- When editing CSS, respect the existing naming conventions and avoid inline styles.
- If the user asks to "make it look like The Odin Project design", refer to the project's reference screenshot/design spec if one is provided — do not invent a design.
- Keep changes minimal and focused: a request to fix a layout bug should not also refactor unrelated sections.
