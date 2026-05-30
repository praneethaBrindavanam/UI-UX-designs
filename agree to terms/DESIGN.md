---
name: Stalwart Professional
colors:
  surface: '#faf9ff'
  surface-dim: '#ccdaff'
  surface-bright: '#faf9ff'
  surface-container-lowest: '#ffffff'
  surface-container-low: '#f1f3ff'
  surface-container: '#e9edff'
  surface-container-high: '#e1e8ff'
  surface-container-highest: '#d8e2ff'
  on-surface: '#051a3e'
  on-surface-variant: '#434654'
  inverse-surface: '#1d3054'
  inverse-on-surface: '#edf0ff'
  outline: '#737685'
  outline-variant: '#c3c6d6'
  surface-tint: '#0c56d0'
  primary: '#003d9b'
  on-primary: '#ffffff'
  primary-container: '#0052cc'
  on-primary-container: '#c4d2ff'
  inverse-primary: '#b2c5ff'
  secondary: '#4f5f7b'
  on-secondary: '#ffffff'
  secondary-container: '#cdddff'
  on-secondary-container: '#51617e'
  tertiary: '#004b59'
  on-tertiary: '#ffffff'
  tertiary-container: '#006477'
  on-tertiary-container: '#76e2ff'
  error: '#ba1a1a'
  on-error: '#ffffff'
  error-container: '#ffdad6'
  on-error-container: '#93000a'
  primary-fixed: '#dae2ff'
  primary-fixed-dim: '#b2c5ff'
  on-primary-fixed: '#001848'
  on-primary-fixed-variant: '#0040a2'
  secondary-fixed: '#d6e3ff'
  secondary-fixed-dim: '#b7c7e8'
  on-secondary-fixed: '#091c35'
  on-secondary-fixed-variant: '#374763'
  tertiary-fixed: '#afecff'
  tertiary-fixed-dim: '#48d7f9'
  on-tertiary-fixed: '#001f27'
  on-tertiary-fixed-variant: '#004e5d'
  background: '#faf9ff'
  on-background: '#051a3e'
  surface-variant: '#d8e2ff'
typography:
  headline-xl:
    fontFamily: Hanken Grotesk
    fontSize: 32px
    fontWeight: '700'
    lineHeight: 40px
    letterSpacing: -0.02em
  headline-lg:
    fontFamily: Hanken Grotesk
    fontSize: 24px
    fontWeight: '600'
    lineHeight: 32px
    letterSpacing: -0.01em
  headline-md:
    fontFamily: Hanken Grotesk
    fontSize: 20px
    fontWeight: '600'
    lineHeight: 28px
  body-lg:
    fontFamily: Atkinson Hyperlegible Next
    fontSize: 18px
    fontWeight: '400'
    lineHeight: 28px
  body-md:
    fontFamily: Atkinson Hyperlegible Next
    fontSize: 16px
    fontWeight: '400'
    lineHeight: 24px
  body-sm:
    fontFamily: Atkinson Hyperlegible Next
    fontSize: 14px
    fontWeight: '400'
    lineHeight: 20px
  label-md:
    fontFamily: Hanken Grotesk
    fontSize: 14px
    fontWeight: '600'
    lineHeight: 16px
    letterSpacing: 0.02em
  label-sm:
    fontFamily: Hanken Grotesk
    fontSize: 12px
    fontWeight: '500'
    lineHeight: 14px
    letterSpacing: 0.04em
  legal-disclaimer:
    fontFamily: Atkinson Hyperlegible Next
    fontSize: 12px
    fontWeight: '400'
    lineHeight: 18px
rounded:
  sm: 0.125rem
  DEFAULT: 0.25rem
  md: 0.375rem
  lg: 0.5rem
  xl: 0.75rem
  full: 9999px
spacing:
  unit: 4px
  xs: 4px
  sm: 8px
  md: 16px
  lg: 24px
  xl: 32px
  margin-mobile: 16px
  margin-desktop: 48px
  gutter: 16px
---

## Brand & Style
This design system is engineered for high-stakes environments where clarity, reliability, and institutional trust are paramount. The brand personality is authoritative yet accessible, stripping away decorative excess in favor of a **Corporate Modern** aesthetic. 

The target audience includes professionals in legal, financial, or administrative sectors who require rapid information retrieval and absolute certainty during interaction. The UI evokes a sense of calm efficiency through balanced proportions, generous whitespace, and a systematic approach to density.

## Colors
The palette is anchored by a deep, accessible "Trust Blue" (Primary) which meets WCAG AAA contrast ratios against white backgrounds. 

- **Primary:** Used for main actions, active states, and brand-critical signifiers.
- **Secondary:** A slate gray used for secondary actions and iconography, providing a sophisticated bridge between the primary blue and the neutrals.
- **Tertiary:** A bright teal used sparingly for informational accents or "success" indicators.
- **Neutral:** A range of grays from near-black text to soft "Surface" tints, ensuring the hierarchy is established through tonal variance rather than just color.

## Typography
Typography is the backbone of this design system. We utilize **Hanken Grotesk** for headlines and labels to provide a sharp, modern, and professional edge. For all body copy and legal text, we use **Atkinson Hyperlegible Next**, specifically chosen for its superior readability and distinction between similar character shapes (I, l, 1), which is critical for legal and financial data.

- **Scale:** Large headlines scale down by 20% on mobile devices to prevent excessive wrapping.
- **Legal Text:** Always presented with a minimum of 1.5 line-height to ensure accessibility even at small sizes.

## Layout & Spacing
The system follows a strict **8px grid** (with 4px increments for micro-adjustments). 

- **Mobile:** A 4-column fluid grid with 16px side margins. 
- **Desktop:** A 12-column fixed grid centered in the viewport, max-width 1200px.
- **Rhythm:** Vertical rhythm is maintained by using the `lg` (24px) spacing unit between major sections and `md` (16px) between related elements within a card or list item.

## Elevation & Depth
Depth is conveyed through **Tonal Layers** and extremely subtle **Ambient Shadows**. This prevents the UI from feeling cluttered or overly "gadgety."

- **Level 0 (Base):** Solid white or very light gray (#F4F5F7).
- **Level 1 (Cards/Surfaces):** White background with a 1px border (#DFE1E6). No shadow.
- **Level 2 (Active/Floating):** White background with a soft, 12% opacity neutral shadow, 8px blur, 4px Y-offset.
- **Interactions:** Hover or press states are indicated by a 10% darken overlay rather than a change in elevation.

## Shapes
The shape language is **Soft (0.25rem)**. This provides a subtle modern touch that softens the "institutional" feel without appearing playful or casual. 

- **Standard Buttons/Inputs:** 4px radius.
- **Cards/Modals:** 8px (rounded-lg) to provide a clear container hierarchy.
- **Selection Indicators:** Checkboxes maintain a 2px radius to feel crisp but not sharp.

## Components
- **Buttons:** Primary buttons use a solid Primary Blue background with white text. Secondary buttons use a transparent background with a 1px border in Secondary Gray.
- **Checkboxes:** When selected, checkboxes must fill with Primary Blue and display a white checkmark. The hit area is expanded to 44px minimum for mobile accessibility.
- **Input Fields:** Use a 1px border (#DFE1E6). On focus, the border thickens to 2px in Primary Blue with a subtle 2px outer glow.
- **Lists:** High-density lists for legal data use 1px horizontal dividers. List items feature a 16px padding on all sides to ensure touch-target compliance.
- **Data Tables:** Use alternating row stripes (Zebra striping) in 50% opacity of the lightest neutral to enhance readability in dense legal documents.
- **Chips:** Used for filtering or status. These utilize the tertiary teal for positive statuses and secondary gray for neutral/inactive filters.