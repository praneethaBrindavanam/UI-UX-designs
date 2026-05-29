---
name: Aura
colors:
  surface: '#f8f9fa'
  surface-dim: '#d9dadb'
  surface-bright: '#f8f9fa'
  surface-container-lowest: '#ffffff'
  surface-container-low: '#f3f4f5'
  surface-container: '#edeeef'
  surface-container-high: '#e7e8e9'
  surface-container-highest: '#e1e3e4'
  on-surface: '#191c1d'
  on-surface-variant: '#404944'
  inverse-surface: '#2e3132'
  inverse-on-surface: '#f0f1f2'
  outline: '#707974'
  outline-variant: '#bfc9c3'
  surface-tint: '#2b6954'
  primary: '#003527'
  on-primary: '#ffffff'
  primary-container: '#064e3b'
  on-primary-container: '#80bea6'
  inverse-primary: '#95d3ba'
  secondary: '#416656'
  on-secondary: '#ffffff'
  secondary-container: '#c3ecd7'
  on-secondary-container: '#476c5b'
  tertiary: '#591700'
  on-tertiary: '#ffffff'
  tertiary-container: '#7f2400'
  on-tertiary-container: '#ff9572'
  error: '#ba1a1a'
  on-error: '#ffffff'
  error-container: '#ffdad6'
  on-error-container: '#93000a'
  primary-fixed: '#b0f0d6'
  primary-fixed-dim: '#95d3ba'
  on-primary-fixed: '#002117'
  on-primary-fixed-variant: '#0b513d'
  secondary-fixed: '#c3ecd7'
  secondary-fixed-dim: '#a8cfbc'
  on-secondary-fixed: '#002115'
  on-secondary-fixed-variant: '#294e3f'
  tertiary-fixed: '#ffdbd0'
  tertiary-fixed-dim: '#ffb59d'
  on-tertiary-fixed: '#390c00'
  on-tertiary-fixed-variant: '#832600'
  background: '#f8f9fa'
  on-background: '#191c1d'
  surface-variant: '#e1e3e4'
typography:
  display-lg:
    fontFamily: Playfair Display
    fontSize: 48px
    fontWeight: '700'
    lineHeight: 56px
    letterSpacing: -0.02em
  display-lg-mobile:
    fontFamily: Playfair Display
    fontSize: 36px
    fontWeight: '700'
    lineHeight: 44px
    letterSpacing: -0.01em
  headline-lg:
    fontFamily: Playfair Display
    fontSize: 32px
    fontWeight: '600'
    lineHeight: 40px
  headline-md:
    fontFamily: Playfair Display
    fontSize: 24px
    fontWeight: '600'
    lineHeight: 32px
  body-lg:
    fontFamily: Inter
    fontSize: 18px
    fontWeight: '400'
    lineHeight: 28px
  body-md:
    fontFamily: Inter
    fontSize: 16px
    fontWeight: '400'
    lineHeight: 24px
  label-lg:
    fontFamily: Inter
    fontSize: 14px
    fontWeight: '600'
    lineHeight: 20px
    letterSpacing: 0.05em
  label-sm:
    fontFamily: Inter
    fontSize: 12px
    fontWeight: '500'
    lineHeight: 16px
rounded:
  sm: 0.25rem
  DEFAULT: 0.5rem
  md: 0.75rem
  lg: 1rem
  xl: 1.5rem
  full: 9999px
spacing:
  base: 8px
  xs: 4px
  sm: 12px
  md: 24px
  lg: 48px
  xl: 80px
  gutter: 24px
  margin-mobile: 20px
  margin-desktop: 64px
---

## Brand & Style
The design system is built for a premium, boutique fitness experience that balances high-performance energy with a restorative, calm atmosphere. The brand personality is sophisticated, grounded, and intentional. It moves away from the aggressive aesthetics of traditional fitness, favoring a minimalist, editorial approach that feels more like a high-end wellness sanctuary.

The visual direction utilizes a "Quiet Premium" style—leveraging expansive whitespace, high-contrast serif typography for an editorial feel, and a refined color palette that draws inspiration from natural elements. The goal is to evoke a sense of focused energy and professional reliability.

## Colors
The palette is anchored by Deep Emerald, providing a sense of luxury and stability. Soft Sage acts as a calming secondary tone for large surfaces and backgrounds, while Warm Terracotta is reserved strictly for high-impact calls to action and active status indicators.

- **Primary (Deep Emerald):** Used for primary buttons, active navigation states, and bold brand expressions.
- **Secondary (Soft Sage):** Used for subtle backgrounds, secondary buttons, and highlighted container states.
- **Accent (Warm Terracotta):** Used sparingly for "Book Now" actions and urgent alerts.
- **Background/Surface:** The use of Off-white for the main background and pure White for cards ensures a crisp, layered hierarchy that remains easy on the eyes.

## Typography
This design system employs a classic high-contrast pairing: a sophisticated serif for headlines and a functional, neutral sans-serif for body copy.

- **Headlines:** Playfair Display provides an editorial, premium feel. Use `display-lg` for hero sections and `headline-lg` for major module titles.
- **Body:** Inter is used for all functional text to ensure maximum readability during active use.
- **Labels:** Use uppercase for small labels and buttons to create a structured, "architectural" feel.

## Layout & Spacing
The layout follows a 12-column fluid grid on desktop and a 4-column grid on mobile. To maintain the "Aura" of the brand, generous whitespace is mandatory. 

- **Vertical Rhythm:** Use `xl` spacing between major sections to allow the content to breathe.
- **Margins:** Desktop views should feature wide margins (`margin-desktop`) to center the content and prevent it from feeling overwhelming.
- **Grids:** Use a 24px gutter for card layouts. For content-heavy pages, a centered 8-column layout is preferred over a full-width 12-column layout to preserve the editorial aesthetic.

## Elevation & Depth
Depth is communicated through tonal layering rather than heavy shadows. 
- **Levels:** Surfaces sit on the `neutral` background. Cards use pure white with a very soft, diffused shadow (0px 4px 20px rgba(0, 0, 0, 0.05)).
- **Interactions:** When an element is hovered, the shadow should slightly deepen, and the element may scale up by 1% to provide a tactile, responsive feel.
- **Separation:** Use thin 1px borders in `Soft Sage` for non-elevated containers to define boundaries without adding visual weight.

## Shapes
The shape language is "Rounded" to reflect the fluid nature of movement and the approachable side of the brand.
- **Default (8px):** Applied to input fields, small buttons, and UI controls.
- **Large (16px):** Applied to cards, modal containers, and feature images.
- **Extra Large (24px):** Applied to top-level layout containers or specific promotional banners.
- **Pill:** Reserved exclusively for tags and status chips.

## Components
- **Buttons:** Primary buttons use Deep Emerald with white text. Secondary buttons use a Soft Sage background with Deep Emerald text. The Warm Terracotta button is used exclusively for "Book" actions.
- **Input Fields:** Use 1px Soft Sage borders that transition to Deep Emerald on focus. Placeholder text should be a lightened Charcoal.
- **Cards:** White background with `rounded-lg` corners and a subtle shadow. Content within cards should have at least 24px of internal padding.
- **Chips/Tags:** Use the Pill shape. Active class tags use Soft Sage with Deep Emerald text; category tags use a light neutral background.
- **Lists:** Clean dividers using 1px Soft Sage lines. Use thin-line icons (1.5pt stroke) to maintain the minimalist aesthetic.
- **Schedule Component:** A custom component for fitness classes. Each class block should use the editorial serif for the time and name, with a secondary label for the instructor.