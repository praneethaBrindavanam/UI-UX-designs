---
name: Voyage Elite
colors:
  surface: '#f8f9ff'
  surface-dim: '#cbdbf5'
  surface-bright: '#f8f9ff'
  surface-container-lowest: '#ffffff'
  surface-container-low: '#eff4ff'
  surface-container: '#e5eeff'
  surface-container-high: '#dce9ff'
  surface-container-highest: '#d3e4fe'
  on-surface: '#0b1c30'
  on-surface-variant: '#45464d'
  inverse-surface: '#213145'
  inverse-on-surface: '#eaf1ff'
  outline: '#76777d'
  outline-variant: '#c6c6cd'
  surface-tint: '#565e74'
  primary: '#000000'
  on-primary: '#ffffff'
  primary-container: '#131b2e'
  on-primary-container: '#7c839b'
  inverse-primary: '#bec6e0'
  secondary: '#006a61'
  on-secondary: '#ffffff'
  secondary-container: '#86f2e4'
  on-secondary-container: '#006f66'
  tertiary: '#000000'
  on-tertiary: '#ffffff'
  tertiary-container: '#191c1e'
  on-tertiary-container: '#818486'
  error: '#ba1a1a'
  on-error: '#ffffff'
  error-container: '#ffdad6'
  on-error-container: '#93000a'
  primary-fixed: '#dae2fd'
  primary-fixed-dim: '#bec6e0'
  on-primary-fixed: '#131b2e'
  on-primary-fixed-variant: '#3f465c'
  secondary-fixed: '#89f5e7'
  secondary-fixed-dim: '#6bd8cb'
  on-secondary-fixed: '#00201d'
  on-secondary-fixed-variant: '#005049'
  tertiary-fixed: '#e0e3e5'
  tertiary-fixed-dim: '#c4c7c9'
  on-tertiary-fixed: '#191c1e'
  on-tertiary-fixed-variant: '#444749'
  background: '#f8f9ff'
  on-background: '#0b1c30'
  surface-variant: '#d3e4fe'
typography:
  headline-lg:
    fontFamily: Plus Jakarta Sans
    fontSize: 32px
    fontWeight: '700'
    lineHeight: '1.2'
  headline-md:
    fontFamily: Plus Jakarta Sans
    fontSize: 24px
    fontWeight: '600'
    lineHeight: '1.3'
  headline-sm:
    fontFamily: Plus Jakarta Sans
    fontSize: 20px
    fontWeight: '600'
    lineHeight: '1.4'
  body-lg:
    fontFamily: Inter
    fontSize: 18px
    fontWeight: '400'
    lineHeight: '1.6'
  body-md:
    fontFamily: Inter
    fontSize: 16px
    fontWeight: '400'
    lineHeight: '1.6'
  body-sm:
    fontFamily: Inter
    fontSize: 14px
    fontWeight: '400'
    lineHeight: '1.5'
  label-md:
    fontFamily: Inter
    fontSize: 14px
    fontWeight: '600'
    lineHeight: '1'
    letterSpacing: 0.02em
  label-sm:
    fontFamily: Inter
    fontSize: 12px
    fontWeight: '500'
    lineHeight: '1'
    letterSpacing: 0.04em
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
  xl: 48px
  gutter: 16px
  margin-mobile: 20px
  margin-desktop: 64px
---

## Brand & Style

The brand personality focuses on reliability, discovery, and effortless precision. It targets modern travelers who value both efficiency and a sense of premium security. The UI evokes a feeling of calm authority—reducing the "travel anxiety" often associated with booking logistics through a refined, spacious aesthetic.

This design system utilizes a **Corporate Modern** style with **Minimalist** leanings. It prioritizes clarity through generous whitespace and a restricted color palette, while using subtle depth cues to guide the user's eye toward critical booking actions. The interface is grounded and professional, avoiding decorative clutter in favor of high-legibility and functional elegance.

## Colors

The palette is anchored by **Deep Navy (#0F172A)**, chosen to instill an immediate sense of institutional trust and permanence. This is contrasted by **Vibrant Teal (#0D9488)**, which serves as the primary action color, drawing the eye to conversion points like "Book Now" or "Search."

The background strategy relies on **Off-White/Slate-50 (#F8FAFC)** to distinguish between card surfaces and the page background without introducing heavy borders. Semantic colors for status indicators include a soft emerald for confirmed bookings, a muted amber for pending states, and a clean crimson for alerts, all adjusted for high legibility against white backgrounds.

## Typography

This design system uses a dual-font strategy to balance character with utility. **Plus Jakarta Sans** is used for headlines to provide a welcoming, contemporary feel with its slightly rounded apertures. **Inter** is utilized for body copy and labels to ensure maximum readability and a systematic, clean appearance across dense information displays.

Hierarchy is established through significant weight shifts. Headlines use Bold or Semi-Bold weights to anchor sections, while body text remains in Regular weight to maintain a light, airy feel. Captions and small labels use Medium weights with slight letter-spacing to maintain legibility at reduced scales.

## Layout & Spacing

The design system employs a **Fluid Grid** model based on an 8px rhythm. For mobile interfaces, a 4-column grid is used with 20px side margins; for desktop, a 12-column grid is utilized with 64px margins. 

The spacing philosophy emphasizes "Macro-Whitespace"—larger gaps between sections (xl) to allow the eye to rest, while keeping related elements within a card grouped with tighter spacing (sm to md). Gutters are fixed at 16px to maintain a dense but organized information density in search results.

## Elevation & Depth

Depth is signaled through **Ambient Shadows** rather than lines. This system avoids harsh borders, instead using soft, diffused shadows with a slight blue tint (`rgba(15, 23, 42, 0.08)`) to lift cards off the background. 

Three levels of elevation are defined:
1. **Level 0 (Flat):** Used for the main background.
2. **Level 1 (Subtle):** Used for content cards (hotels, flights). Features a 4px blur with 2px vertical offset.
3. **Level 2 (Active):** Used for hovered elements or modals. Features a 12px blur with 6px vertical offset to create a "floating" effect.

## Shapes

The shape language is consistently **Rounded**, using a 0.5rem (8px) base radius. This softens the professional tone of the deep blues, making the app feel more accessible and user-friendly. 

Interactive elements like primary buttons and search inputs follow the base radius, while large container cards or image carousels may use `rounded-lg` (16px) to emphasize their role as primary content buckets. Status badges use a full pill-shape to distinguish them from interactive buttons.

## Components

### Buttons & Actions
Primary buttons use the Vibrant Teal fill with white text. They feature a subtle 2px scale-down effect on press. Secondary buttons use a Deep Navy outline or a ghost style for less critical actions.

### Cards
Booking cards are the core component. They feature an image-top or image-left layout, Level 1 elevation, and 16px internal padding. Price points are always anchored to the bottom-right in Plus Jakarta Sans Bold.

### Inputs & Search
Search bars use a white background with a 1px Slate-200 border. Upon focus, the border shifts to Teal with a subtle glow. Icons are used within inputs to provide visual cues (e.g., a calendar icon for dates).

### Status Indicators
Status indicators (e.g., "Confirmed," "Delayed," "Refunded") are styled as small, pill-shaped chips. They use a low-opacity background tint of the semantic color with high-contrast text for accessibility.

### Progress Trackers
For multi-step bookings, a "Stepper" component uses thin lines and numbered circles in Deep Navy to show progress, with the current step highlighted in Teal.