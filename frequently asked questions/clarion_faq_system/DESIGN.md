---
name: Clarion FAQ System
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
  on-surface-variant: '#464555'
  inverse-surface: '#2e3132'
  inverse-on-surface: '#f0f1f2'
  outline: '#777587'
  outline-variant: '#c7c4d8'
  surface-tint: '#4d44e3'
  primary: '#3525cd'
  on-primary: '#ffffff'
  primary-container: '#4f46e5'
  on-primary-container: '#dad7ff'
  inverse-primary: '#c3c0ff'
  secondary: '#712ae2'
  on-secondary: '#ffffff'
  secondary-container: '#8a4cfc'
  on-secondary-container: '#fffbff'
  tertiary: '#7e3000'
  on-tertiary: '#ffffff'
  tertiary-container: '#a44100'
  on-tertiary-container: '#ffd2be'
  error: '#ba1a1a'
  on-error: '#ffffff'
  error-container: '#ffdad6'
  on-error-container: '#93000a'
  primary-fixed: '#e2dfff'
  primary-fixed-dim: '#c3c0ff'
  on-primary-fixed: '#0f0069'
  on-primary-fixed-variant: '#3323cc'
  secondary-fixed: '#eaddff'
  secondary-fixed-dim: '#d2bbff'
  on-secondary-fixed: '#25005a'
  on-secondary-fixed-variant: '#5a00c6'
  tertiary-fixed: '#ffdbcc'
  tertiary-fixed-dim: '#ffb695'
  on-tertiary-fixed: '#351000'
  on-tertiary-fixed-variant: '#7b2f00'
  background: '#f8f9fa'
  on-background: '#191c1d'
  surface-variant: '#e1e3e4'
typography:
  headline-xl:
    fontFamily: Inter
    fontSize: 48px
    fontWeight: '700'
    lineHeight: 56px
    letterSpacing: -0.02em
  headline-xl-mobile:
    fontFamily: Inter
    fontSize: 32px
    fontWeight: '700'
    lineHeight: 40px
    letterSpacing: -0.02em
  headline-lg:
    fontFamily: Inter
    fontSize: 30px
    fontWeight: '600'
    lineHeight: 38px
    letterSpacing: -0.01em
  headline-md:
    fontFamily: Inter
    fontSize: 24px
    fontWeight: '600'
    lineHeight: 32px
    letterSpacing: -0.01em
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
    fontWeight: '500'
    lineHeight: 20px
    letterSpacing: 0.05em
rounded:
  sm: 0.25rem
  DEFAULT: 0.5rem
  md: 0.75rem
  lg: 1rem
  xl: 1.5rem
  full: 9999px
spacing:
  base: 8px
  margin-mobile: 1.25rem
  margin-desktop: 2.5rem
  gutter: 1.5rem
  max-width: 1200px
---

## Brand & Style

This design system is engineered for maximum legibility and reduced cognitive load, essential for users seeking information or troubleshooting. The brand personality is **helpful, organized, and trustworthy**. 

The design style follows a **Modern Corporate** approach with a focus on **Functional Minimalism**. It prioritizes high-quality typography and strategic use of whitespace to guide the user's eye toward answers. By stripping away unnecessary ornamentation, the interface feels reliable and efficient, ensuring that the utility of the content remains the primary focus.

## Colors

The palette is anchored by **Deep Indigo (#4F46E5)**, chosen for its association with professional reliability and its excellent contrast ratios for accessibility. 

- **Primary:** Deep Indigo is used for interactive elements, call-to-actions, and active states.
- **Secondary:** A soft Violet (#7C3AED) is used sparingly for accents or specific category differentiation.
- **Neutral:** A range of soft grays (from #F9FAFB for backgrounds to #111827 for primary text) creates a hierarchy that recedes to let the content shine.
- **Surface:** Pure white (#FFFFFF) is used for cards and content containers to provide a clean, high-contrast canvas.

## Typography

The design system utilizes **Inter** across all levels due to its exceptional legibility in digital interfaces and its neutral, systematic character.

A strict hierarchy is maintained:
- **Headlines:** Use Bold or Semi-Bold weights with slight negative letter-spacing to create a compact, authoritative feel.
- **Body:** Generous line-heights (1.5x - 1.6x) are applied to ensure long-form articles remain readable without causing eye fatigue.
- **Labels:** Medium weights with increased letter-spacing and uppercase styling are used for metadata and category tags to distinguish them from actionable text.

## Layout & Spacing

The layout utilizes a **Fixed Grid** model for desktop to ensure line lengths for help articles stay within the optimal 60-80 character range. 

- **Desktop (1024px+):** A 12-column grid with a maximum container width of 1200px.
- **Tablet (768px - 1023px):** An 8-column grid with 24px margins.
- **Mobile (Up to 767px):** A 4-column fluid grid with 20px margins.

Vertical rhythm is based on an **8px baseline**, with consistent padding (32px or 48px) between major sections to emphasize clarity and separation of topics.

## Elevation & Depth

This design system uses **Tonal Layers** supplemented by **Ambient Shadows** to create a sense of order without overwhelming the user with heavy gradients.

1. **Level 0 (Background):** Solid soft gray (#F9FAFB).
2. **Level 1 (Cards/Search):** Pure white background with a subtle, highly diffused shadow (0px 4px 20px rgba(0, 0, 0, 0.05)).
3. **Level 2 (Active Accordions/Modals):** A slightly more pronounced shadow (0px 10px 30px rgba(0, 0, 0, 0.08)) to indicate focus.

Low-contrast 1px borders (#E5E7EB) are used on inactive elements to define structure without adding visual noise.

## Shapes

A **Rounded** shape language is employed to make the help center feel approachable and modern. 

- **Standard Elements:** 8px (0.5rem) radius for buttons, inputs, and small cards.
- **Large Elements:** 16px (1rem) radius for primary category cards and the search bar container.
- **Pill Shapes:** Used exclusively for tags and status indicators to differentiate them from functional UI buttons.

## Components

### Search Bar
The central feature of the help center. It should be oversized with a 16px border radius, a subtle ambient shadow, and a 20px search icon. Use placeholder text that is conversational (e.g., "How can we help you today?").

### Accordions (FAQ Style)
Accordions use a Level 1 elevation (white background). The header should use a Semi-Bold Inter font. When expanded, the header remains static while the content fades in. A subtle horizontal divider separates the header from the content.

### Category Cards
Grid-based cards that house help topics. They feature a centered 32px icon in the Primary color, a Headline-MD title, and a short Body-MD description. On hover, the card should lift slightly using Level 2 elevation.

### Buttons
- **Primary:** Solid Deep Indigo with white text.
- **Secondary:** White background with a 1px border (#D1D5DB) and Indigo text.
- Focused states must include a 2px offset ring in Primary color for accessibility.

### Input Fields
Inputs use a white background with a 1px #D1D5DB border. On focus, the border transitions to Deep Indigo with a soft 3px outer glow in a semi-transparent Indigo.