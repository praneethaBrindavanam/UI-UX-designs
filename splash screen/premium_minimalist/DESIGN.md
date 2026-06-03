---
name: Premium Minimalist
colors:
  surface: '#f7f9fb'
  surface-dim: '#d8dadc'
  surface-bright: '#f7f9fb'
  surface-container-lowest: '#ffffff'
  surface-container-low: '#f2f4f6'
  surface-container: '#eceef0'
  surface-container-high: '#e6e8ea'
  surface-container-highest: '#e0e3e5'
  on-surface: '#191c1e'
  on-surface-variant: '#464555'
  inverse-surface: '#2d3133'
  inverse-on-surface: '#eff1f3'
  outline: '#777587'
  outline-variant: '#c7c4d8'
  surface-tint: '#4d44e3'
  primary: '#3525cd'
  on-primary: '#ffffff'
  primary-container: '#4f46e5'
  on-primary-container: '#dad7ff'
  inverse-primary: '#c3c0ff'
  secondary: '#565e74'
  on-secondary: '#ffffff'
  secondary-container: '#dae2fd'
  on-secondary-container: '#5c647a'
  tertiary: '#00524b'
  on-tertiary: '#ffffff'
  tertiary-container: '#006c63'
  on-tertiary-container: '#81eddf'
  error: '#ba1a1a'
  on-error: '#ffffff'
  error-container: '#ffdad6'
  on-error-container: '#93000a'
  primary-fixed: '#e2dfff'
  primary-fixed-dim: '#c3c0ff'
  on-primary-fixed: '#0f0069'
  on-primary-fixed-variant: '#3323cc'
  secondary-fixed: '#dae2fd'
  secondary-fixed-dim: '#bec6e0'
  on-secondary-fixed: '#131b2e'
  on-secondary-fixed-variant: '#3f465c'
  tertiary-fixed: '#89f5e7'
  tertiary-fixed-dim: '#6bd8cb'
  on-tertiary-fixed: '#00201d'
  on-tertiary-fixed-variant: '#005049'
  background: '#f7f9fb'
  on-background: '#191c1e'
  surface-variant: '#e0e3e5'
typography:
  headline-lg:
    fontFamily: Manrope
    fontSize: 32px
    fontWeight: '700'
    lineHeight: 40px
    letterSpacing: -0.02em
  headline-lg-mobile:
    fontFamily: Manrope
    fontSize: 24px
    fontWeight: '700'
    lineHeight: 32px
    letterSpacing: -0.01em
  headline-md:
    fontFamily: Manrope
    fontSize: 24px
    fontWeight: '600'
    lineHeight: 32px
  body-lg:
    fontFamily: Manrope
    fontSize: 18px
    fontWeight: '400'
    lineHeight: 28px
  body-md:
    fontFamily: Manrope
    fontSize: 16px
    fontWeight: '400'
    lineHeight: 24px
  label-md:
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
    letterSpacing: 0.05em
rounded:
  sm: 0.25rem
  DEFAULT: 0.5rem
  md: 0.75rem
  lg: 1rem
  xl: 1.5rem
  full: 9999px
spacing:
  unit: 4px
  gutter: 16px
  margin-mobile: 20px
  margin-desktop: 40px
  stack-sm: 8px
  stack-md: 24px
  stack-lg: 48px
---

## Brand & Style
The design system is anchored in the "Premium Minimalist" aesthetic, prioritizing clarity, intentionality, and a sense of calm. It is designed for users who value precision and sophistication, evoking a feeling of quiet confidence and institutional trust.

The visual language avoids unnecessary decoration, instead using generous whitespace, expert typography, and a refined color palette to guide the user's attention. The emotional response should be one of "effortless control"—where the interface feels light and unobtrusive, yet robust and reliable.

## Colors
The palette is built on a foundation of "Deep Space" neutrals and "Electric" accents. 

- **Primary (Electric Indigo):** Used sparingly for key actions and brand moments to provide a modern, energetic spark against the calm background.
- **Secondary (Charcoal Blue):** The primary color for text, iconography, and high-level structural elements, ensuring a grounded and authoritative feel.
- **Tertiary (Teal):** Reserved for success states or secondary data visualizations, providing a cool-toned contrast to the indigo.
- **Neutral:** A range of slate-tinted greys. The background is a very bright, nearly-white slate to maintain a premium "gallery" feel without the harshness of pure white.

## Typography
The system utilizes **Manrope** for its balanced, modern proportions and excellent legibility at all scales. Its geometric tendencies are softened by humanist touches, making it feel both technical and approachable.

For functional elements like data points, captions, and small labels, **Geist** is introduced. Its monospaced-adjacent tracking and precise glyphs provide a "developer-grade" clarity that reinforces the sense of trustworthiness and accuracy. Headlines should use tighter letter-spacing to feel more "locked-in" and editorial.

## Layout & Spacing
The design system employs a **Fluid-Fixed hybrid grid**. On mobile devices, it uses a 4-column grid with 20px side margins. On larger screens, it transitions to a 12-column centered layout.

The spacing philosophy is "Air First." Vertical rhythm is governed by a 4px baseline, but significant sections are separated by large increments (48px+) to prevent the UI from feeling cramped. Elements within a card or group should be tightly related (8px - 12px), while the groups themselves should have ample room to breathe.

## Elevation & Depth
Depth is conveyed through **Tonal Layering** rather than traditional heavy shadows. Surfaces exist on three primary planes:

1.  **Base (Level 0):** The primary background color.
2.  **Surface (Level 1):** White or slightly off-white cards with an extremely subtle, 1px neutral-200 border. No shadow.
3.  **Raised (Level 2):** For active modals or floating elements, use a "Soft Ambient" shadow: a large blur radius (24px+) with very low opacity (4-6%) indigo-tinted shadow.

This approach creates a sense of "layered paper" or "stacked glass" that feels modern and high-end.

## Shapes
The system uses a **Rounded** corner strategy. The base radius of 8px (`rounded`) creates a contemporary feel that is softer than industrial square corners but more structured than playful pill-shapes. 

- **Containers:** Use `rounded-lg` (16px) for main content cards to create a clear "container" metaphor.
- **Interactive Elements:** Buttons and input fields use the base 8px radius to maintain a crisp, professional appearance.
- **Icons:** Should follow a similar corner radius (approx 2px internally) to ensure visual harmony with the UI.

## Components
- **Buttons:** Primary buttons are solid Electric Indigo with white text. Secondary buttons use a transparent background with a 1.5px Charcoal Blue border. Avoid "ghost" buttons for primary actions to maintain clear hierarchy.
- **Input Fields:** Use a subtle background fill (Neutral-100) instead of a bottom line. On focus, the border should transition to a 2px Indigo stroke. Labels should always be visible above the field using the `label-sm` style.
- **Cards:** Cards are the primary organizational unit. They should have no shadow by default, relying on the Neutral-200 border for definition. Padding inside cards should be a minimum of 20px.
- **Chips/Badges:** Use a light tint of the primary or tertiary color (e.g., 10% Indigo) with high-contrast text for status indicators.
- **Navigation:** A clean bottom navigation bar on mobile with thin-stroke icons. The active state is indicated by a color shift to Indigo and a small 4px dot below the icon.