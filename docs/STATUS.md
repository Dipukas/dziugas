# Project Status — Džiugas AI-Guardian

| Field | Value |
|---|---|
| **Client** | Žemaitijos Pienas AB (Džiugas brand) |
| **Project** | AI-Guardian Board Presentation |
| **Prepared by** | promptanatomy.app |
| **Version** | v1.7.8 |
| **Last Updated** | 2026-04-13 |
| **Status** | Active — Deploy-ready |
| **Source of Truth** | `.cursor/rules/dziugas-onepager.mdc` |

---

## File Map

```
03_Dziugas/
├── index.html                         ← LT default page (v1.7.8)
├── index.en.html                      ← EN page (v1.7.8)
├── index.lt.html                      ← LT redirect helper
├── CHANGELOG.md                       ← Version history
├── README.md                          ← Project/deploy documentation
├── .gitignore                         ← Git ignore rules
├── PA-Premium-Icon.png                ← Primary logo used in UI
├── main_photo.png                     ← Source hero image
├── main_photo-640.jpg                 ← Responsive hero image
├── main_photo-1024.jpg                ← Responsive hero image (default)
├── main_photo-1536.jpg                ← Responsive hero image
├── assets/
│   ├── logo-pa.svg                    ← Optional fallback logo
│   └── hero-ripening.svg              ← Optional fallback hero visual
├── docs/
│   ├── manifest.json                  ← Machine-readable project manifest
│   └── STATUS.md                      ← This file
└── .github/
    └── workflows/
        └── deploy-pages.yml           ← GitHub Pages deploy workflow
```

## Deployment Notes

- Static deploy target: GitHub Pages via GitHub Actions.
- Deploy artifact is curated (`_site`) to avoid publishing internal repository files.
- Default route: `/` serves `index.html` (LT).
- Alternative route: `/index.en.html` serves EN page.

## Quality Checklist

- [x] Local asset references are valid (`png/jpg` files present and referenced correctly).
- [x] LT and EN pages point to deploy-safe local assets.
- [x] Metadata version is aligned to `v1.7.8` across active documents.
- [x] Project has baseline repo docs and ignore rules.
- [x] GitHub Pages workflow is present for automatic deploy on `main`.
- [x] Reveal animations have no-JS and reduced-motion accessibility fallbacks.
