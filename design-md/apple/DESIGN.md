---
version: alpha
name: Apple-design-analysis
description: A photography-first interface that turns marketing into a museum gallery. Edge-to-edge product tiles alternate light and dark canvases, framed by SF Pro Display headlines with negative letter-spacing. Single blue accent. Minimal shadows (one product shadow only). Whisper-soft elevation via color and backdrop blur.

colors:
  primary: "#0066cc"
  primary-focus: "#0071e3"
  primary-on-dark: "#2997ff"
  ink: "#1d1d1f"
  body: "#1d1d1f"
  body-on-dark: "#ffffff"
  body-muted: "#cccccc"
  ink-muted-80: "#333333"
  ink-muted-48: "#7a7a7a"
  divider-soft: "#f0f0f0"
  hairline: "#e0e0e0"
  canvas: "#ffffff"
  canvas-parchment: "#f5f5f7"
  surface-pearl: "#fafafc"
  surface-tile-1: "#272729"
  surface-tile-2: "#2a2a2c"
  surface-tile-3: "#252527"
  surface-black: "#000000"
  surface-chip-translucent: "#d2d2d7"
  on-primary: "#ffffff"
  on-dark: "#ffffff"

typography:
  hero-display:
    fontFamily: "SF Pro Display, system-ui, -apple-system, sans-serif"
    fontSize: 56px
    fontWeight: 600
    lineHeight: 1.07
    letterSpacing: -0.28px
  display-lg:
    fontFamily: "SF Pro Display, system-ui, -apple-system, sans-serif"
    fontSize: 40px
    fontWeight: 600
    lineHeight: 1.1
    letterSpacing: 0
  display-md:
    fontFamily: "SF Pro Text, system-ui, -apple-system, sans-serif"
    fontSize: 34px
    fontWeight: 600
    lineHeight: 1.47
    letterSpacing: -0.374px
  lead:
    fontFamily: "SF Pro Display, system-ui, -apple-system, sans-serif"
    fontSize: 28px
    fontWeight: 400
    lineHeight: 1.14
    letterSpacing: 0.196px
  tagline:
    fontFamily: "SF Pro Display, system-ui, -apple-system, sans-serif"
    fontSize: 21px
    fontWeight: 600
    lineHeight: 1.19
    letterSpacing: 0.231px
  body-strong:
    fontFamily: "SF Pro Text, system-ui, -apple-system, sans-serif"
    fontSize: 17px
    fontWeight: 600
    lineHeight: 1.24
    letterSpacing: -0.374px
  body:
    fontFamily: "SF Pro Text, system-ui, -apple-system, sans-serif"
    fontSize: 17px
    fontWeight: 400
    lineHeight: 1.47
    letterSpacing: -0.374px
  caption:
    fontFamily: "SF Pro Text, system-ui, -apple-system, sans-serif"
    fontSize: 14px
    fontWeight: 400
    lineHeight: 1.43
    letterSpacing: -0.224px
  button-large:
    fontFamily: "SF Pro Text, system-ui, -apple-system, sans-serif"
    fontSize: 18px
    fontWeight: 300
    lineHeight: 1.0
    letterSpacing: 0
  button-utility:
    fontFamily: "SF Pro Text, system-ui, -apple-system, sans-serif"
    fontSize: 14px
    fontWeight: 400
    lineHeight: 1.29
    letterSpacing: -0.224px
  fine-print:
    fontFamily: "SF Pro Text, system-ui, -apple-system, sans-serif"
    fontSize: 12px
    fontWeight: 400
    lineHeight: 1.0
    letterSpacing: -0.12px

rounded:
  none: 0px
  xs: 5px
  sm: 8px
  md: 11px
  lg: 18px
  pill: 9999px
  full: 9999px

spacing:
  xxs: 4px
  xs: 8px
  sm: 12px
  md: 17px
  lg: 24px
  xl: 32px
  xxl: 48px
  section: 80px

components:
  button-primary:
    backgroundColor: "{colors.primary}"
    textColor: "{colors.on-primary}"
    typography: "{typography.body}"
    rounded: "{rounded.pill}"
    padding: 11px 22px
  button-primary-active:
    backgroundColor: "{colors.primary}"
    textColor: "{colors.on-primary}"
    rounded: "{rounded.pill}"
  button-secondary-pill:
    backgroundColor: "{colors.canvas}"
    textColor: "{colors.primary}"
    typography: "{typography.body}"
    rounded: "{rounded.pill}"
    padding: 11px 22px
  button-dark-utility:
    backgroundColor: "{colors.ink}"
    textColor: "{colors.on-dark}"
    typography: "{typography.button-utility}"
    rounded: "{rounded.sm}"
    padding: 8px 15px
  button-icon-circular:
    backgroundColor: "{colors.surface-chip-translucent}"
    textColor: "{colors.ink}"
    rounded: "{rounded.full}"
    size: 44px
  text-link:
    backgroundColor: transparent
    textColor: "{colors.primary}"
    typography: "{typography.body}"
  text-link-on-dark:
    backgroundColor: transparent
    textColor: "{colors.primary-on-dark}"
    typography: "{typography.body}"
  global-nav:
    backgroundColor: "{colors.surface-black}"
    textColor: "{colors.on-dark}"
    typography: "{typography.fine-print}"
    height: 44px
  product-tile-light:
    backgroundColor: "{colors.canvas}"
    textColor: "{colors.ink}"
    typography: "{typography.display-lg}"
    rounded: "{rounded.none}"
    padding: 80px
  product-tile-parchment:
    backgroundColor: "{colors.canvas-parchment}"
    textColor: "{colors.ink}"
    typography: "{typography.display-lg}"
    rounded: "{rounded.none}"
    padding: 80px
  product-tile-dark:
    backgroundColor: "{colors.surface-tile-1}"
    textColor: "{colors.on-dark}"
    typography: "{typography.display-lg}"
    rounded: "{rounded.none}"
    padding: 80px
  store-utility-card:
    backgroundColor: "{colors.canvas}"
    textColor: "{colors.ink}"
    typography: "{typography.body-strong}"
    rounded: "{rounded.lg}"
    padding: 24px
  search-input:
    backgroundColor: "{colors.canvas}"
    textColor: "{colors.ink}"
    typography: "{typography.body}"
    rounded: "{rounded.pill}"
    padding: 12px 20px
    height: 44px
  footer:
    backgroundColor: "{colors.canvas-parchment}"
    textColor: "{colors.ink-muted-80}"
    typography: "{typography.fine-print}"
    padding: 64px
---

## Overview

Apple's web presence is a masterclass in **reverent product photography framed by near-invisible UI**. Every page is a stack of edge-to-edge product tiles alternating light and dark canvases.

Density is unusually low. Each tile occupies roughly one viewport. There is no decorative chrome—no borders, no gradients, no decorative frames, no shadows.

**Key Characteristics:**
- Photography-first presentation; UI recedes so the product can speak.
- Alternating full-bleed tiles: white/parchment ↔ near-black, with color change as the section divider.
- Single blue accent (`{colors.primary}` — #0066cc) for all interactive elements.
- Two button grammars: tiny blue pill CTAs and compact utility rectangles.
- SF Pro Display + SF Pro Text with negative letter-spacing for the signature "Apple tight" feel.
- Whisper-soft elevation via color and backdrop blur (NOT shadows).
- Exactly one product shadow for imagery only.
- Section rhythm: light hero → dark tile → light utility → dark → parchment footer.

## Colors

### Brand & Accent
- **Action Blue** (`{colors.primary}` — #0066cc): The single brand-level interactive color for all CTAs and links.
- **Focus Blue** (`{colors.primary-focus}` — #0071e3): Keyboard focus ring on buttons.
- **Sky Link Blue** (`{colors.primary-on-dark}` — #2997ff): Brighter blue for links on dark surfaces.

### Surface
- **Pure White** (`{colors.canvas}` — #ffffff): Dominant canvas.
- **Parchment** (`{colors.canvas-parchment}` — #f5f5f7): Signature Apple off-white for alternating tiles.
- **Near-Black Tile 1** (`{colors.surface-tile-1}` — #272729): Primary dark-tile surface.
- **Pure Black** (`{colors.surface-black}` — #000000): Global nav background only.

### Text
- **Near-Black Ink** (`{colors.ink}` — #1d1d1f): Dominant text on light surfaces.
- **Body On Dark** (`{colors.body-on-dark}` — #ffffff): All text on dark tiles.

## Typography

### Hierarchy

| Token | Size | Weight | Line Height | Letter Spacing | Use |
|---|---|---|---|---|---|
| `{typography.hero-display}` | 56px | 600 | 1.07 | -0.28px | Hero headline ("Apple tight" tracking) |
| `{typography.display-lg}` | 40px | 600 | 1.1 | 0 | Tile headlines |
| `{typography.body}` | 17px | 400 | 1.47 | -0.374px | Default paragraph |

### Principles
- **Negative letter-spacing at display sizes** (−0.12 → −0.374px) for the "Apple tight" cadence.
- **Body copy at 17px, not 16px**—extra pixel defines the brand's reading pace.
- **Weight 600, not 700**, for headlines; weight 300 is rare and deliberate.
- **Weight 500 is deliberately absent**—ladder is 300/400/600/700.
- **Line-height is context-specific**: display 1.07–1.19 (tight), body 1.47 (relaxed).

## Layout

### Spacing System
- **Base unit:** 8px. Structural layout snaps to 8/12/16/24.
- **Section vertical padding:** `{spacing.section}` (80px) inside tiles; tiles stack edge-to-edge with 0 gap.
- **Card padding:** `{spacing.lg}` (24px) inside utility cards.

### Grid & Container
- **Max content width:** ~980px (text), ~1440px (product grids), full-bleed (tiles).
- **Utility grids:** 3–5 columns at desktop, 2 at tablet, 1 at mobile.

## Elevation & Depth

Apple uses **exactly one** drop-shadow, applied only to product imagery:
- `box-shadow: rgba(0, 0, 0, 0.22) 3px 5px 30px 0`

Elevation in the UI comes from **color alternation and backdrop blur**:
- Flat surfaces (95%): tiles, nav, footer.
- Backdrop blur: sub-nav and sticky bars at 80% opacity.
- **No soft-glow or decorative effects**.

## Components

### Buttons

**`button-primary`** — Signature Apple action. Background `{colors.primary}` (Action Blue), text white, rounded `{rounded.pill}`. Active state: `transform: scale(0.95)`.

**`button-secondary-pill`** — Secondary CTA when two pills appear together ("Learn more" / "Buy").

**`button-dark-utility`** — Global nav actions (Sign In, Bag). Background `{colors.ink}`.

### Cards

**`product-tile-light`** — Full-bleed light tile. Background `{colors.canvas}`, no rounding (0px), vertical padding 80px.

**`product-tile-parchment`** — Same as light but on parchment to break consecutive whites.

**`product-tile-dark`** — Full-bleed dark tile. Background `{colors.surface-tile-1}`, text white.

**`store-utility-card`** — Store grid card. Background `{colors.canvas}`, rounded `{rounded.lg}` (18px), 1px hairline border.

## Responsive Behavior

| Name | Width | Key Changes |
|---|---|---|
| Phone | 420–640px | Single-column; hero h1 drops to 34px |
| Tablet | 736–833px | Global nav collapses; 2-column utility grids |
| Desktop | 1069–1440px | Full layout; 4–5 column grids; 1440px max |

## Do's and Don'ts

### Do
- Use `{colors.primary}` (Action Blue) for every interactive element.
- Set headlines with negative letter-spacing (`−0.28 → −0.374px`) for "Apple tight" feel.
- Run body copy at 17px / 400 / 1.47.
- Alternate light/dark tiles for full-bleed rhythm.
- Apply the single product shadow only to imagery resting on surfaces.
- Use `transform: scale(0.95)` as the active state on buttons.

### Don't
- Don't introduce a second accent color.
- Don't add shadows to cards, buttons, or text.
- Don't use gradients as decorative backgrounds.
- Don't round full-bleed tiles (they're rectangular and edge-to-edge).
- Don't tighten line-height below 1.47 for body copy.
