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

DOMAIN 

In your repo on GitHub: **Settings > Pages**, then the **"Custom domain"** field. Type `functormodel.ai`, click **Save**. After it verifies, check **Enforce HTTPS**.

That save also commits a `CNAME` file to your repo root, so don't be surprised when it appears.

Then set DNS at your domain registrar so the domain points to GitHub:

- For the apex `functormodel.ai`: four **A** records to GitHub's Pages IPs: `185.199.108.153`, `185.199.109.153`, `185.199.110.153`, `185.199.111.153`.
- For `www.functormodel.ai`: one **CNAME** record pointing to `johnharby-autonomic.github.io`.

DNS can take a little while to propagate. Once it resolves, GitHub issues the HTTPS certificate automatically, then you can tick Enforce HTTPS. If those exact IPs matter to you, confirm them on GitHub's Pages docs, since they publish the current set.
