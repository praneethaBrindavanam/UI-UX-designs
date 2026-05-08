---
name: Modern Utility
colors:
  surface: '#0b1326'
  surface-dim: '#0b1326'
  surface-bright: '#31394d'
  surface-container-lowest: '#060e20'
  surface-container-low: '#131b2e'
  surface-container: '#171f33'
  surface-container-high: '#222a3d'
  surface-container-highest: '#2d3449'
  on-surface: '#dae2fd'
  on-surface-variant: '#c1c6d7'
  inverse-surface: '#dae2fd'
  inverse-on-surface: '#283044'
  outline: '#8b90a0'
  outline-variant: '#414755'
  surface-tint: '#adc6ff'
  primary: '#adc6ff'
  on-primary: '#002e69'
  primary-container: '#4b8eff'
  on-primary-container: '#00285c'
  inverse-primary: '#005bc1'
  secondary: '#c7fff0'
  on-secondary: '#00382f'
  secondary-container: '#00f2d1'
  on-secondary-container: '#006a5a'
  tertiary: '#ffba20'
  on-tertiary: '#412d00'
  tertiary-container: '#bc8700'
  on-tertiary-container: '#392600'
  error: '#ffb4ab'
  on-error: '#690005'
  error-container: '#93000a'
  on-error-container: '#ffdad6'
  primary-fixed: '#d8e2ff'
  primary-fixed-dim: '#adc6ff'
  on-primary-fixed: '#001a41'
  on-primary-fixed-variant: '#004493'
  secondary-fixed: '#26fedc'
  secondary-fixed-dim: '#00dfc1'
  on-secondary-fixed: '#00201a'
  on-secondary-fixed-variant: '#005144'
  tertiary-fixed: '#ffdea8'
  tertiary-fixed-dim: '#ffba20'
  on-tertiary-fixed: '#271900'
  on-tertiary-fixed-variant: '#5e4200'
  background: '#0b1326'
  on-background: '#dae2fd'
  surface-variant: '#2d3449'
typography:
  display-lg:
    fontFamily: Inter
    fontSize: 32px
    fontWeight: '700'
    lineHeight: '1.2'
    letterSpacing: -0.02em
  headline-md:
    fontFamily: Inter
    fontSize: 20px
    fontWeight: '600'
    lineHeight: '1.4'
    letterSpacing: -0.01em
  body-base:
    fontFamily: Inter
    fontSize: 14px
    fontWeight: '400'
    lineHeight: '1.5'
    letterSpacing: 0em
  body-sm:
    fontFamily: Inter
    fontSize: 12px
    fontWeight: '400'
    lineHeight: '1.5'
    letterSpacing: 0em
  data-mono:
    fontFamily: JetBrains Mono
    fontSize: 13px
    fontWeight: '500'
    lineHeight: '1'
    letterSpacing: -0.01em
  label-caps:
    fontFamily: Inter
    fontSize: 11px
    fontWeight: '700'
    lineHeight: '1'
    letterSpacing: 0.05em
rounded:
  sm: 0.125rem
  DEFAULT: 0.25rem
  md: 0.375rem
  lg: 0.5rem
  xl: 0.75rem
  full: 9999px
spacing:
  unit: 4px
  container-padding: 24px
  gutter: 16px
  component-gap-xs: 4px
  component-gap-sm: 8px
  component-gap-md: 12px
  section-margin: 32px
---

## Brand & Style
This design system is engineered for high-density information environments where cognitive load management is paramount. The brand personality is authoritative, precise, and utilitarian, favoring functional efficiency over decorative elements.

The aesthetic follows a "Modern Utility" philosophy: it blends the structured rigor of enterprise software with contemporary visual refinements like subtle glassmorphism and depth-based layering. It is designed for expert users who require rapid data scanning and complex decision-making capabilities. The emotional response should be one of focused control, reliability, and technical sophistication.

## Colors
The palette is rooted in a deep "Midnight Navy" and "Charcoal" foundation to reduce eye strain during prolonged use. 

- **Primary (Electric Blue):** Reserved for primary actions, active states, and critical paths.
- **Secondary (Mint Green):** Used for "Success" indicators, positive trends, and health statuses.
- **Tertiary (Amber):** Dedicated to "Warning" states and cautionary data points.
- **Neutral Stack:** A range of cool greys and navies used to create structural hierarchy without the harshness of pure black.

Data visualization should utilize these core action colors complemented by a supporting scale of teals and indigos to ensure high contrast against the dark backgrounds.

## Typography
This design system employs a dual-font strategy to maximize legibility in dense layouts.

- **Inter** is the workhorse for all interface labels, body copy, and headings, chosen for its exceptional x-height and clarity at small sizes.
- **JetBrains Mono** (or similar technical mono) is utilized exclusively for numerical data, timestamps, and coordinates to ensure tabular alignment and rapid character recognition.

Hierarchy is established through weight and color (using opacity for secondary text) rather than drastic size shifts, maintaining a compact vertical footprint.

## Layout & Spacing
The layout uses a **Fluid Grid** system with a 4px base unit. In a high-density environment, space is a premium resource; therefore, the spacing rhythm is tight but intentional.

Components should be grouped into logical modules using a 12-column grid for dashboard views. Use "Compact" density for data tables and "Roomy" density for top-level navigation. Gutters are kept at a strict 16px to maximize the visible data area while preventing visual bleed between disparate data sets.

## Elevation & Depth
Elevation in this design system is achieved through **Tonal Layering** and **Subtle Glassmorphism** rather than traditional heavy shadows.

- **Base Layer:** The dark background (`#0B0F1A`).
- **Surface Layer:** Dashboard widgets and cards use a slightly lighter fill (`#161D2E`) with a 1px low-opacity border (`white/8%`).
- **Floating Layer:** Modals and tooltips utilize a translucent backdrop-filter (blur: 12px) with a semi-transparent fill (`#1E293B/80%`) to create a "glass" effect that maintains context of the underlying data.
- **Active States:** Subtle inner glows or 2px solid accents on the left edge of a container indicate focus or selection.

## Shapes
Shapes are disciplined and architectural. A "Soft" roundedness (4px radius) is applied to standard components like buttons, input fields, and small cards to take the edge off the technical aesthetic without feeling "bubbly."

Larger containers or sections may use an 8px radius (`rounded-lg`) to clearly define boundaries. Data visualization markers (nodes, chart points) remain sharp or use minimal 2px rounding to ensure precision.

## Components
- **Buttons:** Primary buttons use a solid Electric Blue fill. Secondary buttons are "Ghost" style with a 1px border and high-contrast text.
- **Cards:** Dashboard widgets must have a defined header area with `label-caps` typography and a subtle separator line.
- **Data Tables:** Row stripping is discouraged; use subtle hover highlights and 1px horizontal dividers. Use `data-mono` for all numerical cells.
- **Inputs:** Darker than the surface layer to create an "inset" feel. Focus states must use the primary Electric Blue border.
- **Status Indicators:** Use small, vibrant "Pills" with the Mint, Amber, or Blue palette. Include a 2px "Pulse" animation for critical/live data updates.
- **Scrollbars:** Custom-styled to be thin (4px-6px) and low-contrast to avoid distracting from the primary content.