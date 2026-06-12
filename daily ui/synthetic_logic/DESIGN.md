---
name: Synthetic Logic
colors:
  surface: '#131313'
  surface-dim: '#131313'
  surface-bright: '#3a3939'
  surface-container-lowest: '#0e0e0e'
  surface-container-low: '#1c1b1b'
  surface-container: '#201f1f'
  surface-container-high: '#2a2a2a'
  surface-container-highest: '#353534'
  on-surface: '#e5e2e1'
  on-surface-variant: '#c2c6d6'
  inverse-surface: '#e5e2e1'
  inverse-on-surface: '#313030'
  outline: '#8c909f'
  outline-variant: '#424754'
  surface-tint: '#adc6ff'
  primary: '#adc6ff'
  on-primary: '#002e6a'
  primary-container: '#4d8eff'
  on-primary-container: '#00285d'
  inverse-primary: '#005ac2'
  secondary: '#4edea3'
  on-secondary: '#003824'
  secondary-container: '#00a572'
  on-secondary-container: '#00311f'
  tertiary: '#ffb95f'
  on-tertiary: '#472a00'
  tertiary-container: '#ca8100'
  on-tertiary-container: '#3e2400'
  error: '#ffb4ab'
  on-error: '#690005'
  error-container: '#93000a'
  on-error-container: '#ffdad6'
  primary-fixed: '#d8e2ff'
  primary-fixed-dim: '#adc6ff'
  on-primary-fixed: '#001a42'
  on-primary-fixed-variant: '#004395'
  secondary-fixed: '#6ffbbe'
  secondary-fixed-dim: '#4edea3'
  on-secondary-fixed: '#002113'
  on-secondary-fixed-variant: '#005236'
  tertiary-fixed: '#ffddb8'
  tertiary-fixed-dim: '#ffb95f'
  on-tertiary-fixed: '#2a1700'
  on-tertiary-fixed-variant: '#653e00'
  background: '#131313'
  on-background: '#e5e2e1'
  surface-variant: '#353534'
typography:
  display-lg:
    fontFamily: Hanken Grotesk
    fontSize: 48px
    fontWeight: '700'
    lineHeight: 56px
    letterSpacing: -0.02em
  headline-md:
    fontFamily: Hanken Grotesk
    fontSize: 24px
    fontWeight: '600'
    lineHeight: 32px
    letterSpacing: -0.01em
  body-base:
    fontFamily: Hanken Grotesk
    fontSize: 16px
    fontWeight: '400'
    lineHeight: 24px
  data-mono:
    fontFamily: Geist
    fontSize: 14px
    fontWeight: '500'
    lineHeight: 20px
    letterSpacing: 0.02em
  label-sm:
    fontFamily: Geist
    fontSize: 12px
    fontWeight: '600'
    lineHeight: 16px
  headline-lg-mobile:
    fontFamily: Hanken Grotesk
    fontSize: 32px
    fontWeight: '700'
    lineHeight: 40px
rounded:
  sm: 0.125rem
  DEFAULT: 0.25rem
  md: 0.375rem
  lg: 0.5rem
  xl: 0.75rem
  full: 9999px
spacing:
  unit: 4px
  gutter: 16px
  margin-mobile: 16px
  margin-desktop: 32px
  container-max: 1440px
---

## Brand & Style

This design system embodies a "Design Lab" aesthetic tailored for 2026—a period defined by hyper-functional clarity and technical precision. The brand personality is professional, adaptive, and performance-oriented, targeting power users who require high information density without cognitive fatigue.

The style is a synthesis of **Minimalism** and **Glassmorphism**, executed with surgical accuracy. It utilizes an "Obsidian" dark mode to minimize eye strain and maximize the vibrance of data visualizations. Every UI element is designed to feel like a calibrated instrument, using precise 1px borders and subtle translucency to suggest depth and layering within a high-performance workspace.

## Colors

The palette is anchored by **Logic Blue** (#3B82F6), a high-vibrancy primary used exclusively for interactive states and primary actions. The background is a deep **Obsidian** (#0A0A0A), providing the highest possible contrast for data and text.

- **Primary:** Logic Blue (#3B82F6) for focus and intent.
- **Success/Status:** Emerald (#10B981) for positive technical indicators.
- **Warning/Alert:** Amber (#F59E0B) for system notifications.
- **Neutrals:** A scale of cool grays starting from #0A0A0A (Base) to #262626 (Borders) and #A3A3A3 (Secondary Text).

Status indicators must maintain high contrast ratios against the dark background to ensure instant legibility in data-heavy environments.

## Typography

This design system utilizes a dual-font strategy to balance legibility with technical character. 

1. **Hanken Grotesk** is used for the primary UI, headlines, and body copy. It provides a clean, contemporary feel that remains legible even at high densities.
2. **Geist** is reserved for labels, data points, and numerical values. Its monospace-adjacent qualities ensure that tables and technical readouts align perfectly, reinforcing the "Design Lab" aesthetic.

All headlines should utilize a slight negative letter spacing to feel tighter and more controlled, while data labels use increased tracking for maximum clarity at small sizes.

## Layout & Spacing

The layout follows a strict **Fluid Grid** model based on a 4px baseline shift. 

- **Desktop:** 12-column grid with 16px gutters.
- **Tablet:** 8-column grid with 16px gutters.
- **Mobile:** 4-column grid with 12px gutters.

The philosophy is "Information First." Spacing between related technical components should be tight (8px-12px), while logical sections are separated by larger gaps (32px-48px) to create a visual hierarchy without relying on heavy decorative elements. Content should reflow smoothly, prioritizing data visibility on smaller viewports.

## Elevation & Depth

Depth is communicated through **Glassmorphism** and **Tonal Layers** rather than traditional shadows. 

- **Level 0 (Base):** Obsidian (#0A0A0A).
- **Level 1 (Cards/Panels):** Surface (#171717) with a 1px solid border (#262626).
- **Level 2 (Modals/Overlays):** Semi-transparent background (rgba(23, 23, 23, 0.8)) with a 20px backdrop blur and a vibrant Logic Blue top-edge highlight (0.5px).

Shadows are used sparingly and should be "Ambient"—low opacity, no blur offset, appearing more like a soft glow behind active elements to suggest they are hovering above the interface.

## Shapes

The shape language is "Soft-Technical." Elements use a consistent **0.25rem (4px)** corner radius. This provides a subtle nod to hardware design while maintaining the sharp, efficient look of a high-performance dashboard. 

- **Buttons/Inputs:** 4px radius.
- **Large Panels:** 8px (rounded-lg) to distinguish primary layout containers from nested components.
- **Interactive States:** On hover, borders should transition from neutral gray to Logic Blue, maintaining the 1px stroke weight.

## Components

### Buttons
Primary buttons use a solid Logic Blue fill with white text. Secondary buttons use a "Ghost" style: 1px border (#262626) with no fill, transitioning to a subtle white-tinted background on hover.

### Chips & Tags
Technical tags use Geist (data-mono) and a semi-transparent Logic Blue background (10% opacity) with a solid 1px border.

### Input Fields
Fields feature a dark background (#111), a 1px border, and a focus state that adds a 1px Logic Blue outer glow. Labels always use the `label-sm` Geist typography.

### Cards
Cards are the primary container. They must have a 1px border and 16px-24px internal padding. In "Design Lab" mode, cards may feature a faint grid pattern background at 2% opacity to emphasize the technical theme.

### Status Indicators
Small, high-contrast circular "pills" used to show system health. They should pulsate slightly when in an "Active" or "Critical" state to draw attention within the static UI.