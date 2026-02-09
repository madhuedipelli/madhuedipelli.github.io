# Daily Learning Log

## Quick Start

### 1. Install dependencies
```bash
pip install -r requirements.txt
```

### 2. Run locally
```bash
mkdocs serve
```
Then open `http://localhost:8000` in your browser.

### 3. Build and deploy to GitHub Pages
```bash
mkdocs gh-deploy
```
This automatically builds the site and pushes to the `gh-pages` branch.

## Project Structure
```
├── mkdocs.yml              # MkDocs configuration
├── requirements.txt        # Python dependencies
├── docs/
│   ├── index.md           # Home page
│   ├── dsa/
│   │   └── index.md       # DSA overview
│   └── system-design/
│       └── index.md       # System Design overview
```

## How to add daily logs

### For DSA problems:
Create files in `docs/dsa/` like:
- `docs/dsa/2025-02-09.md` - Daily log with problems solved
- `docs/dsa/arrays.md` - Topic-specific notes

### For System Design:
Create files in `docs/system-design/` like:
- `docs/system-design/2025-02-09.md` - Daily learnings
- `docs/system-design/database-design.md` - Topic-specific notes

Then update `mkdocs.yml` nav section to include new pages.

## GitHub Pages Setup

Make sure your repository settings have:
1. Go to **Settings → Pages**
2. Set **Source** to `Deploy from a branch`
3. Set **Branch** to `gh-pages` and `/root`

Every time you run `mkdocs gh-deploy`, your site updates automatically!
