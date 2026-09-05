# Broadway: The History of the American Musical — OER Site

A single-page, print-ready website for **Special Topics: Broadway – The History of the American Musical (THE 2076)**, an Open Educational Resource from RRCC Theatre Studies. Content is adapted from *Backstage Pass: A Survey of American Musical Theatre* by Pamyla Stiehl and Bud Coleman (used with permission), and is licensed CC BY-NC-SA.

## What's here

- `index.html` — the full site (no build step, no dependencies beyond two Google Fonts loaded via CDN)
- `assets/Broadway-History-OER-Toolkit.pdf` — the companion PDF version, linked from the site's "Download the PDF" button

## Publish it with GitHub Pages

1. Create a new **public** GitHub repository (e.g. `broadway-oer`).
2. Add these files to the repo root, keeping the `assets/` folder structure intact.
3. Commit and push:
   ```bash
   git init
   git add .
   git commit -m "Add Broadway OER site"
   git branch -M main
   git remote add origin https://github.com/<your-username>/<repo-name>.git
   git push -u origin main
   ```
4. In the repo, go to **Settings → Pages**.
5. Under **Build and deployment**, set **Source** to "Deploy from a branch," choose the `main` branch and `/ (root)` folder, then **Save**.
6. GitHub will publish the site at:
   `https://<your-username>.github.io/<repo-name>/`
   (Usually live within a minute or two.)

## Editing the content

Everything lives in `index.html` — there's no templating layer. Each unit of the course (The Antecedents, The Jazz Age, The Golden Age, etc.) is its own `<section>`, and each historical figure is a collapsible `<details class="figure">` block, so you can add, remove, or reorder entries by copying an existing block and editing the text.

To swap in a different PDF, replace the file in `assets/` and update the filename in the `href` on the "Download the PDF" button near the top of `index.html`.
