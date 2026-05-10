---
name: Modern Sky
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
  on-surface-variant: '#44474d'
  inverse-surface: '#2d3133'
  inverse-on-surface: '#eff1f3'
  outline: '#75777e'
  outline-variant: '#c5c6ce'
  surface-tint: '#4e5f7e'
  primary: '#031632'
  on-primary: '#ffffff'
  primary-container: '#1a2b48'
  on-primary-container: '#8293b5'
  inverse-primary: '#b6c7eb'
  secondary: '#00658d'
  on-secondary: '#ffffff'
  secondary-container: '#2dbcfe'
  on-secondary-container: '#004866'
  tertiary: '#370005'
  on-tertiary: '#ffffff'
  tertiary-container: '#5e000e'
  on-tertiary-container: '#fd595e'
  error: '#ba1a1a'
  on-error: '#ffffff'
  error-container: '#ffdad6'
  on-error-container: '#93000a'
  primary-fixed: '#d7e2ff'
  primary-fixed-dim: '#b6c7eb'
  on-primary-fixed: '#081b38'
  on-primary-fixed-variant: '#374765'
  secondary-fixed: '#c6e7ff'
  secondary-fixed-dim: '#82cfff'
  on-secondary-fixed: '#001e2d'
  on-secondary-fixed-variant: '#004c6b'
  tertiary-fixed: '#ffdad8'
  tertiary-fixed-dim: '#ffb3b0'
  on-tertiary-fixed: '#410007'
  on-tertiary-fixed-variant: '#92001b'
  background: '#f7f9fb'
  on-background: '#191c1e'
  surface-variant: '#e0e3e5'
typography:
  display-lg:
    fontFamily: Hanken Grotesk
    fontSize: 32px
    fontWeight: '700'
    lineHeight: 40px
    letterSpacing: -0.02em
  headline-md:
    fontFamily: Hanken Grotesk
    fontSize: 24px
    fontWeight: '600'
    lineHeight: 32px
  title-lg:
    fontFamily: Hanken Grotesk
    fontSize: 20px
    fontWeight: '600'
    lineHeight: 28px
  body-lg:
    fontFamily: Hanken Grotesk
    fontSize: 16px
    fontWeight: '400'
    lineHeight: 24px
  body-md:
    fontFamily: Hanken Grotesk
    fontSize: 14px
    fontWeight: '400'
    lineHeight: 20px
  price-display:
    fontFamily: Hanken Grotesk
    fontSize: 18px
    fontWeight: '700'
    lineHeight: 24px
    letterSpacing: 0.01em
  label-sm:
    fontFamily: Hanken Grotesk
    fontSize: 12px
    fontWeight: '500'
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
  base: 4px
  xs: 4px
  sm: 8px
  md: 16px
  lg: 24px
  xl: 32px
  container-margin: 20px
  gutter: 12px
---

## Brand & Style
The brand personality centers on the "Modern Sky" concept: a fusion of professional reliability and the airy, expansive feeling of aviation. It targets frequent travelers and business professionals who value efficiency without sacrificing aesthetic clarity. 

The design style is **Corporate / Modern** with a strong emphasis on whitespace and high-legibility data visualization. It avoids clutter by utilizing tonal separation and subtle depth, ensuring that complex flight information feels light and manageable. The emotional response should be one of "calm control"—the user feels the trustworthiness of an established carrier paired with the technological speed of a modern startup.

## Colors
The palette is rooted in **Deep Navy (#1A2B48)**, used for primary branding, headings, and essential UI containers to establish a foundation of trust. **Bright Sky Blue (#00AEEF)** serves as the functional secondary color, reserved for primary call-to-actions, selection states, and interactive icons. 

**High-Contrast Coral (#FF5A5F)** is applied surgically for pricing, urgent alerts, and promotional tags to ensure they pop against the cooler backdrop. Backgrounds are strictly **White (#FFFFFF)** or **Very Light Gray (#F8FAFC)** to maintain a crisp, airy environment that mimics the clarity of a high-altitude sky.

## Typography
This design system utilizes **Hanken Grotesk** for its sharp, contemporary geometry and exceptional legibility in data-dense environments. 

The hierarchy prioritizes the "price-display" and "title-lg" levels to ensure that flight costs and airport codes are the first elements a user identifies. High-contrast weights are used between flight times (Bold) and durations (Medium/Regular) to prevent visual fatigue during search results browsing. Label styles use slight letter spacing and uppercase transforms to differentiate metadata from primary content.

## Layout & Spacing
The design system employs a **Fluid Grid** model optimized for mobile-first interactions. It follows a 4px baseline shift to ensure all elements align to a consistent vertical rhythm. 

A standard 4-column grid is used for mobile displays with 20px outer margins and 12px gutters. For flight search results, horizontal whitespace is maximized to prevent the "dense table" look; padding within flight cards is generous (16px), ensuring touch targets for selecting flights are clear and accessible. Layouts should utilize "Airy Padding" where content-heavy sections are separated by at least 24px (lg) of white space.

## Elevation & Depth
Hierarchy is established through **Ambient Shadows** and **Tonal Layers**. 

The base background is White, while interactive cards (like flight results) use a 1px border in a very light neutral tint and a soft, diffused shadow (0px 4px 20px rgba(26, 43, 72, 0.05)). This creates a "floating" effect that suggests light and air. Modal overlays and bottom sheets utilize a higher elevation with a more pronounced blur to focus user attention. Interactive states for buttons should subtly increase shadow depth upon hover or tap to provide tactile feedback.

## Shapes
The shape language follows a **Rounded** philosophy. UI elements like buttons, input fields, and cards utilize a base radius of 8px to 12px. 

This specific range is chosen to strike a balance between the "friendly" nature of travel and the "professional" precision of aviation. Secondary elements like chips and tags for "Fastest" or "Cheapest" flights should use a fully rounded (pill) shape to distinguish them from structural data containers. Progress bars and icons should maintain consistent rounded terminals to match the container radius.

## Components

### Buttons
Primary buttons use the Bright Sky Blue background with white text and 8px corners. Secondary buttons use a Deep Navy outline with a transparent fill.

### Cards
Flight cards are the core component. They must feature a white background, the 0.05 opacity navy shadow, and internal 16px padding. Use the Coral color exclusively for the price component within the card.

### Chips
Used for filtering (e.g., "1 Stop," "Airline"). They feature a light gray background in their inactive state and transition to Sky Blue with white text when selected.

### Input Fields
Search inputs for "Origin" and "Destination" should be large (min-height 56px), with a subtle 1px border. Focus states should highlight the border in Sky Blue.

### Flight Timeline
A custom vertical or horizontal line component using the Deep Navy for terminal points and a dashed line for the flight path, representing the journey visually.

### Alerts & Modals
Emergency or price-drop alerts use a soft Coral tint background with high-contrast Coral text to ensure immediate visibility without being jarring.