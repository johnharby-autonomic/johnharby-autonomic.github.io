# Autonomic AI, LLC - static site

Clean, self-contained static version of functormodel.ai. No Wix, no external
dependencies, no tracking. One shared stylesheet (styles.css) drives every page.

## Deploy to GitHub Pages
1. Copy everything in this folder into your repo
   (johnharby-autonomic.github.io), at the repo root.
2. Commit and push.
3. In the repo: Settings > Pages > Build from branch > main / root.
4. Your custom domain (functormodel.ai) goes in Settings > Pages > Custom domain.
   Add a CNAME record at your DNS: www -> johnharby-autonomic.github.io.

## Structure
- index.html plus one .html file per page
- styles.css  (edit colors/fonts here, applies site-wide)
- images/     (page images extracted from the originals, available if you
              want to place any; pages are currently text-focused and clean)

## Still needed
These two pages are linked in the nav/footer but were not in the upload set,
so their links will 404 until added: benchmark.html, customers.html.
Send those two saved pages and they drop straight in.
