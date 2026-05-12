---
name: High-Energy Event Discovery
colors:
  surface: '#f8f9ff'
  surface-dim: '#d0dbed'
  surface-bright: '#f8f9ff'
  surface-container-lowest: '#ffffff'
  surface-container-low: '#eff4ff'
  surface-container: '#e6eeff'
  surface-container-high: '#dee9fc'
  surface-container-highest: '#d9e3f6'
  on-surface: '#121c2a'
  on-surface-variant: '#464554'
  inverse-surface: '#27313f'
  inverse-on-surface: '#eaf1ff'
  outline: '#767586'
  outline-variant: '#c7c4d7'
  surface-tint: '#494bd6'
  primary: '#4648d4'
  on-primary: '#ffffff'
  primary-container: '#6063ee'
  on-primary-container: '#fffbff'
  inverse-primary: '#c0c1ff'
  secondary: '#006b5f'
  on-secondary: '#ffffff'
  secondary-container: '#6df5e1'
  on-secondary-container: '#006f64'
  tertiary: '#a63047'
  on-tertiary: '#ffffff'
  tertiary-container: '#c6495e'
  on-tertiary-container: '#fffbff'
  error: '#ba1a1a'
  on-error: '#ffffff'
  error-container: '#ffdad6'
  on-error-container: '#93000a'
  primary-fixed: '#e1e0ff'
  primary-fixed-dim: '#c0c1ff'
  on-primary-fixed: '#07006c'
  on-primary-fixed-variant: '#2f2ebe'
  secondary-fixed: '#71f8e4'
  secondary-fixed-dim: '#4fdbc8'
  on-secondary-fixed: '#00201c'
  on-secondary-fixed-variant: '#005048'
  tertiary-fixed: '#ffdadc'
  tertiary-fixed-dim: '#ffb2b9'
  on-tertiary-fixed: '#400010'
  on-tertiary-fixed-variant: '#891933'
  background: '#f8f9ff'
  on-background: '#121c2a'
  surface-variant: '#d9e3f6'
typography:
  display-lg:
    fontFamily: Montserrat
    fontSize: 48px
    fontWeight: '800'
    lineHeight: '1.1'
    letterSpacing: -0.02em
  display-lg-mobile:
    fontFamily: Montserrat
    fontSize: 36px
    fontWeight: '800'
    lineHeight: '1.1'
  headline-md:
    fontFamily: Montserrat
    fontSize: 30px
    fontWeight: '700'
    lineHeight: '1.2'
  headline-sm:
    fontFamily: Montserrat
    fontSize: 24px
    fontWeight: '700'
    lineHeight: '1.2'
  body-lg:
    fontFamily: Inter
    fontSize: 18px
    fontWeight: '400'
    lineHeight: '1.6'
  body-md:
    fontFamily: Inter
    fontSize: 16px
    fontWeight: '400'
    lineHeight: '1.5'
  label-caps:
    fontFamily: Inter
    fontSize: 12px
    fontWeight: '700'
    lineHeight: '1'
    letterSpacing: 0.05em
  data-point:
    fontFamily: Inter
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
  container-max: 1280px
  gutter: 1.5rem
  margin-mobile: 1rem
  margin-desktop: 2.5rem
  stack-sm: 0.5rem
  stack-md: 1rem
  stack-lg: 2rem
---

## Brand & Style

This design system is built for a high-energy, social audience that thrives on discovery and connection. The brand personality is **dynamic, inviting, and urban**, striking a balance between a high-end editorial feel and a vibrant social feed.

The visual style leverages **Modern Glassmorphism** and **High-Contrast Bold** aesthetics. We use depth and translucency to create a sense of layering, mirroring the layered experiences of city life. The UI should never feel static; it utilizes subtle gradients and layered surfaces to suggest movement and momentum. Photography is the hero, treated with immersive treatments to ensure text legibility while maintaining a high-energy "vibe."

## Colors

The palette is anchored by **Electric Indigo**, a high-vibrancy hue reserved for primary actions, active states, and brand moments. 

- **Primary (Electric Indigo):** Used for CTA buttons, progress indicators, and primary navigation links.
- **Secondary (Teal - #14B8A6):** Dedicated to "Outdoor," "Tech," or "Professional" event categories.
- **Tertiary (Coral - #FB7185):** Dedicated to "Music," "Nightlife," or "Social" event categories.
- **Neutral (Deep Charcoal):** Specifically used for typography and high-contrast borders to ground the vibrant accents.
- **Surface:** We use a "Soft White" (#FAFAFA) for the background to allow card shadows and glass effects to pop without feeling clinical.

## Typography

The typography system pairs the geometric strength of **Montserrat** for headlines with the functional precision of **Inter** for body copy. 

Headlines should use tight tracking and bold weights to communicate energy. Body text prioritizes readability with generous line heights. For critical event metadata like "Date" and "Location," we use the `data-point` style to ensure these details are scannable at a glance. All labels should be uppercase with slight letter spacing to differentiate them from interactive text.

## Layout & Spacing

This design system utilizes a **12-column fluid grid** for desktop and a **single-column stack** for mobile. 

- **Desktop:** 12 columns with 24px gutters. Content is centered with a max-width of 1280px.
- **Mobile:** 16px side margins. Cards should span the full width of the viewport minus margins to maximize photography impact.
- **Spacing Logic:** We use an 8px base grid. Vertically, elements are grouped using `stack` units. Related information (e.g., event title and date) uses `stack-sm`, while distinct sections use `stack-lg`.

## Elevation & Depth

We create hierarchy using **Ambient Shadows** and **Tonal Layering**. 

1.  **Level 0 (Base):** The main background (#FAFAFA).
2.  **Level 1 (Cards):** Pure white background with a "Soft Glow" shadow: `0px 10px 30px rgba(99, 102, 241, 0.08)`. Note the subtle Indigo tint in the shadow to tie it to the brand color.
3.  **Level 2 (Floating/Interactive):** Active cards or dropdowns use a more pronounced shadow: `0px 20px 40px rgba(0, 0, 0, 0.12)`.
4.  **Glass Layer:** Overlays (like price tags on images) use a backdrop-blur (12px) with a 70% white opacity to maintain legibility without obscuring the photography.

## Shapes

The shape language is **Rounded**, conveying a friendly and modern social feel. 

- **Standard Buttons & Inputs:** 8px (0.5rem) corner radius.
- **Event Cards:** 16px (1rem) corner radius to feel substantial and modern.
- **Category Chips:** Fully pill-shaped (rounded-full) to distinguish them from actionable buttons.
- **Media:** Images within cards should inherit the card's top-level radius but remain sharp on interior edges where they meet text containers.

## Components

- **Primary Buttons:** Solid Electric Indigo with white text. On hover, apply a slight upward translate (-2px) and deepen the shadow.
- **Event Cards:** The core component. Top 60% is a high-quality image with a gradient overlay (black to transparent) at the bottom to host white text for the event title. The bottom 40% is a white container for the date, location, and "Join" CTA.
- **Category Chips:** Use a light tint of the category color (Teal or Coral) for the background (10% opacity) and the full-strength color for the text.
- **Search Inputs:** Large, 16px rounded fields with soft shadows and a prominent Indigo search icon.
- **Interactive Avatars:** For social proof, use overlapping avatar stacks ("+5 friends going") with 2px white borders between each face.
- **Date Badges:** Placed in the top-left corner of event images, using a glassmorphic square with centered, bold Montserrat text.