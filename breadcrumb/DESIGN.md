---
name: Precision & Clarity
colors:
  surface: '#faf8ff'
  surface-dim: '#d2d9f4'
  surface-bright: '#faf8ff'
  surface-container-lowest: '#ffffff'
  surface-container-low: '#f2f3ff'
  surface-container: '#eaedff'
  surface-container-high: '#e2e7ff'
  surface-container-highest: '#dae2fd'
  on-surface: '#131b2e'
  on-surface-variant: '#434655'
  inverse-surface: '#283044'
  inverse-on-surface: '#eef0ff'
  outline: '#737686'
  outline-variant: '#c3c6d7'
  surface-tint: '#0053db'
  primary: '#004ac6'
  on-primary: '#ffffff'
  primary-container: '#2563eb'
  on-primary-container: '#eeefff'
  inverse-primary: '#b4c5ff'
  secondary: '#505f76'
  on-secondary: '#ffffff'
  secondary-container: '#d0e1fb'
  on-secondary-container: '#54647a'
  tertiary: '#943700'
  on-tertiary: '#ffffff'
  tertiary-container: '#bc4800'
  on-tertiary-container: '#ffede6'
  error: '#ba1a1a'
  on-error: '#ffffff'
  error-container: '#ffdad6'
  on-error-container: '#93000a'
  primary-fixed: '#dbe1ff'
  primary-fixed-dim: '#b4c5ff'
  on-primary-fixed: '#00174b'
  on-primary-fixed-variant: '#003ea8'
  secondary-fixed: '#d3e4fe'
  secondary-fixed-dim: '#b7c8e1'
  on-secondary-fixed: '#0b1c30'
  on-secondary-fixed-variant: '#38485d'
  tertiary-fixed: '#ffdbcd'
  tertiary-fixed-dim: '#ffb596'
  on-tertiary-fixed: '#360f00'
  on-tertiary-fixed-variant: '#7d2d00'
  background: '#faf8ff'
  on-background: '#131b2e'
  surface-variant: '#dae2fd'
typography:
  display-xl:
    fontFamily: Manrope
    fontSize: 48px
    fontWeight: '700'
    lineHeight: '1.1'
    letterSpacing: -0.02em
  display-lg:
    fontFamily: Manrope
    fontSize: 36px
    fontWeight: '700'
    lineHeight: '1.2'
    letterSpacing: -0.02em
  headline-md:
    fontFamily: Manrope
    fontSize: 24px
    fontWeight: '600'
    lineHeight: '1.3'
    letterSpacing: -0.01em
  headline-sm:
    fontFamily: Manrope
    fontSize: 20px
    fontWeight: '600'
    lineHeight: '1.4'
    letterSpacing: '0'
  body-lg:
    fontFamily: Inter
    fontSize: 18px
    fontWeight: '400'
    lineHeight: '1.6'
    letterSpacing: '0'
  body-md:
    fontFamily: Inter
    fontSize: 16px
    fontWeight: '400'
    lineHeight: '1.5'
    letterSpacing: '0'
  body-sm:
    fontFamily: Inter
    fontSize: 14px
    fontWeight: '400'
    lineHeight: '1.5'
    letterSpacing: '0'
  label-md:
    fontFamily: Inter
    fontSize: 12px
    fontWeight: '600'
    lineHeight: '1'
    letterSpacing: 0.05em
  label-sm:
    fontFamily: Inter
    fontSize: 11px
    fontWeight: '500'
    lineHeight: '1'
    letterSpacing: 0.02em
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
  xxl: 48px
  gutter: 24px
  margin-page: 40px
---

## Brand & Style
This design system is built on the principles of **Modern Minimalism** with a **Corporate / Modern** execution. It targets professional environments where information density must be balanced with extreme readability. The brand personality is disciplined, sophisticated, and high-functioning, evoking a sense of calm efficiency.

The visual language avoids unnecessary decoration, relying instead on mathematical precision in spacing and a strict typographic hierarchy. The aesthetic is "quiet" to allow the user's content to take center stage, using subtle motion and purposeful color accents to guide interaction without overwhelming the senses.

## Colors
The palette is rooted in a "Greyscale Plus One" philosophy. The primary interaction color is a precise, high-visibility blue used exclusively for actionable elements, progress indicators, and active states. 

- **Primary:** Used for primary buttons, active toggles, and critical wayfinding.
- **Secondary:** A muted slate used for supporting information and less emphasized UI controls.
- **Neutral:** A deep navy-black for maximum text contrast.
- **Surface & Background:** Layers of near-white and soft grey create a sense of depth and separation without the need for heavy borders.

## Typography
The system utilizes a dual-font pairing to distinguish between structural "editorial" elements and functional "interface" elements. 

**Manrope** is used for headlines to provide a modern, slightly geometric character that feels premium and balanced. **Inter** is used for all body copy and UI labels due to its exceptional legibility at small sizes and its neutral, utilitarian tone. 

Maintain a strict vertical rhythm by adhering to the defined line heights. Use `label-md` for secondary metadata and section headers to introduce variety without adding new colors.

## Layout & Spacing
The layout follows a **Fixed Grid** model for desktop (1280px max-width) and a **Fluid Grid** for mobile devices. The system is built on a 4px baseline grid to ensure all components align perfectly.

- **Grid:** 12-column layout with 24px gutters. 
- **Rhythm:** Use `md` (16px) for internal component padding and `lg` (24px) for spacing between distinct logical groups. 
- **Whitespace:** Use generous `xxl` (48px) margins between major sections to prevent visual clutter and signal a change in context.

## Elevation & Depth
This design system uses **Tonal Layers** supplemented by **Ambient Shadows** to create hierarchy. 

1.  **Level 0 (Background):** The base layer using the background color hex.
2.  **Level 1 (Surface):** Cards and main content areas using the surface color hex. These use a very subtle 1px border (#E2E8F0) rather than a shadow to maintain a "flat-modern" look.
3.  **Level 2 (Interactive/Floating):** Modals, dropdowns, and active cards. These use extra-diffused, low-opacity shadows (Offset: 0, 10px; Blur: 15px; Color: rgba(15, 23, 42, 0.05)).

Avoid heavy blurs or glassmorphism. Depth should feel physical but understated.

## Shapes
The design system utilizes **Soft** roundedness. This provides a approachable feel while maintaining the professional rigor of a grid-based layout. 

- **Small Components (Buttons, Inputs):** 0.25rem (4px) corner radius.
- **Medium Components (Cards, Modals):** 0.5rem (8px) corner radius.
- **Large Containers:** 0.75rem (12px) corner radius.

Iconography should follow this rule, using a 1.5pt or 2pt stroke weight with slightly rounded caps and joins to match the component geometry.

## Components
- **Buttons:** Primary buttons use the primary accent color with white text. Secondary buttons use a ghost style (light grey background or simple border). All buttons feature a 4px radius and 16px horizontal padding.
- **Inputs:** Fields use a 1px border (#CBD5E1). On focus, the border shifts to the primary color with a subtle 2px outer glow (primary color at 10% opacity).
- **Chips:** Used for filtering and tags. These are low-contrast, using a light grey background and `label-sm` typography. Active chips toggle to the primary color.
- **Cards:** Cards should be border-only for static content and use a subtle ambient shadow on hover if they are clickable.
- **Lists:** Maintain high readability with 12px vertical padding between items and a light divider (#F1F5F9).
- **Iconography:** Use a consistent 24px bounding box for all icons. Icons should be "Line Art" style, never filled, unless in an active/selected state.