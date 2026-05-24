---
name: Lumina Creative
colors:
  surface: '#131316'
  surface-dim: '#131316'
  surface-bright: '#39393c'
  surface-container-lowest: '#0e0e11'
  surface-container-low: '#1b1b1e'
  surface-container: '#1f1f22'
  surface-container-high: '#2a2a2d'
  surface-container-highest: '#353438'
  on-surface: '#e4e1e6'
  on-surface-variant: '#d4c0d7'
  inverse-surface: '#e4e1e6'
  inverse-on-surface: '#303033'
  outline: '#9d8ba0'
  outline-variant: '#514255'
  surface-tint: '#ecb2ff'
  primary: '#ecb2ff'
  on-primary: '#520071'
  primary-container: '#bd00ff'
  on-primary-container: '#ffffff'
  inverse-primary: '#9900cf'
  secondary: '#b9f1ff'
  on-secondary: '#00363f'
  secondary-container: '#00e0ff'
  on-secondary-container: '#005f6d'
  tertiary: '#ffb1c3'
  on-tertiary: '#66002c'
  tertiary-container: '#e7006e'
  on-tertiary-container: '#ffffff'
  error: '#ffb4ab'
  on-error: '#690005'
  error-container: '#93000a'
  on-error-container: '#ffdad6'
  primary-fixed: '#f8d8ff'
  primary-fixed-dim: '#ecb2ff'
  on-primary-fixed: '#320047'
  on-primary-fixed-variant: '#74009f'
  secondary-fixed: '#a5eeff'
  secondary-fixed-dim: '#00daf8'
  on-secondary-fixed: '#001f25'
  on-secondary-fixed-variant: '#004e5a'
  tertiary-fixed: '#ffd9e0'
  tertiary-fixed-dim: '#ffb1c3'
  on-tertiary-fixed: '#3f0019'
  on-tertiary-fixed-variant: '#8f0041'
  background: '#131316'
  on-background: '#e4e1e6'
  surface-variant: '#353438'
typography:
  display-lg:
    fontFamily: Sora
    fontSize: 64px
    fontWeight: '800'
    lineHeight: '1.1'
    letterSpacing: -0.02em
  display-lg-mobile:
    fontFamily: Sora
    fontSize: 40px
    fontWeight: '800'
    lineHeight: '1.1'
    letterSpacing: -0.02em
  headline-md:
    fontFamily: Sora
    fontSize: 32px
    fontWeight: '700'
    lineHeight: '1.2'
  headline-sm:
    fontFamily: Sora
    fontSize: 24px
    fontWeight: '600'
    lineHeight: '1.3'
  body-lg:
    fontFamily: Hanken Grotesk
    fontSize: 18px
    fontWeight: '400'
    lineHeight: '1.6'
  body-md:
    fontFamily: Hanken Grotesk
    fontSize: 16px
    fontWeight: '400'
    lineHeight: '1.6'
  label-bold:
    fontFamily: Space Grotesk
    fontSize: 14px
    fontWeight: '700'
    lineHeight: '1.0'
    letterSpacing: 0.05em
  label-mono:
    fontFamily: Space Grotesk
    fontSize: 12px
    fontWeight: '500'
    lineHeight: '1.0'
rounded:
  sm: 0.5rem
  DEFAULT: 1rem
  md: 1.5rem
  lg: 2rem
  xl: 3rem
  full: 9999px
spacing:
  unit: 4px
  xs: 4px
  sm: 8px
  md: 16px
  lg: 24px
  xl: 40px
  xxl: 80px
  gutter: 24px
  margin-mobile: 16px
  margin-desktop: 64px
---

## Brand & Style

This design system is built for high-energy creative platforms, experimental startups, and immersive digital experiences. The brand personality is expressive, kinetic, and unapologetically bold. It aims to evoke a sense of digital craftsmanship through tactile interactions and luminous visual cues.

The design style merges **Glassmorphism** with **High-Contrast Bold** aesthetics. It utilizes frosted-glass surfaces to provide depth, while vibrant, neon-inflected gradients serve as the primary drivers of action and attention. Every interaction is designed to feel alive, using glow and light to guide the user through the interface.

## Colors

The palette is optimized for a **Dark Mode** environment to allow the vibrant gradients to "pop." 

- **Primary (Electric Purple):** Used for main actions and focus states.
- **Secondary (Cyber Cyan):** Used for informative accents and alternative actions.
- **Tertiary (Hot Pink):** Used for high-energy highlights and playful elements.
- **Neutral:** A deep, obsidian black-grey provides the foundation, ensuring that the glass effects maintain high legibility and contrast.

All interactive elements should leverage the defined gradients rather than flat colors to maintain the "luminous" feel.

## Typography

The typography system uses a tiered approach to balance character with readability.

1. **Headlines (Sora):** A geometric sans-serif with unique quirks that feels futuristic and premium. Use for all major titles.
2. **Body (Hanken Grotesk):** A highly legible, contemporary sans-serif for long-form text and interface labels.
3. **Labels (Space Grotesk):** Utilized for button text and metadata. The slight technical edge of Space Grotesk complements the glassmorphic UI.

Maintain tight tracking on large display headers to increase visual impact.

## Layout & Spacing

The design system employs a **Fluid Grid** with a baseline unit of 4px. Layouts are designed to be expansive, using generous white space (or "dark space") to separate glass containers.

- **Desktop:** 12-column grid, 64px side margins, 24px gutters.
- **Mobile:** 4-column grid, 16px side margins, 16px gutters.

Spacing between interactive elements should be generous (MD or LG) to prevent visual clutter and accommodate the "glow" radius of buttons.

## Elevation & Depth

Depth is created through **Glassmorphism** and **Light Emission** rather than traditional drop shadows.

- **Layer 0 (Background):** Deep neutral `#0F0F12`.
- **Layer 1 (Card/Container):** Background blur (20px) with a semi-transparent white fill (5%) and a 1px inner border (12% white) to catch the "light."
- **Layer 2 (Interactive):** Elements that sit on top of glass containers. These use "Ambient Glows"—shadows that match the color of the element (e.g., a purple button has a soft purple shadow) with a high blur radius (30px) and low opacity (40%).
- **Layer 3 (Modals):** High-intensity blur (40px) with a slightly darker tint to pull focus.

## Shapes

The default shape language is **Pill-shaped (3)** for buttons to emphasize the playful and friendly nature of the system. However, specific components use a hierarchy of shapes:

- **Interactive Primary:** Pill-shaped (9999px) for maximum "squish" and touch-friendliness.
- **Containers/Cards:** Large rounded (1.5rem / 24px) to create a soft, modern frame.
- **Inputs:** Rounded (0.75rem / 12px) to provide a distinct look from buttons.
- **Structural Accents:** Sharp (0px) used sparingly for high-fashion or brutalist-inspired sections.

## Components

### Buttons & Interactivity
Buttons are the core of this system. They should be styled as follows:
- **Primary:** Electric Purple gradient, white text, pill-shaped. On hover, trigger a `glowing` animation.
- **Secondary:** Glass-surface background with a Cyber Cyan border. On hover, the border "pulses."
- **Ghost:** No background, underline on hover with a `sparkling` particle effect.

### Interactive Animations
- **Pulsing:** A rhythmic scale (1.0 to 1.05) and opacity shift (0.8 to 1.0) for "waiting" states.
- **Glowing:** An expansion of the box-shadow (glow) radius from 10px to 30px.
- **Sparkling:** Small, 2px star-shaped particles that spawn and fade around the element's perimeter on click or success states.

### Input Fields
Inputs use the `glass-surface` token with a subtle `glass-border`. When focused, the border transitions to a `cyber-cyan` gradient, and the background blur increases slightly.

### Cards
Glassmorphic containers with a subtle 1px border. Cards should not have shadows unless hovered, at which point an `ambient-glow` matching the content color should appear.

### Chips
Small, pill-shaped elements using the `tertiary` (Hot Pink) gradient for high visibility, or `glass-surface` for passive metadata.