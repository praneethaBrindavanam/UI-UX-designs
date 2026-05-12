---
name: Sonic Obsidian
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
  on-surface-variant: '#cfc2d6'
  inverse-surface: '#dae2fd'
  inverse-on-surface: '#283044'
  outline: '#988d9f'
  outline-variant: '#4d4354'
  surface-tint: '#ddb7ff'
  primary: '#ddb7ff'
  on-primary: '#490080'
  primary-container: '#b76dff'
  on-primary-container: '#400071'
  inverse-primary: '#842bd2'
  secondary: '#5de6ff'
  on-secondary: '#00363e'
  secondary-container: '#00cbe6'
  on-secondary-container: '#00515d'
  tertiary: '#ffafd3'
  on-tertiary: '#620040'
  tertiary-container: '#e364a7'
  on-tertiary-container: '#560038'
  error: '#ffb4ab'
  on-error: '#690005'
  error-container: '#93000a'
  on-error-container: '#ffdad6'
  primary-fixed: '#f0dbff'
  primary-fixed-dim: '#ddb7ff'
  on-primary-fixed: '#2c0051'
  on-primary-fixed-variant: '#6900b3'
  secondary-fixed: '#a2eeff'
  secondary-fixed-dim: '#2fd9f4'
  on-secondary-fixed: '#001f25'
  on-secondary-fixed-variant: '#004e5a'
  tertiary-fixed: '#ffd8e7'
  tertiary-fixed-dim: '#ffafd3'
  on-tertiary-fixed: '#3d0026'
  on-tertiary-fixed-variant: '#85145a'
  background: '#0b1326'
  on-background: '#dae2fd'
  surface-variant: '#2d3449'
typography:
  display-lg:
    fontFamily: Sora
    fontSize: 48px
    fontWeight: '800'
    lineHeight: 52px
    letterSpacing: -0.04em
  headline-lg:
    fontFamily: Sora
    fontSize: 32px
    fontWeight: '700'
    lineHeight: 40px
    letterSpacing: -0.02em
  headline-md:
    fontFamily: Sora
    fontSize: 24px
    fontWeight: '700'
    lineHeight: 32px
  track-title:
    fontFamily: Hanken Grotesk
    fontSize: 18px
    fontWeight: '600'
    lineHeight: 24px
  artist-name:
    fontFamily: Hanken Grotesk
    fontSize: 14px
    fontWeight: '400'
    lineHeight: 20px
  body-md:
    fontFamily: Hanken Grotesk
    fontSize: 16px
    fontWeight: '400'
    lineHeight: 24px
  label-caps:
    fontFamily: Space Grotesk
    fontSize: 12px
    fontWeight: '600'
    lineHeight: 16px
    letterSpacing: 0.1em
rounded:
  sm: 0.25rem
  DEFAULT: 0.5rem
  md: 0.75rem
  lg: 1rem
  xl: 1.5rem
  full: 9999px
spacing:
  unit: 4px
  container-padding-mobile: 16px
  container-padding-desktop: 32px
  gutter: 12px
  stack-tight: 4px
  stack-base: 12px
  stack-large: 24px
---

## Brand & Style

This design system is engineered for a high-octane music and entertainment experience. It targets a Gen-Z and Millennial audience that craves immersion, speed, and visual stimulation. The brand personality is "Electric Sophistication"—combining the raw energy of a live concert with the polished aesthetic of high-end hardware.

The visual style is a hybrid of **Glassmorphism** and **High-Contrast Modernism**. It leverages deep obsidian surfaces to let vibrant accents pop, creating a sense of infinite depth. The emotional goal is to make the user feel like they are "inside" the music, using translucency and light-refraction effects to simulate digital high-fidelity equipment.

## Colors

The palette is anchored in a dark-mode-first philosophy. The background uses **Obsidian** (#020617) for absolute depth, while **Charcoal** (#1E293B) provides structural variance for containers. 

**Electric Purple** is the primary driver for action, used for play buttons, active states, and primary brand moments. **Neon Cyan** and **Hot Pink** serve as high-energy accents for secondary interactions like "Live" indicators, trending badges, or genre-specific highlights. Vibrant gradients should transition from Purple to Pink or Cyan to create a sense of movement and "light leak" effects.

## Typography

This design system utilizes a trio of modern sans-serifs to establish a high-energy hierarchy. **Sora** is used for impactful headlines, featuring a wide stance and technical geometric curves. **Hanken Grotesk** handles the heavy lifting for track titles and body copy, providing exceptional legibility at small sizes. **Space Grotesk** is reserved for labels and metadata (like timestamps or bitrates), reinforcing the high-tech, futuristic tone.

Track titles must always be two weight-classes heavier than artist names to ensure immediate scannability in dense lists.

## Layout & Spacing

The layout philosophy is "Dense but Breathable." Content is packed tightly to simulate a sense of abundance and energy, but consistent 12px gutters prevent visual clutter. 

We utilize a **fluid grid** that adapts to safe areas. For mobile, a 2-column or 3-column "card shelf" is standard. On desktop, the system expands to a 12-column grid where the sidebar and "Now Playing" widgets occupy fixed widths (280px and 320px respectively), while the central feed remains fluid. Vertical rhythm should rely on 4px increments to maintain a technical, tight feel.

## Elevation & Depth

Depth is achieved through **Glassmorphism** rather than traditional drop shadows. Surfaces do not "float" with shadows; they "stack" with light.

- **Level 0 (Base):** Obsidian (#020617).
- **Level 1 (Cards):** Charcoal (#1E293B) with a 1px inner border of `glass-stroke`.
- **Level 2 (Overlays/Modals):** A 20px Backdrop Blur with 60% opacity fill and a subtle radial gradient emanating from the top-left corner to simulate a light source.
- **Level 3 (Interactive):** Elements like active play buttons feature a "Neon Glow"—a diffused drop shadow using the primary accent color (#A855F7) at 40% opacity.

## Shapes

The shape language is defined by **Generous Roundedness**. Standard UI components use an 8px (0.5rem) radius to feel modern and accessible. However, high-fidelity Content Cards (Album art, Artist profiles) utilize **rounded-xl (1.5rem)** to create a distinctive, premium feel that frames the media as the "hero" of the interface. 

Interactive elements like play buttons or tags should utilize "Pill" shapes (full rounding) to contrast against the structured grid of cards.

## Components

- **Buttons:** Primary buttons are pill-shaped with an Electric Purple to Hot Pink linear gradient. Text is white and bold. Secondary buttons use a "Ghost" style with a 1px Neon Cyan border and white text.
- **Content Cards:** Feature 24px corner radii. They must include a subtle 1px top-light border to separate them from the obsidian background. Hover states should trigger a 1.05x scale transform and increase the intensity of the backdrop blur.
- **Glass Playbar:** The persistent bottom player should use a high-blur (30px) frosted glass effect with a translucent Obsidian background. All controls are white, with the progress bar rendered in a Cyan-to-Purple gradient.
- **Track Lists:** Dense 56px rows. Artist names are secondary text (70% opacity). Active tracks are highlighted with a Neon Cyan "equalizer" animation icon.
- **Chips/Badges:** Small, pill-shaped, and high-contrast. Use Hot Pink for "LIVE" or "NEW" to ensure they demand immediate attention.
- **Input Fields:** Dark charcoal fill with a 1px border that glows Electric Purple when focused.