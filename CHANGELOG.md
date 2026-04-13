# CHANGELOG — Džiugas AI-Guardian One-Pager

> **Project:** Džiugas AI-Guardian Board Presentation
> **Client:** Žemaitijos Pienas AB (Džiugas brand)
> **Prepared by:** [promptanatomy.app](https://promptanatomy.app)
> **Document:** `index.html`
> **Source of Truth:** `.cursor/rules/dziugas-onepager.mdc`

---

## [v1.7.4] — 2026-04-13

### LT/EN Microcopy Compression & Tone Neutralization

**Changed**
- Shortened and de-romanticized high-impact narrative copy in:
  - `index.html` (LT)
  - `index.en.html` (EN)
- Updated Hero, Brand, Problem, Solution, and Closing principle text blocks to be more factual and scannable.
- Reduced manual-craft/pathos framing and aligned LT/EN semantic parity around operational quality messaging.
- Tightened UI microcopy in both locales:
  - CTA labels (shorter action wording)
  - Section labels and heatmap headings
  - KPI bullet phrasing for faster board-level readability

**Result**
- Clearer, shorter bilingual messaging with less emotional overstatement and stronger consistency across LT/EN pages.

---

## [v1.7.3] — 2026-04-13

### Repository Publish & Remote Sync

**Changed**
- Published project to remote repository:
  - `https://github.com/Dipukas/dziugas`
- Pushed `main` branch and enabled upstream tracking (`main -> origin/main`).
- Included deployment workflow and static site assets in the initial remote history.

**Result**
- Repository is now live on GitHub and ready for GitHub Actions Pages deployment runs.

---

## [v1.7.2] — 2026-04-13

### Accessibility & Safer Pages Artifact

**Changed**
- Added keyboard accessibility focus styles (`:focus-visible`) for interactive links in:
  - `index.html`
  - `index.en.html`
- Added graceful fallback for reveal animations when JavaScript is unavailable (`<noscript>` visibility override).
- Added reduced-motion support (`prefers-reduced-motion`) to disable animation transitions for accessibility-sensitive users.
- Updated GitHub Pages workflow to publish a curated public artifact (`_site`) instead of the full repository.

**Result**
- Better keyboard and no-JS resilience for both locales.
- Lower risk of publishing non-public project files through Pages deploy.

---

## [v1.7.1] — 2026-04-13

### Deploy Readiness & Asset Stabilization

**Changed**
- Audited local asset links in `index.html` and `index.en.html` to ensure deploy-safe paths.
- Bumped localized page meta versions to `1.7.1` in:
  - `index.html`
  - `index.en.html`
- Synchronized project metadata files to current release:
  - `docs/STATUS.md`
  - `docs/manifest.json`

**Added**
- `README.md` with project structure, local preview instructions, and GitHub Pages URL.
- `.gitignore` for OS/editor noise.
- `.github/workflows/deploy-pages.yml` for automatic GitHub Pages deployment on `main`.
- `assets/logo-pa.svg` and `assets/hero-ripening.svg` as optional local fallback visuals.

**Result**
- Repository is deployment-ready for GitHub Pages with automated workflow and aligned project documentation.

---

## [v1.7.0] — 2026-04-13

### Premium SaaS Visual Polish (Kiss/Marry/Kill Implementation)

**Changed**
- Implemented full visual polish pass in `index.html` focused on premium SaaS UX quality, while preserving content intent and section architecture.
- Navigation upgraded with in-page wayfinding links (`#brand`, `#problem`, `#solution`, `#strategy`, `#pilot`, `#principle`) and a persistent nav CTA.
- Conversion flow aligned to one consistent primary intent (`mailto:hello@promptanatomy.app`) across nav, hero, mid-page, and closing CTAs.
- Hero first-read experience stabilized:
  - Above-the-fold content no longer depends on reveal state for initial visibility.
  - Trust bar weight reduced to keep focus on headline/value/CTA hierarchy.
- Refactored inline styling into reusable classes for section intros, proof eyebrows, timeline labels, strategy phase variants, and heatmap presentation.
- Localized LT `#pilot` proof block microcopy that previously mixed EN/LT labels (case metrics and key labels now consistently Lithuanian).

**UX / Design System**
- Added responsive nav behavior improvements for smaller viewports (compact top bar priorities).
- Added section `scroll-margin-top` to prevent fixed-nav anchor clipping.
- Improved small-label readability in proof/KPI blocks (`11px` class usage raised where needed for better contrast legibility).
- Reduced decorative noise by softening divider prominence and centralizing repeated visual patterns into class-based components.

**Result**
- Cleaner premium presentation, clearer navigation/orientation, and more consistent conversion journey, with stronger maintainability from reduced inline style fragmentation.

---

## [v1.6.1] — 2026-04-13

### LT Grammar Polish (Hero)

**Changed**
- Updated Lithuanian hero phrasing in `index.html`:
  - `Džiugas ratai` → `Džiugo ratai`
- Bumped `index.html` document meta version to `1.6.1`.

**Result**
- More natural Lithuanian grammar in the first-read hero sentence while preserving meaning.

---

## [v1.6.0] — 2026-04-13

### UI/UX Microcopy Refinement (LT + EN)

**Changed**
- Applied prioritized microcopy improvements from the bilingual UX audit in:
  - `index.html` (LT)
  - `index.en.html` (EN)
- Strengthened primary action clarity in Hero and Closing CTAs:
  - LT: `Peržiūrėti 3 etapų pilotinį planą`, `Suderinti 30 min. pokalbį dėl piloto`
  - EN: `View the 3-phase pilot plan`, `Book a 30-minute pilot discussion`
- Improved clarity and consistency in key sections:
  - Hero risk phrasing, Problem framing, timeline risk labels
  - Solution intro wording (`AI` instead of more technical `neural` framing)
  - Benefits and strategy objective phrasing for board-level readability
- Updated trust/legal/accessibility microcopy:
  - PGI/SGN trust-label wording in LT/EN
  - Footer legal line adjusted to internal-use wording in both locales
  - Accessibility labels refined (`aria-label`) for better language consistency
- Bumped localized page meta version to `1.6.0`.

**Result**
- Faster first-read comprehension, clearer action intent, and tighter EN/LT semantic parity while preserving content meaning and page architecture.

---

## [v1.5.2] — 2026-04-13

### Responsive Hero Image Variants (`srcset`)

**Added**
- Generated responsive hero image assets from `main_photo.png`:
  - `main_photo-640.jpg`
  - `main_photo-1024.jpg`
  - `main_photo-1536.jpg`

**Changed**
- Updated hero image in `index.html` and `index.en.html` to use:
  - `srcset` for responsive source selection
  - `sizes` matching the hero media container width
  - `main_photo-1024.jpg` as balanced default source

**Result**
- Faster loading on mobile and improved bandwidth efficiency while preserving desktop visual quality.

---

## [v1.5.1] — 2026-04-13

### Hero Visual Integration (`main_photo.png`)

**Added**
- Hero image card integrated into both localized pages:
  - `index.html` (LT)
  - `index.en.html` (EN)
- Responsive `.hero-media` component with:
  - 16:9 aspect ratio
  - rounded premium container with accent border
  - subtle gradient overlay for visual consistency and text harmony

**UX / Performance**
- Hero image configured for above-the-fold loading (`loading="eager"`, `fetchpriority="high"`)
- `object-fit: cover` and centered cropping for stable responsive rendering
- Print mode adjusted to hide hero media for cleaner board-print output

**Accessibility**
- Localized descriptive `alt` text applied in LT and EN pages

---

## [v1.5.0] — 2026-04-13

### EN+LT Bilingual Rollout (LT Default)

**Added**
- `index.en.html` as dedicated English route
- `index.lt.html` as Lithuanian entry route alias to the default page
- LT/EN language switch control in top navigation of localized pages

**Changed**
- `index.html` converted to Lithuanian-first default experience (`lang="lt"`)
- Lithuanian-localized hero, key section copy, CTA labels, trust labels, and footer legal line
- Navigation attribution and accessibility labels localized for Lithuanian default page
- Document version meta bumped to `1.5.0` in localized pages

**Maintained**
- Existing design system tokens, section architecture, animations, and interaction behavior
- Brand hierarchy consistency: `AI-Guardian by Prompt Anatomy` remains stable across locales
- Footer integration positioning preserved with Prompt Anatomy AI Operating System reference

---

## [v1.4.1] — 2026-04-13

### Footer Consistency + Prompt Anatomy Integration

**Changed**
- Footer brand hierarchy aligned to header voice: `AI-Guardian by Prompt Anatomy` (replaces `Prompt Anatomy · AI-Guardian`)
- Footer legal line extended with integration statement: `Built on Prompt Anatomy AI Operating System`
- Prompt Anatomy website link normalized to `https://www.promptanatomy.app/`

**Added**
- Specific LinkedIn destination for brand presence: `https://www.linkedin.com/company/prompt-anatomy/` (replaces generic LinkedIn root)
- Accessibility polish in footer controls: logo alt text set to `Prompt Anatomy`, clearer link aria labels (`Prompt Anatomy Website`, `Prompt Anatomy LinkedIn`)

**Validated**
- Footer typography and spacing remain consistent with existing nav/footer style system
- `index.html` passes lint checks with no reported issues

---

## [v1.4.0] — 2026-04-13

### Source of Truth & Document Management System

**Added**
- `.cursor/rules/dziugas-onepager.mdc` rewritten as the **single authoritative source of truth** (9 sections: project overview, file map, editing constraints, design system, page architecture, verified brand facts with sources, industry reference, tone rules, version history)
- `CHANGELOG.md` — detailed version history (this file)
- `docs/manifest.json` — machine-readable project manifest with brand facts, assets, design system, version history
- `docs/STATUS.md` — human-readable project dashboard with file map, open items, quality checklist
- Document hierarchy established: cursor rule governs all derived files
- `source_of_truth` field added to `docs/manifest.json`

**Changed**
- Cursor rule glob expanded from `["index.html"]` to `["**/*"]` — applies project-wide
- `index.html` `<meta name="author">`, `<meta name="version">`, `<meta name="date">` tags added for document versioning
- Editing constraint added: version bump required on every `index.html` change, with changelog sync

**Documented**
- Full verified brand facts with source URLs (zpienas.lt, dziugashouse.lt, Dairy Industries Intl., Nasdaq Baltic)
- Complete design system color table (14 tokens)
- Page architecture map (8 sections with IDs)
- Eberle × Gebr. Baldauf industry reference details
- 5-stage Džiugas production process (from dziugashouse.lt)
- All 8 product tiers confirmed: Mild (12mo) through Extra Aged (120mo)

---

## [v1.3.0] — 2026-04-13

### Brand Alignment — Prompt Anatomy × Žemaitijos Pienas Colors

**Changed**
- Accent gold shifted from `#D4AF37` to `#EAB832` to match Prompt Anatomy brand identity (PA lightning bolt icon color)
- Background deepened from `#050505` to `#0A0A0A` for warmer tone matching PA icon aesthetic
- All `rgba(212,175,55,…)` glow/shadow values updated to `rgba(234,184,50,…)` for consistency
- Added `--zp-red: #A61D37` design token for potential Žemaitijos Pienas corporate red usage

**Added**
- `PA-Premium-Icon.png` integrated as navigation and footer logo (replaces generic "D" square)
- Nav title updated: "AI-Guardian **by Prompt Anatomy**"
- Footer branding: "Prompt Anatomy · AI-Guardian"
- Nav attribution styled with lightning bolt accent
- EXCLUSIVE 60mo and SPECIAL AGED 100mo added to aging timeline (from [zpienas.lt/dziugas](https://www.zpienas.lt/dziugas/) product catalog)

**Fixed**
- Mobile timeline marker overflow — now hides 4 of 8 labels on small screens

**Assets**
- `PA-Premium-Icon.png` — Prompt Anatomy lightning bolt icon
- `Untitled design (7).png` — Prompt Anatomy banner (reference)

---

## [v1.2.0] — 2026-04-13

### Responsive & Print Polish

**Added**
- `<meta name="theme-color" content="#0A0A0A">` for mobile browser chrome
- Mobile-responsive timeline marker hiding (`@media max-width: 768px`)

**Fixed**
- Timeline markers overflowing on small viewports

---

## [v1.1.0] — 2026-04-13

### Full Content Build — All Sections Complete

**Added**
- **Hero**: "Where Century-Old Craft Meets Computer Vision." headline, trust bar (Est. 1924, PGI, 90+ Awards, 40+ Markets), single CTA
- **Brand Context**: Legend of Džiugas, 4-ingredient philosophy, Čiurlionis symphonies, business facts grid (1924 / 90+ / 120mo / 1,300+)
- **The Problem**: Three pain-point cards (Ripening Vulnerability, Labor Pressure, Batch Loss Risk) + aging risk timeline visualization (Mild 12mo → Extra 120mo)
- **AI-Guardian Solution**: 3-step pipeline (Capture → Analyze → Act), 3 benefit cards, design principle callout
- **Strategic Priorities**: Core/Strategic/Explore cards replacing MARRY/KISS/KILL, animated investment heatmap (95%/70%/45%)
- **Industry Proof & Pilot Plan**: Eberle × Gebr. Baldauf case study (100% inspection, 24/7 autonomous, full traceability), 3-phase pilot roadmap (3mo/6mo/12mo), success metrics
- **Džiugas Principle**: Closing philosophy + "Begin the Pilot Conversation" CTA
- **Footer**: promptanatomy.app attribution, confidentiality notice
- IntersectionObserver scroll-reveal animations (CSS + minimal JS)
- Animated heatmap bars (triggered on scroll)
- Smooth scroll anchor navigation
- `@media print` styles: white background, black text, no fixed nav, no animations

---

## [v1.0.0] — 2026-04-13

### Project Initialization

**Added**
- `.cursor/rules/dziugas-onepager.mdc` — Cursor rule with brand facts, design tokens, tone guidelines, single-file constraint
- `index.html` — Document skeleton with full CSS design system

**Design System**
- CSS custom properties (design tokens)
- Plus Jakarta Sans (headings) + Inter (body) typography
- Glass-morphism card components
- Gold gradient text utility
- Badge and section-label components
- Reveal animation classes with delay variants

**Verified Brand Facts**
- Founded 1924, Telšiai, Samogitia
- 4 ingredients: summer milk, starter culture, non-animal rennet, salt
- Aged 12–120 months to Čiurlionis and Oginskis symphonies
- EU PGI since 2019, Japan GI proposed 2025
- 90+ international awards (DLG, Crystal Taste, Superior Taste, Anuga)
- Parent: Žemaitijos Pienas AB, Nasdaq Vilnius, 1,300+ employees
- Godparents: President Valdas Adamkus and Alma Adamkienė (2010)
