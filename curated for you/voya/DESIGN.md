---
name: Voya
colors:
  surface: '#f8f9fa'
  surface-dim: '#d9dadb'
  surface-bright: '#f8f9fa'
  surface-container-lowest: '#ffffff'
  surface-container-low: '#f3f4f5'
  surface-container: '#edeeef'
  surface-container-high: '#e7e8e9'
  surface-container-highest: '#e1e3e4'
  on-surface: '#191c1d'
  on-surface-variant: '#464652'
  inverse-surface: '#2e3132'
  inverse-on-surface: '#f0f1f2'
  outline: '#777683'
  outline-variant: '#c7c5d4'
  surface-tint: '#4f54b4'
  primary: '#15157d'
  on-primary: '#ffffff'
  primary-container: '#2e3192'
  on-primary-container: '#9da1ff'
  inverse-primary: '#c0c1ff'
  secondary: '#ad3300'
  on-secondary: '#ffffff'
  secondary-container: '#ff642d'
  on-secondary-container: '#5a1600'
  tertiary: '#002e2d'
  on-tertiary: '#ffffff'
  tertiary-container: '#004645'
  on-tertiary-container: '#59b8b5'
  error: '#ba1a1a'
  on-error: '#ffffff'
  error-container: '#ffdad6'
  on-error-container: '#93000a'
  primary-fixed: '#e1e0ff'
  primary-fixed-dim: '#c0c1ff'
  on-primary-fixed: '#04006d'
  on-primary-fixed-variant: '#373a9b'
  secondary-fixed: '#ffdbd0'
  secondary-fixed-dim: '#ffb59e'
  on-secondary-fixed: '#3a0b00'
  on-secondary-fixed-variant: '#842500'
  tertiary-fixed: '#94f2ef'
  tertiary-fixed-dim: '#78d6d2'
  on-tertiary-fixed: '#00201f'
  on-tertiary-fixed-variant: '#00504e'
  background: '#f8f9fa'
  on-background: '#191c1d'
  surface-variant: '#e1e3e4'
typography:
  display-lg:
    fontFamily: Playfair Display
    fontSize: 48px
    fontWeight: '700'
    lineHeight: 56px
    letterSpacing: -0.02em
  display-lg-mobile:
    fontFamily: Playfair Display
    fontSize: 36px
    fontWeight: '700'
    lineHeight: 44px
    letterSpacing: -0.01em
  headline-lg:
    fontFamily: Playfair Display
    fontSize: 32px
    fontWeight: '600'
    lineHeight: 40px
  headline-md:
    fontFamily: Playfair Display
    fontSize: 24px
    fontWeight: '600'
    lineHeight: 32px
  body-lg:
    fontFamily: Inter
    fontSize: 18px
    fontWeight: '400'
    lineHeight: 28px
  body-md:
    fontFamily: Inter
    fontSize: 16px
    fontWeight: '400'
    lineHeight: 24px
  label-md:
    fontFamily: Inter
    fontSize: 14px
    fontWeight: '600'
    lineHeight: 20px
    letterSpacing: 0.05em
  caption:
    fontFamily: Inter
    fontSize: 12px
    fontWeight: '400'
    lineHeight: 16px
rounded:
  sm: 0.25rem
  DEFAULT: 0.5rem
  md: 0.75rem
  lg: 1rem
  xl: 1.5rem
  full: 9999px
spacing:
  base: 8px
  container-margin-mobile: 20px
  container-margin-desktop: 48px
  gutter: 24px
  stack-sm: 12px
  stack-md: 24px
  stack-lg: 48px
---

## Brand & Style

The design system is anchored in the concept of "Editorial Exploration." It balances the raw, visceral energy of world travel with the sophisticated curation of a high-end travel magazine. The brand personality is adventurous yet refined, aimed at discerning travelers who seek meaningful, personalized experiences rather than generic tourism.

The visual style employs **Minimalism with Editorial flourishes**. It relies on expansive white space, high-quality full-bleed photography, and a sophisticated typographic hierarchy to create a sense of calm and inspiration. The UI acts as a silent concierge—unobtrusive, functional, and deeply elegant—allowing the travel imagery to serve as the primary emotional driver.

## Colors

The palette is designed to evoke the transition from deep sea/twilight to the warmth of a setting sun. 

- **Primary (Deep Indigo):** Used for core branding, primary actions, and navigational elements to establish trust and authority.
- **Secondary (Warm Sunset Orange):** Reserved for high-intent calls to action, highlights, and discovery-based features to spark energy.
- **Accent (Sage Green):** Utilized for wellness, nature-focused categories, and success states, providing a calming counterpoint to the primary colors.
- **Background (Soft Off-White):** Replaces pure white to reduce eye strain and provide a more "paper-like" editorial feel.
- **Neutral (Slate Grays):** Used for secondary text and borders to maintain high legibility without the harshness of pure black.

## Typography

This design system uses a high-contrast typographic pairing to reinforce its editorial narrative. 

**Playfair Display** is used for all headlines and display text. Its elegant serifs suggest a curated, premium experience. For mobile devices, display sizes are scaled down to ensure the text remains impactful without breaking layout flow.

**Inter** is the functional workhorse for body copy, UI labels, and inputs. It is chosen for its exceptional legibility at small sizes and its neutral, modern character which doesn't compete with the expressive headlines. 

Use `label-md` for buttons and navigation items, applying the defined letter spacing and uppercase transform to distinguish interactive elements from static content.

## Layout & Spacing

The layout philosophy follows a **Fluid Grid** model with generous margins to maintain a premium feel. 

- **Mobile:** 4-column grid with 20px side margins and 16px gutters.
- **Desktop:** 12-column grid with a max-width of 1440px, centered, with 48px margins and 24px gutters.

The spacing rhythm is based on a factor of 8px. Use `stack-lg` for separating major content sections and `stack-sm` for grouping related elements (like a headline and its sub-caption). Full-bleed imagery should be used frequently for hero sections, breaking the grid margins to create a more immersive, cinematic experience.

## Elevation & Depth

To maintain a minimalist aesthetic while providing visual cues for interactivity, this design system uses **Ambient Shadows** and tonal layering.

- **Level 0 (Surface):** The `Soft Off-White` background.
- **Level 1 (Cards):** Low-contrast surfaces with a subtle shadow (Blur: 12px, Y: 4px, Color: 4% opacity of Primary Color).
- **Level 2 (Modals/Popovers):** Higher contrast shadows (Blur: 24px, Y: 8px, Color: 8% opacity of Primary Color).

Avoid heavy borders; instead, use slight shifts in background color or these soft shadows to define boundaries. Depth should feel like physical layers of high-quality paper stacked lightly on top of one another.

## Shapes

The shape language is defined by **rounded elegance**. High corner radii are used to soften the geometric nature of the digital grid, making the app feel more approachable and friendly.

- **Standard Elements (Buttons, Inputs):** 0.5rem (8px).
- **Cards & Large Containers:** 1.5rem (24px) for a distinctive, modern "curated card" look.
- **Interactive Chips:** Pill-shaped (fully rounded) to differentiate them from functional buttons.

Large full-bleed images that act as headers should remain sharp on the outside edges (0px) but can adopt the 24px radius when presented as floating elements or within a scrollable list.

## Components

### Buttons
- **Primary:** Deep Indigo background with White text. Pill-shaped or 8px rounded corners.
- **Secondary:** Transparent background with a 1px Deep Indigo border or Warm Sunset Orange for high-energy conversion points.
- **State Changes:** On hover/active, apply a 10% black overlay to the background color.

### Cards
- Travel destination cards must use 24px rounded corners (`rounded-xl`).
- Use an aspect ratio of 4:5 for destination previews to maximize visual impact.
- Text overlays on imagery must use a subtle dark-to-transparent gradient (bottom-up) to ensure Playfair Display headings remain legible.

### Input Fields
- Understated style: Only a bottom border (1px Slate) or a very light background fill (#F1F3F5).
- Focus state: Border transitions to Deep Indigo (Primary) with a subtle glow.

### Chips & Tags
- Used for travel categories (e.g., "Beach", "Cultural", "Luxury").
- Pill-shaped with the Sage Green accent at 10% opacity for the background and 100% opacity for the text.

### Navigation
- A minimalist bottom navigation bar on mobile with thin-stroke icons and no text labels for a cleaner look, or a centered top-bar menu on desktop using `label-md` typography.