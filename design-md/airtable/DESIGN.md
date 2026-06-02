---
version: alpha
name: Airtable-design-analysis
description: A sober, editorial workflow-software interface anchored on white canvas and dark-ink type, where brand voltage comes from full-bleed signature cards in coral, dark green, peach, and dark navy. Haas Grotesk at modest weights. Color-block-first elevation. Generous whitespace. Demo grids with product UI fragments.

colors:
  primary: "#181d26"
  primary-active: "#0d1218"
  ink: "#181d26"
  body: "#333840"
  muted: "#41454d"
  hairline: "#dddddd"
  border-strong: "#9297a0"
  canvas: "#ffffff"
  surface-soft: "#f8fafc"
  surface-strong: "#e0e2e6"
  surface-dark: "#181d26"
  signature-coral: "#aa2d00"
  signature-forest: "#0a2e0e"
  signature-cream: "#f5e9d4"
  signature-peach: "#fcab79"
  signature-mint: "#a8d8c4"
  on-primary: "#ffffff"
  on-dark: "#ffffff"
  link: "#1b61c9"
  link-active: "#1a3866"

typography:
  display-xl:
    fontFamily: "Haas Groot Disp, Haas, sans-serif"
    fontSize: 48px
    fontWeight: 500
    lineHeight: 1.1
    letterSpacing: 0
  display-lg:
    fontFamily: "Haas Groot Disp, Haas, sans-serif"
    fontSize: 40px
    fontWeight: 400
    lineHeight: 1.2
    letterSpacing: 0
  display-md:
    fontFamily: "Haas Groot Disp, Haas, sans-serif"
    fontSize: 32px
    fontWeight: 400
    lineHeight: 1.2
    letterSpacing: 0
  title-lg:
    fontFamily: "Haas, sans-serif"
    fontSize: 24px
    fontWeight: 400
    lineHeight: 1.35
    letterSpacing: 0.12px
  title-md:
    fontFamily: "Haas Groot Disp, Haas, sans-serif"
    fontSize: 20px
    fontWeight: 400
    lineHeight: 1.5
    letterSpacing: 0
  label-md:
    fontFamily: "Haas, sans-serif"
    fontSize: 16px
    fontWeight: 500
    lineHeight: 1.4
    letterSpacing: 0
  button:
    fontFamily: "Haas, sans-serif"
    fontSize: 16px
    fontWeight: 500
    lineHeight: 1.4
    letterSpacing: 0
  body-md:
    fontFamily: "Haas, sans-serif"
    fontSize: 14px
    fontWeight: 400
    lineHeight: 1.25
    letterSpacing: 0
  caption:
    fontFamily: "Haas, sans-serif"
    fontSize: 14px
    fontWeight: 500
    lineHeight: 1.35
    letterSpacing: 0.16px

rounded:
  xs: 2px
  sm: 6px
  md: 10px
  lg: 12px
  pill: 9999px
  full: 9999px

spacing:
  xxs: 4px
  xs: 8px
  sm: 12px
  md: 16px
  lg: 24px
  xl: 32px
  xxl: 48px
  section: 96px

components:
  button-primary:
    backgroundColor: "{colors.primary}"
    textColor: "{colors.on-primary}"
    typography: "{typography.button}"
    rounded: "{rounded.lg}"
    padding: 16px 24px
  button-primary-active:
    backgroundColor: "{colors.primary-active}"
    textColor: "{colors.on-primary}"
    rounded: "{rounded.lg}"
  button-secondary:
    backgroundColor: "{colors.canvas}"
    textColor: "{colors.ink}"
    typography: "{typography.button}"
    rounded: "{rounded.lg}"
    padding: 16px 24px
  text-link:
    backgroundColor: transparent
    textColor: "{colors.link}"
    typography: "{typography.body-md}"
  top-nav:
    backgroundColor: "{colors.canvas}"
    textColor: "{colors.ink}"
    typography: "{typography.body-md}"
    height: 64px
  hero-band:
    backgroundColor: "{colors.canvas}"
    textColor: "{colors.ink}"
    typography: "{typography.display-lg}"
    padding: 96px
  signature-coral-card:
    backgroundColor: "{colors.signature-coral}"
    textColor: "{colors.on-primary}"
    typography: "{typography.display-md}"
    rounded: "{rounded.lg}"
    padding: 48px
  signature-forest-card:
    backgroundColor: "{colors.signature-forest}"
    textColor: "{colors.on-primary}"
    typography: "{typography.display-md}"
    rounded: "{rounded.lg}"
    padding: 48px
  hero-card-dark:
    backgroundColor: "{colors.surface-dark}"
    textColor: "{colors.on-dark}"
    typography: "{typography.display-md}"
    rounded: "{rounded.lg}"
    padding: 48px
  feature-card-tabbed:
    backgroundColor: "{colors.surface-soft}"
    textColor: "{colors.ink}"
    typography: "{typography.title-lg}"
    rounded: "{rounded.lg}"
    padding: 32px
  cream-callout-card:
    backgroundColor: "{colors.signature-cream}"
    textColor: "{colors.ink}"
    typography: "{typography.title-lg}"
    rounded: "{rounded.md}"
    padding: 24px
  demo-grid-card:
    backgroundColor: "{colors.canvas}"
    textColor: "{colors.ink}"
    typography: "{typography.label-md}"
    rounded: "{rounded.md}"
    padding: 16px
  text-input:
    backgroundColor: "{colors.canvas}"
    textColor: "{colors.ink}"
    typography: "{typography.body-md}"
    rounded: "{rounded.sm}"
    padding: 12px 16px
    height: 44px
  footer:
    backgroundColor: "{colors.canvas}"
    textColor: "{colors.body}"
    typography: "{typography.body-md}"
    padding: 64px
---

## Overview

Airtable's marketing surfaces are quietly editorial. The base atmosphere is white canvas, dark ink type, generous whitespace, and a near-black pill CTA—nothing is fighting for attention until a signature card breaks the quiet.

Type voice is Haas Grotesk at modest weights (400 for display, 500 for titles and buttons). Display headlines never go bolder than 500—emphasis comes from size and color contrast, not font weight.

**Key Characteristics:**
- Primary CTA is `{colors.primary}` (near-black) with white text and 12px corner radius.
- Secondary CTA is white with ink text and hairline outline; the two form Airtable's signature button pair.
- Hero is white canvas with no atmospheric gradient, no mesh, no flourish.
- Brand voltage lives in **signature surface cards**: coral, forest, dark navy, and cream.
- Demo-card grids carry product UI fragments on warm pastel surfaces.
- Section rhythm: white → signature card → white → cream → dark → light gray → white.
- Vertical rhythm is `{spacing.section}` (96px) between major bands.

## Colors

### Brand & Accent
- **Primary** (`{colors.primary}` — #181d26): Dominant brand color for CTAs and display type.
- **Primary Active** (`{colors.primary-active}` — #0d1218): Press state on buttons.

### Surface
- **Canvas** (`{colors.canvas}` — #ffffff): Default page surface.
- **Surface Soft** (`{colors.surface-soft}` — #f8fafc): Tabbed feature cards.
- **Surface Strong** (`{colors.surface-strong}` — #e0e2e6): Light gray CTA banner.
- **Surface Dark** (`{colors.surface-dark}` — #181d26): Dark navy mid-page cards.

### Signature Surfaces
These colors carry brand voltage as full-bleed card surfaces:
- **Coral** (`{colors.signature-coral}` — #aa2d00): Dark coral homepage signature card.
- **Forest** (`{colors.signature-forest}` — #0a2e0e): Deep green signature card.
- **Cream** (`{colors.signature-cream}` — #f5e9d4): Soft beige callout band.
- **Peach** (`{colors.signature-peach}` — #fcab79), **Mint** (`{colors.signature-mint}` — #a8d8c4): Demo-grid pastels.

## Typography

### Hierarchy

| Token | Size | Weight | Line Height | Use |
|---|---|---|---|---|
| `{typography.display-xl}` | 48px | 500 | 1.1 | Articles page h2 |
| `{typography.display-lg}` | 40px | 400 | 1.2 | Homepage h1 hero |
| `{typography.display-md}` | 32px | 400 | 1.2 | Platform-page h2 |
| `{typography.title-lg}` | 24px | 400 | 1.35 | Section titles |
| `{typography.button}` | 16px | 500 | 1.4 | CTA labels |
| `{typography.body-md}` | 14px | 400 | 1.25 | Body copy |

### Principles
- **Weight 400 for display sizes**—a 40px h1 is intentionally not bold.
- Visual emphasis via size, color, and signature surface cards—not font weight.

## Layout

### Spacing System
- **Base unit:** 4px.
- **Section padding (vertical):** `{spacing.section}` (96px)—universal rhythm constant.
- **Card padding:** `{spacing.xl}` (32px) for feature cards; `{spacing.xxl}` (48px) for signature cards; `{spacing.lg}` (24px) for callouts.
- **Gutters:** `{spacing.lg}` (24px) between grid cards.

### Grid & Container
- **Max content width:** ~1280px centered.
- **Demo-grid:** 3–4 columns at desktop, 2 at tablet, 1 at mobile.
- **Editorial body:** Single column at large breakpoints.

## Elevation & Depth

**Philosophy: color-block first, shadow second.**
- **Flat:** Body sections, top nav, footer.
- **Soft hairline:** 1px border on inputs and secondary buttons.
- **Card flat:** No shadow; relies on color contrast.

Depth comes from **color alternation between white and signature surfaces**, not decorative effects.

## Components

### Buttons

**`button-primary`** — Signature primary CTA. Background `{colors.primary}` (near-black), white text, 12px radius, 16px × 24px padding.

**`button-secondary`** — White outline button. White fill, dark ink text, 1px hairline.

### Cards

**`hero-band`** — Full-page white hero. No card surface, no border, no shadow—just headline, sub-headline, and buttons in clean whitespace.

**`signature-coral-card`** — Large full-bleed coral card. Background `{colors.signature-coral}`, white text, 12px radius, 48px padding.

**`signature-forest-card`** — Deep green signature card.

**`hero-card-dark`** — Dark navy mid-page CTA card.

**`cream-callout-card`** — Beige callout with product UI fragments.

**`demo-grid-card`** — Multi-card grid with product screenshots on canvas or pastel backgrounds.

## Responsive Behavior

| Name | Width | Key Changes |
|---|---|---|
| Mobile | < 768px | Single-column; top nav hamburger; demo-grid 1-up |
| Tablet | 768–1024px | 2-up demo-grid; pricing table scrollable |
| Desktop | 1024–1440px | 3–4 up demo-grid; full nav; 4-up pricing |

## Do's and Don'ts

### Do
- Keep `{component.button-primary}` near-black.
- Use secondary button as the natural pair with primary button.
- Trust whitespace as atmosphere (no gradient, mesh, or backdrop).
- Use signature cards to break editorial monotony.
- Keep demo-grid heights uneven (feels intentional, not spec-sheet).

### Don't
- Don't use link-blue (#1b61c9) as the primary button.
- Don't add gradient backdrops to hero sections.
- Don't bold display-weight type.
- Don't repeat the same surface color in consecutive bands (rhythm matters).
- Don't add extra shadows or decorative effects.
