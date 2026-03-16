# 🦆 Duck Pond

interactive duck pond. add a duck, feed the ducks, have them migrate.

An interactive watercolor duck pond built with vanilla HTML5 Canvas — no dependencies, no build step.

## Features

- **Click the pond** to add a duck (up to 18)
- **Feed mode** — toss breadcrumbs and watch ducks swim toward them
- **Plant border** — cycle through cattail, lavender, milkweed, and daylily borders
- **Migrate** — send all ducks flying off screen
- Real-time **wave physics** simulation
- Duck **wake ripples** that follow movement
- Ducks avoid each other with **separation steering**

## Live demo

Hosted on GitHub Pages: `(https://aaltheaa.github.io/duckpond/)`

## Running locally

No build step needed — just open `index.html` in a browser:

```bash
open index.html
# or
python3 -m http.server 8000
```

## Deploying to GitHub Pages

1. Push this repo to GitHub (must be public)
2. Go to **Settings → Pages**
3. Set source to **Deploy from branch → main → / (root)**
4. Your site will be live at `https://<username>.github.io/<repo-name>` within ~60 seconds

## Tech

Pure HTML5 Canvas + vanilla JavaScript. The wave simulation runs a discrete 2D wave equation on an 86×48 grid. Duck movement uses steering behaviours (wander, seek, separation) with a signed distance field for smooth boundary repulsion.
