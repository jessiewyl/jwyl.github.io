# Personal website

Static site. Three files: `index.html`, `styles.css`, and a `pdfs/` folder.

## Adding a project PDF

1. Drop the PDF into `pdfs/` (e.g. `pdfs/astro-research-1.pdf`).
2. The links in `index.html` already point at those filenames — no HTML change
   needed if you use the same names:
   - `pdfs/resume.pdf`
   - `pdfs/jewelry-tryon.pdf`
   - `pdfs/astro-research-1.pdf`
   - `pdfs/astro-research-2.pdf`
3. To add another project, copy a `<div class="project">` block in `index.html`
   and change the title, text, and PDF filename.

## Publishing on GitHub Pages

Create a repo named `jessiewyl.github.io`, then:

    git init
    git add .
    git commit -m "Personal website"
    git branch -M main
    git remote add origin https://github.com/jessiewyl/jessiewyl.github.io.git
    git push -u origin main

In the repo's Settings > Pages, set Source to "Deploy from a branch",
branch `main`, folder `/ (root)`. The site goes live at
https://jessiewyl.github.io

## Local preview

    python3 -m http.server 8000

Then open http://localhost:8000
