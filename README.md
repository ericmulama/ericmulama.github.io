# Erick Mulama Shituku — Portfolio

Source for my GIS & remote sensing consulting portfolio, published at:

**https://ericmulama.github.io** *(live once GitHub Pages is enabled — see below)*

## Contents

- `index.html` — the site (single page, no build step, no dependencies beyond Google Fonts)
- `images/` — the five map plates used in the Marine Spatial Planning Atlas section

## Publishing this to GitHub Pages

1. Create a new repository on GitHub named **exactly** `<your-username>.github.io` (for a username-root site) — leave it empty, no README/license/gitignore.
2. Upload these files (`index.html` and the `images/` folder) to the repository, either via the GitHub web UI ("Add file → Upload files", drag the whole `images` folder in) or via git:
   ```bash
   git init
   git add .
   git commit -m "Initial portfolio site"
   git branch -M main
   git remote add origin https://github.com/<your-username>/<your-username>.github.io.git
   git push -u origin main
   ```
3. In the repository, go to **Settings → Pages**. Under "Build and deployment", set Source to **Deploy from a branch**, branch `main`, folder `/ (root)`. Save.
4. GitHub builds the site (usually under a minute) and the live URL appears at the top of that Pages settings page — `https://<your-username>.github.io`.

## Updating later

Edit `index.html` directly (it's plain HTML/CSS, no build step), commit, and push — Pages redeploys automatically within a minute or two of every push to `main`.
