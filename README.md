🤖 AI Coding Assignment Evaluator

# AI Coding Assignment Evaluator — Teal UI (Single‑File SPA)

## Overview
This project is a **single HTML file** prototype of an **AI Coding Assignment Evaluator** website.  
It is built as a **multi‑page SPA (Single Page Application)** using **hash routing** (example: `#/home`, `#/demo`) and demonstrates an MVP-style product UI for evaluating coding submissions.

The site is **front-end only** and the “evaluation” output is **mock/simulated** (no backend required).

---

## What’s Updated in This Version
This updated version includes:
- **Teal gradient theme** (matches the “Image #2” teal style)
- Removed the **“Submit Your Assignment”** card (as requested)
- Removed the **hero quick pills** (Evaluate / History / Settings / About)
- **Smooth UI animations**
  - Fade-up section reveals
  - Floating hero icon
  - Shimmer effect on CTA button
  - Hover lift on cards/buttons
- **Responsive navigation**
  - Desktop navbar
  - Mobile menu button + slide-down mobile navigation
- Kept the original SPA pages:
  - Home, Product, How it works, Pricing, About, Demo
- Demo page generates a **structured report**:
  - Overall score
  - Dimension scores (Correctness, Time, Space, Readability, Best Practices)
  - Notes + suggestions
  - Download report as TXT
  - Copy report to clipboard

---

## Pages / Routes
This file uses hash routes. You can navigate via navbar or manually:

- `#/home` — Landing page + sample evaluation card
- `#/product` — Features and example output
- `#/how-it-works` — Evaluation pipeline steps
- `#/pricing` — Pricing plans (illustrative)
- `#/about` — Fairness + use cases
- `#/demo` — Paste GitHub URL / upload file → generate mock report

---

## Demo Evaluator (How It Works)

Demo Link: 
    https://bhargavi2048-boop.github.io/AI-Coding-Assignment-Evaluator/

On the **Demo** page you can:

1. Paste a **GitHub file URL** *or* upload a **code file**
2. Optionally choose a language
3. Select a **rubric profile**
   - Balanced (default)
   - Correctness-focused
   - Readability-focused
4. Add evaluator notes (optional)
5. Click **Generate report**

### Important Notes
- For GitHub URL input, the app does **not fetch GitHub code** (to avoid browser CORS issues).  
  It generates a mock evaluation seed based on the URL so the UI still works offline.
- Uploading a file reads real text from the file and generates a mock score based on simple heuristics.

---

## How to Run
### Option 1 (Simplest)
1. Save the file as: **`AI Coding Assignment Evaluator.html`**
2. Double‑click the file to open in any modern browser (Chrome / Edge / Firefox)

### Option 2 (Recommended)
Run it using a local server (better for consistent behavior):
- VS Code → **Live Server**
- Python:
  ```bash
  python -m http.server
  ```
  Then open: `http://localhost:8000`

---

## Tech Stack
- **HTML + CSS + JavaScript** (all in one file)
- No libraries / no frameworks
- Hash routing (SPA navigation)
- Clipboard + download features for report export

---

## Customization
### Change Theme
Edit the CSS variables in `:root`:
- `--teal`, `--teal-2`, `--teal-3`
- `--header-bg`, `--text`, `--muted`

### Add a New Page
1. Add a route entry in the `routes` object (JS)
2. Create a `<section class="page" id="page-yourpage">...</section>`
3. Add a navbar link: `<a href="#/yourpage" data-link>...</a>`

### Replace Mock Evaluator With Real Backend
In the Demo logic:
- Replace the mock scoring function (`scoreFromText(...)`) with an API call:
  - `fetch("/api/evaluate", ...)`
- Render the returned JSON into the existing report UI structure

---

## Limitations (Current MVP)
- No real code execution or test running
- No real GitHub raw content fetch for URL input (front-end only)
- Scores are simulated/heuristic-based for demonstration

---

## License / Usage
This is a demo/MVP prototype suitable for assignments and portfolio demos.  
You may modify and reuse it for educational purposes.

👩‍💻 Author
Bhargavi N

“Code is like poetry; every line should sing with clarity.”
