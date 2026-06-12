# First-Time Setup & Deployment

This walks you through publishing ProteinPlate to **https://lgtkgtv.github.io/protein-plate/** for free. No prior web-hosting experience needed.

## Step 1 — Create the GitHub repository

1. Go to <https://github.com/new>.
2. **Repository name:** `protein-plate`
3. Visibility: **Public**. Do **not** add a README/license/.gitignore (this folder already has them).
4. Click **Create repository**.

## Step 2 — Push this folder to GitHub

From inside this `protein-plate/` folder on your computer:

```bash
git init
git add .
git commit -m "Initial commit: ProteinPlate guide"
git branch -M main
git remote add origin https://github.com/lgtkgtv/protein-plate.git
git push -u origin main
```

## Step 3 — Allow the action to publish

The included workflow needs permission to push the built site.

1. In your repo: **Settings → Actions → General**.
2. Under **Workflow permissions**, choose **Read and write permissions** → **Save**.

(If you already pushed before doing this, re-run the workflow: **Actions** tab → latest run → **Re-run jobs**.)

## Step 4 — Turn on GitHub Pages

The workflow builds your site and pushes it to a branch called `gh-pages`.

1. **Settings → Pages**.
2. **Source:** *Deploy from a branch*.
3. **Branch:** `gh-pages`  ·  **Folder:** `/ (root)`  →  **Save**.

Wait ~1 minute, then open **https://lgtkgtv.github.io/protein-plate/**. Done.

## Everyday workflow after that

Edit any file in `docs/`, then:

```bash
git add .
git commit -m "Update recipes"
git push
```

Every push to `main` rebuilds and republishes the site automatically.

## Preview locally before pushing (optional)

```bash
pip install -r requirements.txt   # installs mkdocs-material
mkdocs serve                      # open http://127.0.0.1:8000
```

## Alternative: one-command manual deploy

If you'd rather not use the GitHub Action, delete `.github/workflows/deploy.yml` and run this from your machine whenever you want to publish:

```bash
mkdocs gh-deploy --force
```

Then do Step 4 once.

## Later: custom domain (proteinplate.org)

When you're ready to spend on a domain, add a one-line `docs/CNAME` file containing `proteinplate.org`, point the domain's DNS to GitHub Pages, and set the custom domain under **Settings → Pages**. No content changes needed. Until then, the free `github.io` URL works perfectly.
