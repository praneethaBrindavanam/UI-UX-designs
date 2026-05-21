---
name: Celestial Voyager
colors:
  surface: '#101415'
  surface-dim: '#101415'
  surface-bright: '#363a3b'
  surface-container-lowest: '#0b0f10'
  surface-container-low: '#191c1e'
  surface-container: '#1d2022'
  surface-container-high: '#272a2c'
  surface-container-highest: '#323537'
  on-surface: '#e0e3e5'
  on-surface-variant: '#ccc3d7'
  inverse-surface: '#e0e3e5'
  inverse-on-surface: '#2d3133'
  outline: '#958da1'
  outline-variant: '#4a4455'
  surface-tint: '#d3bbff'
  primary: '#d3bbff'
  on-primary: '#3f008d'
  primary-container: '#6d28d9'
  on-primary-container: '#dac5ff'
  inverse-primary: '#7331df'
  secondary: '#ffb95f'
  on-secondary: '#472a00'
  secondary-container: '#ee9800'
  on-secondary-container: '#5b3800'
  tertiary: '#c4c6cf'
  on-tertiary: '#2e3037'
  tertiary-container: '#55585f'
  on-tertiary-container: '#cdced7'
  error: '#ffb4ab'
  on-error: '#690005'
  error-container: '#93000a'
  on-error-container: '#ffdad6'
  primary-fixed: '#ebddff'
  primary-fixed-dim: '#d3bbff'
  on-primary-fixed: '#250059'
  on-primary-fixed-variant: '#5b00c5'
  secondary-fixed: '#ffddb8'
  secondary-fixed-dim: '#ffb95f'
  on-secondary-fixed: '#2a1700'
  on-secondary-fixed-variant: '#653e00'
  tertiary-fixed: '#e1e2eb'
  tertiary-fixed-dim: '#c4c6cf'
  on-tertiary-fixed: '#191c22'
  on-tertiary-fixed-variant: '#44474e'
  background: '#101415'
  on-background: '#e0e3e5'
  surface-variant: '#323537'
typography:
  display-xl:
    fontFamily: Sora
    fontSize: 64px
    fontWeight: '700'
    lineHeight: '1.1'
    letterSpacing: 0.05em
  headline-lg:
    fontFamily: Sora
    fontSize: 40px
    fontWeight: '600'
    lineHeight: '1.2'
    letterSpacing: 0.02em
  headline-lg-mobile:
    fontFamily: Sora
    fontSize: 32px
    fontWeight: '600'
    lineHeight: '1.2'
    letterSpacing: 0.02em
  headline-md:
    fontFamily: Sora
    fontSize: 24px
    fontWeight: '500'
    lineHeight: '1.3'
  body-lg:
    fontFamily: Geist
    fontSize: 18px
    fontWeight: '400'
    lineHeight: '1.6'
  body-md:
    fontFamily: Geist
    fontSize: 16px
    fontWeight: '400'
    lineHeight: '1.5'
  label-sm:
    fontFamily: Geist
    fontSize: 12px
    fontWeight: '600'
    lineHeight: '1'
    letterSpacing: 0.1em
rounded:
  sm: 0.25rem
  DEFAULT: 0.5rem
  md: 0.75rem
  lg: 1rem
  xl: 1.5rem
  full: 9999px
spacing:
  unit: 8px
  container-margin-desktop: 64px
  container-margin-mobile: 20px
  gutter: 24px
  gap-lg: 40px
  gap-md: 24px
  gap-sm: 12px
---

## Brand & Style

This design system is built to evoke the vastness and mystery of the cosmos while maintaining the high-precision feel of aerospace technology. The target audience includes modern explorers and space tourists who value both safety and awe-inspiring experiences.

The aesthetic blends **Modern Glassmorphism** with a **Futuristic** technical edge. It utilizes deep, immersive backgrounds punctuated by vibrant, light-emitting accents. The interface should feel like a high-end cockpit display—translucent, layered, and illuminated from within. Whitespace is used generously to signify the "void" of space, ensuring that UI elements feel like celestial bodies floating in a structured vacuum.

## Colors

The palette is anchored in a dark-mode-first approach to simulate the deep vacuum of space.

*   **Deep Space Navy (#0B0E14):** The foundational layer. Used for all primary backgrounds and deep structural containers.
*   **Nebula Purple (#6D28D9):** The primary brand color. Used for interactive states, primary actions, and decorative glows.
*   **Supernova Orange (#F59E0B):** An energetic accent color. Reserved for critical calls-to-action (CTAs), status alerts, and high-priority navigation points.
*   **Starlight White (#F8FAFC):** High-contrast text and iconography to ensure maximum legibility against the dark void.

Color application should favor gradients and blurs to mimic the gaseous nature of nebulae, rather than flat fills.

## Typography

The typography strategy pairs expressive geometric headings with high-precision technical body copy.

**Sora** is utilized for display and headlines. Its wide apertures and geometric construction feel inherently futuristic. For all headlines, a wider tracking (letter spacing) is required to enhance the "expansive" feel of the system.

**Geist** is used for all UI and body text. Its monolinear, technical character provides the legibility needed for dense information (like flight coordinates or oxygen levels). Labels and small UI elements should utilize uppercase styling with generous tracking to mimic instrumentation panels.

## Layout & Spacing

This design system uses a **Fluid Grid** model based on a 12-column layout for desktop and a 4-column layout for mobile. 

Layouts should emphasize asymmetrical balance to feel more dynamic and organic, like planetary orbits. Spacing is governed by an 8px base unit. To maintain the "celestial" feel, use larger-than-standard margins (`64px` on desktop) to allow the content to breathe against the background star-field. Content should reflow vertically on mobile, with margins tightening to `20px` to maximize screen real estate for technical data.

## Elevation & Depth

Hierarchy is established through **Glassmorphism** and **Light Emission** rather than traditional shadows.

1.  **Base Layer:** The star-field background remains fixed.
2.  **Surface Layer:** All cards and containers use a semi-transparent Deep Space Navy fill (approx 40-60% opacity) with a `backdrop-filter: blur(20px)`.
3.  **Illumination:** Instead of drop shadows, active elements utilize a "Nebula Glow"—a soft, outer box-shadow using the Primary color with high diffusion and low opacity.
4.  **Borders:** Containers use a 1px solid border at 20% opacity of Starlight White. On hover or focus, these borders should transition to a gradient of Nebula Purple and Supernova Orange to simulate light-bending.

## Shapes

The shape language is **Rounded**, utilizing a `0.5rem` (8px) base radius. This softens the technical aesthetic, making the interface feel more approachable and ergonomic for travelers. Large hero sections and image containers should use the `rounded-xl` (1.5rem) setting to mimic the curved windows of a spacecraft. 

Interactive elements like pills or tags should remain fully rounded (`rounded-full`) to differentiate them from structural containers.

## Components

### Buttons
*   **Primary:** Supernova Orange fill with dark text. No shadow, but a subtle "inner glow" on hover.
*   **Secondary:** Ghost style with a Nebula Purple glowing border and white text.
*   **States:** On press, buttons should "contract" slightly (scale 0.98) to provide tactile feedback.

### Input Fields
Inputs should be transparent with a bottom-border only (2px Starlight White at 30% opacity). Upon focus, the border animates to full opacity with a 4px Nebula Purple glow underneath.

### Cards
Cards must utilize the glassmorphic style: semi-transparent navy background, heavy backdrop blur, and thin starlight borders. Content inside cards should be padded with `gap-md`.

### Chips & Badges
Small, pill-shaped elements used for status (e.g., "In Transit", "Docked"). Use a low-opacity fill of the status color with high-contrast text.

### Progress Bars / Gauges
Linear indicators should be used for fuel, oxygen, or time. Use the Supernova Orange for critical levels and Nebula Purple for standard progress, always featuring a subtle "pulsing" glow at the leading edge of the bar.

### Star-Field Backgrounds
All views should feature a subtle, multi-layered parallax star-field. The stars should vary in size and opacity, with occasional "nebula clouds" (blurred purple/blue gradients) at the edges of the viewport to add depth.