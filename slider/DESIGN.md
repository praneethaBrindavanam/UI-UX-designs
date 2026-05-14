---
name: Aura Luxury Estates
colors:
  surface: '#f9f9f9'
  surface-dim: '#dadada'
  surface-bright: '#f9f9f9'
  surface-container-lowest: '#ffffff'
  surface-container-low: '#f3f3f3'
  surface-container: '#eeeeee'
  surface-container-high: '#e8e8e8'
  surface-container-highest: '#e2e2e2'
  on-surface: '#1a1c1c'
  on-surface-variant: '#45474a'
  inverse-surface: '#2f3131'
  inverse-on-surface: '#f1f1f1'
  outline: '#76777b'
  outline-variant: '#c6c6ca'
  surface-tint: '#5d5e62'
  primary: '#000000'
  on-primary: '#ffffff'
  primary-container: '#1a1c1f'
  on-primary-container: '#838487'
  inverse-primary: '#c6c6ca'
  secondary: '#755a26'
  on-secondary: '#ffffff'
  secondary-container: '#fdd798'
  on-secondary-container: '#785c29'
  tertiary: '#000000'
  on-tertiary: '#ffffff'
  tertiary-container: '#091d2e'
  on-tertiary-container: '#73869a'
  error: '#ba1a1a'
  on-error: '#ffffff'
  error-container: '#ffdad6'
  on-error-container: '#93000a'
  primary-fixed: '#e2e2e6'
  primary-fixed-dim: '#c6c6ca'
  on-primary-fixed: '#1a1c1f'
  on-primary-fixed-variant: '#45474a'
  secondary-fixed: '#ffdea8'
  secondary-fixed-dim: '#e6c183'
  on-secondary-fixed: '#271900'
  on-secondary-fixed-variant: '#5b4311'
  tertiary-fixed: '#d1e4fb'
  tertiary-fixed-dim: '#b5c8df'
  on-tertiary-fixed: '#091d2e'
  on-tertiary-fixed-variant: '#36485b'
  background: '#f9f9f9'
  on-background: '#1a1c1c'
  surface-variant: '#e2e2e2'
typography:
  display-lg:
    fontFamily: Bodoni Moda
    fontSize: 64px
    fontWeight: '600'
    lineHeight: 72px
    letterSpacing: -0.02em
  display-lg-mobile:
    fontFamily: Bodoni Moda
    fontSize: 40px
    fontWeight: '600'
    lineHeight: 48px
    letterSpacing: -0.01em
  headline-lg:
    fontFamily: Bodoni Moda
    fontSize: 48px
    fontWeight: '500'
    lineHeight: 56px
  headline-lg-mobile:
    fontFamily: Bodoni Moda
    fontSize: 32px
    fontWeight: '500'
    lineHeight: 40px
  headline-md:
    fontFamily: Bodoni Moda
    fontSize: 32px
    fontWeight: '500'
    lineHeight: 40px
  title-lg:
    fontFamily: Manrope
    fontSize: 20px
    fontWeight: '600'
    lineHeight: 28px
    letterSpacing: 0.01em
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
    fontFamily: Manrope
    fontSize: 14px
    fontWeight: '600'
    lineHeight: 20px
    letterSpacing: 0.05em
rounded:
  sm: 0.25rem
  DEFAULT: 0.5rem
  md: 0.75rem
  lg: 1rem
  xl: 1.5rem
  full: 9999px
spacing:
  unit: 8px
  container-max-width: 1440px
  gutter: 24px
  margin-mobile: 20px
  margin-desktop: 64px
  stack-sm: 16px
  stack-md: 32px
  stack-lg: 80px
---

## Brand & Style

This design system is engineered for the high-end luxury real estate market, targeting ultra-high-net-worth individuals who value discretion, architectural excellence, and seamless digital experiences. The brand personality is "Quiet Luxury"—sophisticated, intentional, and authoritative without being loud.

The visual style is **Modern Minimalist with Tonal Layering**. It prioritizes expansive whitespace (often referred to as "architectural breathing room") and high-quality editorial photography. The emotional response should be one of calm confidence, reliability, and exclusivity. By utilizing a restrained color palette and sharp typographic hierarchy, the UI recedes to let the properties remain the primary focus.

## Colors

The palette is anchored in high-contrast neutrals to establish a premium editorial feel.

*   **Primary (Deep Charcoal):** Used for primary text, iconography, and structural borders. It provides a more sophisticated depth than pure black.
*   **Secondary (Muted Gold):** Reserved for high-intent actions, selected states, and premium signifiers (e.g., "Verified Listing").
*   **Tertiary (Elegant Navy):** Used sparingly for interactive elements or as a subtle background variation to differentiate content blocks.
*   **Neutral (Crisp White/Off-White):** The foundation of the UI. Backgrounds utilize a subtle off-white to reduce eye strain and feel more like premium cardstock.

Status colors (Success, Error, Warning) should be desaturated to maintain the sophisticated aesthetic, ensuring they do not clash with the core brand palette.

## Typography

The typography strategy relies on the tension between the high-contrast, editorial **Bodoni Moda** and the technical, clean **Manrope**.

*   **Serif (Bodoni Moda):** Use for property titles, hero sections, and editorial quotes. It conveys heritage and luxury.
*   **Sans-Serif (Manrope):** Use for all functional UI elements, property details, and body copy. Its modern proportions ensure high legibility at small sizes.
*   **Labels:** All small labels and "caps" should use Manrope with increased letter spacing to maintain a clean, organized appearance in dense data areas like property specifications.

## Layout & Spacing

The layout philosophy is based on a **Fixed Grid with Generous Margins**. To convey luxury, we avoid crowding elements.

*   **Desktop:** 12-column grid with a maximum content width of 1440px. Side margins are intentionally wide (64px) to center the focus.
*   **Mobile:** 4-column grid with 20px margins. 
*   **Rhythm:** Use an 8px base unit. Vertical rhythm should favor larger gaps (stack-lg) between distinct sections to create a "gallery" feel as the user scrolls.
*   **Whitespace:** Use whitespace as a functional element to group related information rather than relying on heavy borders or dividers.

## Elevation & Depth

Hierarchy is achieved through **Tonal Layering and Ambient Shadows**.

*   **Surfaces:** The base background is `Neutral`. Floating elements like cards use pure white.
*   **Shadows:** Shadows are extremely soft and desaturated. Use a large blur radius (20px-40px) with very low opacity (4-8%) to make elements appear to lift gently off the page. Avoid harsh shadows or "black" tints; use a shadow color derived from the `Primary` charcoal.
*   **Depth:** Only three levels of elevation are permitted:
    1.  **Level 0 (Base):** Main background.
    2.  **Level 1 (Card):** Property cards and filter bars.
    3.  **Level 2 (Overlay):** Modals, dropdown menus, and navigation headers.

## Shapes

The shape language is refined and geometric. We avoid overly "bubbly" aesthetics in favor of structured elegance.

*   **Corner Radii:** A consistent 8px (`rounded`) is the default for buttons, input fields, and small UI components. Large property cards and image containers use 16px (`rounded-xl`) to soften the visual impact of high-resolution photography.
*   **Interactive Elements:** Buttons maintain a structured, rectangular feel with the same 8px radius, never fully pill-shaped, to keep the professional tone.

## Components

*   **Buttons:** Primary buttons are solid `Primary (Charcoal)` with white text. Secondary buttons use a fine 1px border. "Ghost" buttons for tertiary actions use the `Secondary (Gold)` color for text.
*   **Input Fields:** Minimalist design with a bottom-border only or a very light 4-sided border in a light grey. Focused states use a transition to the `Secondary (Gold)` color.
*   **Cards:** Property cards are the centerpiece. They should feature full-bleed imagery at the top with a subtle 1px internal border. Information (price, location) is typeset with generous padding (24px).
*   **Chips/Badges:** Small, subtle tags for property features (e.g., "Pool", "Helipad"). Use a light gray background with `Label-MD` typography.
*   **Navigation:** A sticky top header with high transparency and a backdrop-blur (glassmorphism) effect to maintain context while scrolling through high-impact imagery.
*   **Floor Plan Viewer:** A specialized component using high-contrast line work and `Tertiary (Navy)` accents for interactive zones.