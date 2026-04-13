# Džiugas AI-Guardian One-Pager

Static board presentation website for the Džiugas brand (Žemaitijos Pienas AB), prepared by promptanatomy.app.

## Project Structure

- `index.html` - Lithuanian default page (`/`)
- `index.en.html` - English page (`/index.en.html`)
- `index.lt.html` - helper redirect to LT default page
- `PA-Premium-Icon.png` - primary logo asset
- `main_photo-*.jpg` - responsive hero assets
- `assets/logo-pa.svg` and `assets/hero-ripening.svg` - optional fallback visuals
- `.github/workflows/deploy-pages.yml` - GitHub Pages deployment workflow

## Local Preview

No build step is required. Open `index.html` directly in a browser.

For a local server (optional):

```powershell
python -m http.server 8080
```

Then open `http://localhost:8080`.

## GitHub Pages Deploy

This repository is configured for automatic GitHub Pages deploy via GitHub Actions on each push to `main`.
The workflow publishes a curated `_site` artifact (public pages + required assets only).

After first successful workflow run, the site URL will be:

- `https://dipukas.github.io/dziugas/`

## First Upload Commands

Run these commands in project root:

```powershell
git init
git checkout -b main
git add .
git commit -m "Initial project import with GitHub Pages deploy setup"
git remote add origin https://github.com/Dipukas/dziugas.git
git push -u origin main
```

Then in GitHub repository settings:

- `Settings -> Pages -> Source` should be set to **GitHub Actions**.

## Smoke Test Checklist

- Open `https://dipukas.github.io/dziugas/` and verify LT page loads.
- Open `https://dipukas.github.io/dziugas/index.en.html` and verify EN page loads.
- Confirm hero image and logo load correctly.
- Confirm no broken links in top navigation and CTA buttons.

## Notes

- This is a static project (no Node.js, no bundler, no framework).
- Version history is tracked in `CHANGELOG.md`.
