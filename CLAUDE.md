# The Granite Centre — Project Context

## About the Business
- **Name:** The Granite Centre
- **Industry:** Premium granite, marble & quartz supply and installation
- **Location:** 2 The Fairway, Harlow, Essex, CM18 6LY
- **Phone:** 01279 443081 (international: +44 1279 443081)
- **Email:** sales@thegranitecentre.co.uk
- **Speciality:** Kitchen worktops (primary), bathroom vanities, flooring, bespoke cut-to-size

## Project
Single-page website homepage (`index.html`) modelled on krantzdesigns.co.uk but adapted for granite supply.

**Tech stack:** Plain HTML + CSS + JS — no frameworks, no build tools. Opens directly in browser.

## Files
| File | Purpose |
|---|---|
| `index.html` | Main website — all HTML, CSS and JS in one file |
| `logo.png` | Company logo — dark mark on white background |
| `dark-granite.jpg` | Hero section background image |
| `about-granite.jpg` | About section right panel — close-up granite texture |
| `kitchen-worktop.jpg` | Product feature section — kitchen worktop scene |
| `light-granite.JPG` | Second parallax banner background |

## Design System
| Token | Value | Usage |
|---|---|---|
| `--bg` | `#111111` | Main background |
| `--bg2` | `#1a1a1a` | Section backgrounds |
| `--bg3` | `#222222` | Card/panel backgrounds |
| `--text` | `#f5f0eb` | Body text (warm white) |
| `--muted` | `#a89f95` | Secondary text |
| `--gold` | `#c9a96e` | Accent / brand colour |
| `--gold-lt` | `#dfc08a` | Hover state for gold |
| `--border` | `rgba(201,169,110,0.25)` | Subtle gold borders |

**Fonts:** `Playfair Display` (headings, serif) + `Inter` (body, sans-serif) — loaded from Google Fonts

## Logo Usage
The logo PNG has a white background (not transparent). To render white on dark backgrounds:
- `filter: invert(1)` — flips dark mark to white
- `mix-blend-mode: screen` — makes the black background transparent
- Nav logo: `height: 66px`
- Footer logo: `height: 52px`
- Hero badge (bottom-right): `width: 320px`, `opacity: 0.85`

## Page Sections (in order)
1. **Top bar** — phone number + "Request a Quote" CTA
2. **Nav** — sticky, logo image + 5 nav links + hamburger (mobile)
3. **Hero** — full-viewport, `dark-granite.jpg` background, headline, 2 CTAs, logo badge bottom-right
4. **Three Pillars** — Precision Cut / Naturally Beautiful / Expert Installation
5. **About** — text left, `about-granite.jpg` right, "Natural Granite" label
6. **Product Feature** — `kitchen-worktop.jpg` left, Kitchen Worktops content right
7. **Why Choose Us** — 3 numbered items (01 Unmatched Selection, 02 Complete Service, 03 Guaranteed Quality)
8. **Testimonials** — 3 quote cards, dark background
9. **Contact/Quote Form** — name, phone, email, project type, budget, message
10. **Footer** — logo, nav links, product links, contact details, social icons

## Preferences
- British English spelling throughout
- Dark & premium aesthetic — avoid anything that looks "light" or "clean"
- Gold (`#c9a96e`) is the only accent colour — do not introduce other colours
- All edits to `index.html` only unless a new page is explicitly requested
- Always preview changes using the "Granite Centre" server (port 3000)

## Design Guardrails
- **Invoke the `frontend-design` skill** before writing any frontend code, every session
- **Colours:** Never introduce new colours — only use the design system tokens above
- **Shadows:** Never flat shadows. Use layered, dark-tinted shadows (e.g. `0 2px 8px rgba(0,0,0,0.3), 0 8px 32px rgba(0,0,0,0.5)`)
- **Typography:** Playfair Display for headings, Inter for body — never the same font for both. Tight tracking (`-0.03em`) on large headings, generous line-height (`1.7`) on body
- **Gradients:** Layer multiple dark gradients for depth and premium feel
- **Animations:** Only animate `transform` and `opacity`. Never `transition-all`. Use smooth easing
- **Interactive states:** Every clickable element needs hover, focus-visible, and active states
- **Images:** Dark gradient overlays on all hero/banner images to maintain premium dark feel
- **Spacing:** Use the existing spacing patterns — not random values
- **Depth:** Surfaces should feel layered (base `#111` → elevated `#1a1a` → floating `#222`)

## Hard Rules
- Do not add sections or content not requested
- Do not "improve" existing design unprompted — only change what is asked
- Do not use `transition-all`
- Do not introduce colours outside the design system
- British English only
