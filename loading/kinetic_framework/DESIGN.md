---
name: Kinetic Framework
colors:
  surface: '#131315'
  surface-dim: '#131315'
  surface-bright: '#39393b'
  surface-container-lowest: '#0e0e10'
  surface-container-low: '#1b1b1d'
  surface-container: '#201f21'
  surface-container-high: '#2a2a2c'
  surface-container-highest: '#353437'
  on-surface: '#e5e1e4'
  on-surface-variant: '#cbc4d2'
  inverse-surface: '#e5e1e4'
  inverse-on-surface: '#303032'
  outline: '#948e9c'
  outline-variant: '#494551'
  surface-tint: '#cfbcff'
  primary: '#cfbcff'
  on-primary: '#381e72'
  primary-container: '#6750a4'
  on-primary-container: '#e0d2ff'
  inverse-primary: '#6750a4'
  secondary: '#cdc0e9'
  on-secondary: '#342b4b'
  secondary-container: '#4d4465'
  on-secondary-container: '#bfb2da'
  tertiary: '#e7c365'
  on-tertiary: '#3e2e00'
  tertiary-container: '#c9a74d'
  on-tertiary-container: '#503d00'
  error: '#ffb4ab'
  on-error: '#690005'
  error-container: '#93000a'
  on-error-container: '#ffdad6'
  primary-fixed: '#e9ddff'
  primary-fixed-dim: '#cfbcff'
  on-primary-fixed: '#22005d'
  on-primary-fixed-variant: '#4f378a'
  secondary-fixed: '#e9ddff'
  secondary-fixed-dim: '#cdc0e9'
  on-secondary-fixed: '#1f1635'
  on-secondary-fixed-variant: '#4b4263'
  tertiary-fixed: '#ffdf93'
  tertiary-fixed-dim: '#e7c365'
  on-tertiary-fixed: '#241a00'
  on-tertiary-fixed-variant: '#594400'
  background: '#131315'
  on-background: '#e5e1e4'
  surface-variant: '#353437'
typography:
  display-xl:
    fontFamily: Space Grotesk
    fontSize: 64px
    fontWeight: '700'
    lineHeight: '1.1'
    letterSpacing: -0.04em
  headline-lg:
    fontFamily: Space Grotesk
    fontSize: 32px
    fontWeight: '600'
    lineHeight: '1.2'
  body-md:
    fontFamily: Geist
    fontSize: 16px
    fontWeight: '400'
    lineHeight: '1.5'
  label-mono:
    fontFamily: JetBrains Mono
    fontSize: 12px
    fontWeight: '500'
    lineHeight: '1.0'
    letterSpacing: 0.1em
rounded:
  sm: 0.125rem
  DEFAULT: 0.25rem
  md: 0.375rem
  lg: 0.5rem
  xl: 0.75rem
  full: 9999px
spacing:
  unit: 8px
  container-padding: 2rem
  stack-gap: 1rem
  progress-height-sm: 4px
  progress-height-md: 12px
  progress-height-lg: 32px
---

## Brand & Style

This design system is a multi-modal framework specifically engineered for high-performance motion and loading states. It transitions seamlessly between three distinct visual personas while maintaining a unified logic for progress visualization and temporal feedback.

- **Minimalist Web Persona:** Focuses on clarity and reduction. It uses heavy whitespace, sharp typographic hierarchy, and precision-engineered progress lines to reduce cognitive load during wait times.
- **Cinematic Persona:** Employs a "theatrical" dark mode aesthetic. It utilizes glassmorphism, deep background blurs, and sunset-hued glows to create a premium, immersive transition between content states.
- **Gaming Persona:** A high-energy, futuristic aesthetic. It leverages high-contrast neon accents, technical geometric shapes, and aggressive motion curves to maintain user engagement during data-heavy loads.

The overarching philosophy is **Active Transparency**: loading is never a "dead" state, but a choreographed transition that communicates the system's velocity.

## Colors

The system operates primarily in a sophisticated **dark mode** to accommodate the Cinematic and Gaming personas, with a high-contrast Light variation for the Minimalist persona. 

- **Deep Indigo (#2E10FF):** Used for the Minimalist persona. It represents intelligence and stability.
- **Sunset Orange (#FF4D00):** The primary driver for the Cinematic persona, often paired with localized glows and "heat" maps in progress bars.
- **Cyber Lime (#CCFF00):** The high-visibility core for the Gaming persona, designed to vibrate against deep blacks.

For loading states, use **60% opacity** of the primary color for track backgrounds and **100% opacity** with an additive glow for active progress indicators.

## Typography

The typography strategy differentiates between the technical nature of "loading" and the brand's voice.

1. **Space Grotesk** is used for large display percentages and status headlines. Its geometric construction feels both technical (Gaming) and architectural (Minimal).
2. **Geist** provides a neutral, highly legible secondary layer for status messages and descriptions.
3. **JetBrains Mono** is reserved for "System Logs" or granular data loading (e.g., "KB/s" or "Asset 45/100").

For the Minimalist persona, keep weights at `400` or `500`. For Gaming and Cinematic, use `700` for display states to anchor the user's eye during motion.

## Layout & Spacing

This system utilizes a **Fluid Grid** with a heavy emphasis on vertical stacking. 

- **The Focus Zone:** All loading indicators are centered horizontally and vertically in the viewport or their respective containers to signify priority.
- **Progress Rhythm:** A base 8px scale governs all elements. Progress bars utilize specific height tokens: `sm` for discreet top-of-page loaders, `md` for standard cards, and `lg` for full-screen cinematic transitions.
- **Adaptive Reflow:** On mobile, progress bars expand to fill the full width of the container minus a 16px safe area, while on desktop, they are capped at a 480px max-width to maintain visual density.

## Elevation & Depth

Hierarchy is established through "Luminosity Tiers" rather than traditional shadows.

- **Minimalist Depth:** Uses flat, high-contrast layers. The loader sits on the highest Z-index with a subtle `1px` stroke to separate it from the background.
- **Cinematic Depth:** Relies on **Glassmorphism**. Surface containers use a `backdrop-filter: blur(20px)` and `20%` white opacity. The loading progress emits a "diffuse glow" (box-shadow: 0 0 30px Sunset Orange) that reflects onto the glass layer.
- **Gaming Depth:** Uses **Tonal Stacking**. The background is absolute black (#000000). Active elements use "Neon Outlines"—2px solid Cyber Lime strokes with a secondary outer glow to simulate a screen-emitted light source.

## Shapes

The shape language is controlled by the **Soft (1)** token (0.25rem radius) to ensure a modern, professional feel across all personas.

- **Minimalist:** Strictly follows the `rounded-sm` (4px) rule for a sharp, precise look.
- **Cinematic:** Overrides to `rounded-xl` for large container glass panels to soften the aesthetic and feel more "organic."
- **Gaming:** Often reverts to `rounded-none` for progress bar caps to emphasize a "digital/pixel" precision, while buttons remain `rounded-sm`.

## Components

### Progress Bars
- **The Flow-Bar:** A continuous, non-stepped bar. In the Gaming persona, it features a "scanning" highlight that moves faster than the actual progress.
- **The Segmented Loader:** 5–10 discrete blocks. Ideal for the Cinematic persona to show chapter loading.
- **The Radial Pulse:** A circular loader used for focal point loading. The stroke should be "tapered," thinning at the tail.

### Skeletons & Shimmers
- **Wave Shimmer:** Use a linear gradient at a 45-degree angle. In the Minimalist persona, use a subtle Grey-to-White transition. In Gaming, use a Cyber Lime-to-Transparent pulse.
- **Ghost Cards:** Low-opacity representations of content. Use a `pulsate` animation (opacity 0.4 to 0.8) rather than a sliding shimmer for the Cinematic persona to keep it "calm."

### Interaction Points
- **Actionable Chips:** While loading, chips should enter a "Processing" state—text changes to "Syncing..." and the leading icon is replaced by a 12px Radial Pulse.
- **Input Fields:** During submission, the bottom border of the input field transforms into a 2px progress bar (the "Border-Loader").