# Microsoft Events — Static Website

A pixel-perfect, responsive Microsoft Events website built with **HTML + CSS only** (no JavaScript). Every interaction — dropdowns, hamburger menu, carousels, filter chips, accordion filters — is powered entirely by CSS.

## Pages

| Page | File | Description |
|------|------|-------------|
| Home | `index.html` | 15-section landing page: hero, event finder, featured events, category carousel, upcoming events carousel, industry events, sponsor, learning, next steps, footer |
| Search | `search.html` | Warm-cream search page with gradient decoration |
| Browse Catalog | `search-catalog.html` | Sidebar accordion filters + 3-column event card grid with pagination |
| Event Detail | `event-detail.html` | Individual event page (Microsoft Build 2026) with detail sidebar |

## CSS-Only Interactions

- **Hamburger menu**: `<input type="checkbox">` + `:checked ~ .nav`
- **Dropdowns**: Parent `:hover` / `:focus-within` shows absolute child
- **Mega dropdown**: `position: static` on parent, full-width absolute child
- **Filter chips**: Hidden `<input type="radio">` + `<label>`, `:checked + .chip` toggles
- **Carousels**: `overflow-x: auto; scroll-snap-type: x mandatory`
- **Sidebar accordions**: `<details>/<summary>`, `details[open] .plus-icon { transform: rotate(45deg) }`
- **Active sub-nav**: `:target` + `:has()` selectors

## Design Tokens

| Token | Value |
|-------|-------|
| Background | `#ffffff` |
| Warm sections | `#faf5f0` |
| Cool sections | `#eae4f5` |
| Footer bg | `#f2f2f2` |
| Primary text | `#1b1534` |
| Accent | `#6b2fa0` |
| Link blue | `#0067b8` |

## Responsive Breakpoints

- **Desktop**: 1200px+
- **Tablet**: 768–1199px (hamburger activates at 900px)
- **Mobile**: < 768px
- **Small mobile**: < 480px

## Structure

```
microsoft-events/
├── index.html
├── search.html
├── search-catalog.html
├── event-detail.html
├── README.md
└── assets/
    ├── css/
    │   └── styles.css
    └── img/
        └── partner-logos/
```

## Quick Start

Open `index.html` in any modern browser. No build step or server required.
