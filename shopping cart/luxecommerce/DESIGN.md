---
name: LuxeCommerce
colors:
  surface: '#f9f9ff'
  surface-dim: '#d3daef'
  surface-bright: '#f9f9ff'
  surface-container-lowest: '#ffffff'
  surface-container-low: '#f1f3ff'
  surface-container: '#e9edff'
  surface-container-high: '#e1e8fd'
  surface-container-highest: '#dce2f7'
  on-surface: '#141b2b'
  on-surface-variant: '#404944'
  inverse-surface: '#293040'
  inverse-on-surface: '#edf0ff'
  outline: '#707974'
  outline-variant: '#bfc9c3'
  surface-tint: '#2b6954'
  primary: '#003527'
  on-primary: '#ffffff'
  primary-container: '#064e3b'
  on-primary-container: '#80bea6'
  inverse-primary: '#95d3ba'
  secondary: '#006c49'
  on-secondary: '#ffffff'
  secondary-container: '#6cf8bb'
  on-secondary-container: '#00714d'
  tertiary: '#25312b'
  on-tertiary: '#ffffff'
  tertiary-container: '#3b4741'
  on-tertiary-container: '#a8b5ad'
  error: '#ba1a1a'
  on-error: '#ffffff'
  error-container: '#ffdad6'
  on-error-container: '#93000a'
  primary-fixed: '#b0f0d6'
  primary-fixed-dim: '#95d3ba'
  on-primary-fixed: '#002117'
  on-primary-fixed-variant: '#0b513d'
  secondary-fixed: '#6ffbbe'
  secondary-fixed-dim: '#4edea3'
  on-secondary-fixed: '#002113'
  on-secondary-fixed-variant: '#005236'
  tertiary-fixed: '#d9e6dd'
  tertiary-fixed-dim: '#bdcac1'
  on-tertiary-fixed: '#131e19'
  on-tertiary-fixed-variant: '#3e4943'
  background: '#f9f9ff'
  on-background: '#141b2b'
  surface-variant: '#dce2f7'
typography:
  display:
    fontFamily: Manrope
    fontSize: 48px
    fontWeight: '800'
    lineHeight: '1.2'
    letterSpacing: -0.02em
  h1:
    fontFamily: Manrope
    fontSize: 32px
    fontWeight: '700'
    lineHeight: '1.2'
  h2:
    fontFamily: Manrope
    fontSize: 24px
    fontWeight: '700'
    lineHeight: '1.3'
  h3:
    fontFamily: Manrope
    fontSize: 20px
    fontWeight: '600'
    lineHeight: '1.4'
  body-lg:
    fontFamily: Manrope
    fontSize: 18px
    fontWeight: '400'
    lineHeight: '1.6'
  body-md:
    fontFamily: Manrope
    fontSize: 16px
    fontWeight: '400'
    lineHeight: '1.6'
  price-lg:
    fontFamily: Manrope
    fontSize: 24px
    fontWeight: '700'
    lineHeight: '1'
    letterSpacing: -0.01em
  label-sm:
    fontFamily: Manrope
    fontSize: 14px
    fontWeight: '600'
    lineHeight: '1'
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
  margin: 32px
---

## Brand & Style

The design system is anchored in a philosophy of "Essentialist Luxury." It targets a discerning consumer who values clarity, efficiency, and premium quality. The aesthetic is a fusion of **Minimalism** and **Modern Corporate** styles, prioritizing high-ratio white space to allow product photography to breathe. 

By removing unnecessary visual noise, the design system cultivates an environment of trust and sophistication. Every interaction should feel intentional and effortless, evoking a sense of calm reliability throughout the purchasing journey.

## Colors

The palette is centered around a deep, authoritative **Emerald Green** as the primary brand color, signaling growth, stability, and premium value. 

- **Primary:** Used for key actions, brand touchpoints, and high-level headings.
- **Secondary:** A lighter mint green used for accents, success states, and subtle highlights.
- **Neutral:** A range of cool-toned grays from nearly black (#111827) for text to soft off-whites for background layering.
- **Surface:** High-use of pure white (#FFFFFF) to maintain the clean aesthetic and provide maximum contrast for product imagery.

## Typography

This design system utilizes **Manrope** for its balanced, modern, and highly legible geometric qualities. Typography is the primary driver of hierarchy.

- **Pricing:** Always rendered in semi-bold or bold weights with tighter letter-spacing to ensure the value is the first thing a user perceives.
- **Product Details:** Use `body-md` for descriptions to ensure high readability.
- **Labels:** Use `label-sm` with increased letter-spacing for metadata and micro-copy to maintain an organized, systematic look.

## Layout & Spacing

The design system employs a **Fixed Grid** model for desktop (12 columns, 1200px max-width) and a **Fluid Grid** for mobile. 

A strict 8px spacing rhythm ensures consistency across all components. Large "Macro-spacing" (`xl`) is used between major page sections to reinforce the clean aesthetic, while "Micro-spacing" (`xs`, `sm`) is reserved for internal component logic, such as the gap between a product title and its price. Gutters are kept wide to prevent the UI from feeling cramped.

## Elevation & Depth

Hierarchy is established through **Ambient Shadows** and **Tonal Layering**. 

- **Level 0 (Base):** Pure white or light gray backgrounds.
- **Level 1 (Cards):** Soft, highly-diffused shadows (Y: 4px, Blur: 20px, 5% opacity) to lift product cards and cart items off the base.
- **Level 2 (Overlays):** Used for cart drawers and modals, featuring a slightly deeper shadow and a backdrop blur (12px) to maintain context while focusing user attention.
- **Interactive:** Elements should subtly "lift" (increase shadow depth) on hover to provide tactile feedback.

## Shapes

The shape language is defined as **Rounded**, utilizing a medium corner radius that balances approachability with professional structure.

- **Standard Elements:** Buttons, input fields, and small cards use a `0.5rem` (8px) radius.
- **Large Elements:** Product containers and featured banners use a `1rem` (16px) radius.
- **Quantity Selectors:** Should mirror the button radius to maintain a unified visual language.

## Components

### Buttons
The **Checkout Button** is the most prominent element. It uses the Primary Deep Emerald color, white text, and a minimum height of 56px for high tap-target accessibility. It should span the full width of the container in the cart view.

### Cart Items
Cart items are styled as horizontal cards with a subtle bottom border or soft shadow. They must prioritize the product thumbnail (left-aligned) followed by the title and price. The "Remove" action should be an icon-only button or subtle text link to avoid clutter.

### Quantity Selector
A clean, segmented control. It consists of a light gray container with a "minus" icon, the current numeric value in the center, and a "plus" icon. The background should be a subtle neutral tint to distinguish it from the pure white background of the cart item.

### Input Fields
Clean, outlined boxes with a 1px border in a medium-gray. Labels sit above the field in `label-sm`. Focus states use a 2px Primary Emerald border to signal active interaction clearly.

### Product Cards
Minimalist containers with ample padding. The image is the hero, followed by a left-aligned title in `h3` and the price in `price-lg`. Icons for "Add to Wishlist" should be placed in the top right corner of the image area using a semi-transparent circular background.