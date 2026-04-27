---
name: Luminous Navigation
colors:
  surface: '#121414'
  surface-dim: '#121414'
  surface-bright: '#37393a'
  surface-container-lowest: '#0c0f0f'
  surface-container-low: '#1a1c1c'
  surface-container: '#1e2020'
  surface-container-high: '#282a2b'
  surface-container-highest: '#333535'
  on-surface: '#e2e2e2'
  on-surface-variant: '#c5c6cd'
  inverse-surface: '#e2e2e2'
  inverse-on-surface: '#2f3131'
  outline: '#8f9097'
  outline-variant: '#44474d'
  surface-tint: '#b9c7e4'
  primary: '#b9c7e4'
  on-primary: '#233148'
  primary-container: '#0a192f'
  on-primary-container: '#74829d'
  inverse-primary: '#515f78'
  secondary: '#adc7ff'
  on-secondary: '#002e68'
  secondary-container: '#4a8eff'
  on-secondary-container: '#00285b'
  tertiary: '#00dbe9'
  on-tertiary: '#00363a'
  tertiary-container: '#001d1f'
  on-tertiary-container: '#009099'
  error: '#ffb4ab'
  on-error: '#690005'
  error-container: '#93000a'
  on-error-container: '#ffdad6'
  primary-fixed: '#d6e3ff'
  primary-fixed-dim: '#b9c7e4'
  on-primary-fixed: '#0d1c32'
  on-primary-fixed-variant: '#39475f'
  secondary-fixed: '#d8e2ff'
  secondary-fixed-dim: '#adc7ff'
  on-secondary-fixed: '#001a41'
  on-secondary-fixed-variant: '#004493'
  tertiary-fixed: '#7df4ff'
  tertiary-fixed-dim: '#00dbe9'
  on-tertiary-fixed: '#002022'
  on-tertiary-fixed-variant: '#004f54'
  background: '#121414'
  on-background: '#e2e2e2'
  surface-variant: '#333535'
typography:
  h1:
    fontFamily: Inter
    fontSize: 32px
    fontWeight: '700'
    lineHeight: '1.2'
    letterSpacing: -0.02em
  h2:
    fontFamily: Inter
    fontSize: 24px
    fontWeight: '600'
    lineHeight: '1.3'
    letterSpacing: -0.01em
  body-lg:
    fontFamily: Inter
    fontSize: 18px
    fontWeight: '400'
    lineHeight: '1.5'
    letterSpacing: '0'
  body-md:
    fontFamily: Inter
    fontSize: 16px
    fontWeight: '400'
    lineHeight: '1.5'
    letterSpacing: '0'
  label-caps:
    fontFamily: Inter
    fontSize: 12px
    fontWeight: '700'
    lineHeight: '1.0'
    letterSpacing: 0.05em
  button:
    fontFamily: Inter
    fontSize: 16px
    fontWeight: '600'
    lineHeight: '1.0'
    letterSpacing: 0.01em
rounded:
  sm: 0.25rem
  DEFAULT: 0.5rem
  md: 0.75rem
  lg: 1rem
  xl: 1.5rem
  full: 9999px
spacing:
  unit: 4px
  xs: 4px
  sm: 8px
  md: 16px
  lg: 24px
  xl: 32px
  container-margin: 20px
  gutter: 12px
---

## Brand & Style

This design system is built on a foundation of "Digital Depth," a sophisticated aesthetic designed for high-performance mobile navigation. It prioritizes clarity and innovative spatial awareness, utilizing a refined **Glassmorphic** style to create a sense of layering without clutter. 

The brand personality is professional yet cutting-edge—evoking the feeling of a high-end aerospace interface or a premium financial dashboard. The goal is to make the user feel empowered and focused, using transparency and blurs to maintain context while highlighting the most critical navigation paths.

The visual language relies on:
- **Translucency:** To imply hierarchy and persistent context.
- **Precision:** Through crisp borders and high-contrast accents.
- **Fluidity:** Through soft shadows that simulate physical light sources behind the glass panes.

## Colors

The palette is anchored in a dark-mode-first approach to maximize the "glow" effect of the glassmorphic elements. 

- **Primary:** Deep Navy (#0A192F) serves as the infinite background and the base for solid surfaces.
- **Secondary:** Vibrant Electric Blue (#007BFF) is the core action color, used for primary buttons and active states.
- **Tertiary:** Cyan Spark (#00F0FF) is used sparingly for data visualization highlights and micro-interactions to provide a "tech" feel.
- **Neutral:** Crisp White (#FFFFFF) and various opacities of white are used for typography and delicate border highlights.

Surface colors should utilize `rgba(255, 255, 255, 0.05)` for glass backgrounds, ensuring legibility against the deep navy base.

## Typography

This design system utilizes **Inter** for its exceptional readability on mobile screens and its neutral, systematic character. 

The typographic hierarchy is "Bottom-Heavy," meaning labels and body text are treated with as much care as headlines to ensure navigation utility.
- Use **H1** for main screen titles.
- Use **Label-Caps** for category headers and utility text, always in uppercase with increased letter spacing.
- Contrast is achieved primarily through weight and color (Pure White for headlines, 70% White for secondary body).

## Layout & Spacing

This design system uses a **Fluid Grid** with a 4px baseline rhythm. For mobile navigation, a 4-column grid is the standard for content, while the navigation elements often float above the grid using safe-area margins.

- **Safe Zones:** Maintain a 20px horizontal margin for all primary content.
- **Rhythm:** Use 16px (md) for standard padding within cards and 8px (sm) for internal element spacing.
- **Negative Space:** Embrace generous top-of-screen breathing room to allow the background deep navy to provide visual rest.

## Elevation & Depth

Depth is the defining characteristic of this design system. It is communicated through three specific layers:

1.  **The Void (Base):** The solid Deep Navy background.
2.  **Glass Panes (Level 1):** Semi-transparent surfaces (`rgba(255, 255, 255, 0.05)`) with a 20px backdrop blur and a 1px solid border at 10% white opacity. This creates the "frosted" look.
3.  **Active Elements (Level 2):** Elements that float higher. These use a subtle electric blue glow (`drop-shadow: 0 8px 24px rgba(0, 123, 255, 0.2)`) instead of standard black shadows.

Shadows should be diffused and wide. Avoid sharp, dark shadows; instead, use tinted blurs to suggest light emitting from the UI elements.

## Shapes

The shape language is modern and approachable, using **Rounded** (Level 2) corners to soften the technical nature of the navy and blue palette.

- **Cards/Modules:** Use a 16px (rounded-lg) corner radius.
- **Buttons/Inputs:** Use an 8px (standard) corner radius.
- **Search Bars:** Should be fully rounded (Pill-shaped) to distinguish them from actionable containers.
- **Borders:** All glass elements must have a 1px "inner glow" border to define the edge against the dark background.

## Components

- **Navigation Bar:** A floating glass dock at the bottom of the screen. Icons use the primary blue for active states and a 40% white for inactive.
- **Glass Buttons:** Primary buttons are solid Electric Blue with a slight inner top-highlight. Secondary buttons are glass-textured with a white border.
- **Chips:** Small, high-radius (pill) elements. Active chips should use a Tertiary Cyan stroke.
- **Cards:** Background-blurred containers with a 1px top-left highlight border to simulate a light source.
- **Inputs:** Darker than the background with a subtle inner shadow. On focus, the border transitions to Electric Blue with a soft outer glow.
- **Lists:** Separated by thin, 5% white opacity lines. Each list item should have a subtle horizontal press-state that increases the background opacity to 10%.
- **Navigation Indicator:** A subtle horizontal "dash" under active menu items, rendered in Tertiary Cyan to draw the eye.