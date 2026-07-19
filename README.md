# Solve with Genesis — Website

Four-page static site. Plain HTML + one shared `style.css` — no build step, no framework, no dependencies. Any text editor and a browser is all you need to maintain it.

- `index.html` — Home
- `methodology.html` — How Jonathan approaches every engagement
- `case-studies.html` — Five real engagements, situation/approach/result
- `about.html` — Bio and quick facts
- `style.css` — Shared design system for all four pages

## Before you publish

Search all four files for these and replace with your real details:

- `hello@solvewithgenesis.com` — the email CTA, repeated on every page.
- `Jonathan` — used in the "Email Jonathan" button label throughout. Change if you'd rather it read generically.

## Publish it

**Option A — GitHub Pages (free)**
```bash
cd solve-with-genesis-website
git init && git add -A && git commit -m "Initial four-page site"
git branch -M main
git remote add origin https://github.com/<your-username>/<repo-name>.git
git push -u origin main
```
Then in the repo on GitHub: Settings → Pages → Source → deploy from `main`, `/ (root)`. Point solvewithgenesis.com at the resulting GitHub Pages URL via a CNAME record in GoDaddy DNS.

**Option B — GoDaddy Web Hosting**
If you have a hosting plan (not just the domain), upload all five files to the root of your hosting directory (usually `public_html`) via GoDaddy's File Manager or FTP. That's the whole deployment.

## Extending it

To add a fifth page, copy any existing page as a template, keep the `<link rel="stylesheet" href="style.css">` line, and add a nav link to it in all five files' `<nav class="links">` block.
