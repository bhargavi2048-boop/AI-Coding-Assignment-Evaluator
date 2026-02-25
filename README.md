🤖 AI Coding Assignment Evaluator

# AI Coding Assignment Evaluator (Single‑File SPA)

A front‑end-only prototype of an AI Coding Assignment Evaluator UI. Built as a **single HTML file** with **hash-based SPA routing** to demonstrate an MVP workflow for evaluating coding submissions and generating a rubric-style report.

> Note: This version is UI-only. The “evaluation” is **mock/simulated** (no backend required).

---

## Live Demo

- Demo:
       https://bhargavi2048-boop.github.io/AI-Coding-Assignment-Evaluator/

---

## Key Features

- **Teal gradient UI theme** with consistent design tokens
- **Single‑file SPA** (HTML + CSS + JavaScript in one file)
- **Hash routing navigation** (example: `#/home`, `#/demo`)
- Smooth UI polish:
  - Fade‑up section reveals
  - Floating hero icon
  - CTA shimmer effect
  - Hover lift on cards/buttons
- **Responsive navigation**
  - Desktop navbar
  - Mobile menu button + mobile navigation panel
- Demo evaluator (mock):
  - Accepts **GitHub file URL** (seeded mock evaluation)
  - Accepts **uploaded code file** (reads real file content)
  - Generates a structured evaluation report:
    - Overall score
    - Correctness
    - Time Efficiency
    - Space Efficiency
    - Readability
    - Best Practices
    - Notes + suggestion
  - Export options:
    - **Download report as TXT**
    - **Copy report to clipboard**

---

## What’s Updated in This Version

- Teal gradient theme (matches the reference teal style)
- Removed:
  - The “Submit Your Assignment” card
  - Hero quick pills (Evaluate / History / Settings / About)
- Improved animation + interaction polish
- Kept the original SPA pages:
  - Home, Product, How it works, Pricing, About, Demo

---

## Pages / Routes

This project uses hash routes. You can navigate via the UI or manually:

- `#/home` — Landing page + sample evaluation card  
- `#/product` — Features and example output  
- `#/how-it-works` — Evaluation pipeline steps  
- `#/pricing` — Pricing plans (illustrative)  
- `#/about` — Fairness + use cases  
- `#/demo` — Paste GitHub URL / upload file → generate mock report  

---

## Demo Evaluator (How It Works)

On the Demo page you can:

1. Paste a GitHub file URL **or** upload a code file  
2. (Optional) Choose a language  
3. Select a rubric profile:
   - Balanced (default)
   - Correctness‑focused
   - Readability‑focused
4. Add evaluator notes (optional)  
5. Click **Generate report**  
6. Copy or download the generated report

### Important Notes

- For **GitHub URL input**, the app does **not** fetch GitHub file contents (to avoid browser CORS issues).  
  Instead, it generates a mock evaluation “seed” based on the URL so the UI works offline.
- For **file uploads**, the app reads real text from the uploaded file and produces a mock score using simple heuristics.

---

## Tech Stack

- HTML + CSS + JavaScript (single file)
- No libraries / no frameworks
- Hash routing (SPA navigation)
- Clipboard API + download export for report output

---

## Project Structure

This repository is intentionally minimal:

- `index.html` — Entire SPA (UI, styles, routing, demo evaluator logic)

---

## How to Run Locally

### Option 1 — Open the file directly
1. Save/open the HTML file (example: `hks.html`)
2. Double‑click to open in a modern browser (Chrome / Edge / Firefox)

### Option 2 — Run with a local server (recommended)
Using a local server can be more consistent across browsers.

**VS Code**
- Use the “Live Server” extension

**Python**
```bash
python -m http.server
```

Then open:
- http://localhost:8000

---

## Deployment (GitHub Pages)

This project can be deployed via GitHub Pages by serving the HTML file from the repository (commonly from the `main` branch).  
The live demo link above is an example deployment.

---

## Customization Guide

### Change Theme
Edit CSS variables in `:root`, for example:

- `--teal`, `--teal-2`, `--teal-3`
- `--header-bg`, `--text`, `--muted`

### Add a New Page
1. Add a route entry in the `routes` object (JavaScript)
2. Create a new page section:
   - `<section class="page" id="page-yourpage"> ... </section>`
3. Add a navigation link:
   - `<a href="#/yourpage" data-link>...</a>`

### Replace Mock Evaluator With a Real Backend
In the Demo logic:
- Replace the mock scoring function (`scoreFromText(...)`) with an API call, e.g.:
  - `fetch("/api/evaluate", ...)`
- Render the returned JSON into the existing report UI structure

---

## Limitations (Current MVP)

- No real code execution or sandboxed test running
- No GitHub raw content fetch for URL input (front‑end only)
- Scores are heuristic/simulated for demonstration

---

## Roadmap (Optional Enhancements)

- Fetch GitHub raw file content server‑side (avoid CORS)
- Add a backend runner (Docker sandbox) to run tests securely
- Rubric editor (custom weights per dimension)
- Export as PDF
- Optional similarity detection module (neutral “review recommended” tone)

---

## Author

**Bhargavi N**

 “Code is like poetry; every line should sing with clarity.”

---

## License

This is a demo/MVP prototype suitable for assignments and portfolio demos.  
You may modify and reuse it for educational purposes.
