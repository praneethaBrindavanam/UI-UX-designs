---
name: Aura
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
  on-surface-variant: '#cbc4cd'
  inverse-surface: '#e2e2e2'
  inverse-on-surface: '#2f3131'
  outline: '#958f97'
  outline-variant: '#49454c'
  surface-tint: '#d1c0e2'
  primary: '#d1c0e2'
  on-primary: '#372b46'
  primary-container: '#0f051d'
  on-primary-container: '#827392'
  inverse-primary: '#665976'
  secondary: '#e6feff'
  on-secondary: '#003739'
  secondary-container: '#00f4fe'
  on-secondary-container: '#006c71'
  tertiary: '#ecb1ff'
  on-tertiary: '#520070'
  tertiary-container: '#170022'
  on-tertiary-container: '#c118ff'
  error: '#ffb4ab'
  on-error: '#690005'
  error-container: '#93000a'
  on-error-container: '#ffdad6'
  primary-fixed: '#eedcff'
  primary-fixed-dim: '#d1c0e2'
  on-primary-fixed: '#211630'
  on-primary-fixed-variant: '#4e415d'
  secondary-fixed: '#63f7ff'
  secondary-fixed-dim: '#00dce5'
  on-secondary-fixed: '#002021'
  on-secondary-fixed-variant: '#004f53'
  tertiary-fixed: '#f9d8ff'
  tertiary-fixed-dim: '#ecb1ff'
  on-tertiary-fixed: '#320046'
  on-tertiary-fixed-variant: '#75009e'
  background: '#121414'
  on-background: '#e2e2e2'
  surface-variant: '#333535'
typography:
  display-lg:
    fontFamily: Syne
    fontSize: 48px
    fontWeight: '800'
    lineHeight: 56px
    letterSpacing: -0.02em
  display-lg-mobile:
    fontFamily: Syne
    fontSize: 36px
    fontWeight: '800'
    lineHeight: 42px
    letterSpacing: -0.02em
  headline-md:
    fontFamily: Syne
    fontSize: 32px
    fontWeight: '700'
    lineHeight: 40px
  headline-sm:
    fontFamily: Syne
    fontSize: 24px
    fontWeight: '700'
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
  label-md:
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
  sm: 0.5rem
  DEFAULT: 1rem
  md: 1.5rem
  lg: 2rem
  xl: 3rem
  full: 9999px
spacing:
  unit: 8px
  container-margin-desktop: 80px
  container-margin-mobile: 24px
  gutter: 24px
  card-gap: 24px
---

## Brand & Style

The design system embodies a "Modern Noir" aesthetic—a sophisticated, futuristic vision of the smart home. It targets high-end users who value privacy, precision, and a premium atmosphere. The interface should feel like a digital extension of a luxurious, contemporary living space.

The style is defined by **Dark Glassmorphism**. It utilizes deep, immersive backgrounds punctuated by translucent UI surfaces that mimic frosted glass. This creates a sense of physical depth and spatial awareness within the application. The emotional response is one of calm, effortless control and technological mastery.

Key principles:
- **Immersive Depth:** Use layers of transparency and blur to create a multi-dimensional environment.
- **Atmospheric Lighting:** UI elements should emit subtle glows, suggesting they are light sources within a dark room.
- **Precision:** Every border and alignment must be sharp and intentional to maintain a high-end, engineered feel.

## Colors

The palette is rooted in the "Deep Space Violet" primary color, providing a vast, cinematic canvas. Contrast is achieved through high-energy accents that represent active states and connectivity.

- **Deep Space Violet (#0F051D):** The foundation. Used for the base background and deep shadows.
- **Electric Cyan (#00F5FF):** Functional secondary color. Used for active home states, "on" switches, and temperature cooling.
- **Neon Orchid (#BF00FF):** Aesthetic accent. Used for branding moments, smart scenes, and temperature heating.
- **Glass Surface (#FFFFFF10):** The primary material for cards and navigation bars, always paired with a 20px to 40px backdrop blur.
- **Borders:** Use a 1px solid stroke of `#FFFFFF15` on the top and left edges of glass elements to simulate a light-catching "edge" effect.

## Typography

This design system utilizes a high-contrast typographic pairing to balance futuristic character with utility.

- **Syne:** Used for all display and headline roles. Its unique, wide geometry provides the "futuristic" signature. Use the Extra Bold weight for display text to command attention.
- **Inter:** Used for all functional text, data readouts, and body copy. Inter’s neutrality ensures that complex home data remains legible even against blurred glass backgrounds.

**Styling Note:** Use `label-md` for navigation items and section headers. The uppercase styling with increased letter spacing adds a technical, "HUD" (Heads-Up Display) quality to the UI.

## Layout & Spacing

The layout philosophy follows a **Fluid Grid** model with generous safe areas to maintain a premium, uncluttered feel.

- **Grid:** A 12-column grid for desktop and a 4-column grid for mobile.
- **Rhythm:** All spacing is derived from an 8px base unit. 
- **Margins:** Desktop layouts utilize wide 80px side margins to center the focus on the "Home Dashboard" glass panels. Mobile layouts use a 24px margin to allow glass elements to feel expansive.
- **Padding:** Internal card padding should be a minimum of 24px to ensure touch targets for smart controls are easily accessible.

## Elevation & Depth

Depth is not communicated through traditional grey shadows, but through **Backdrop Blurs and Glows**.

- **Surface Layers:**
  - Base: Deep Space Violet background.
  - Level 1: Glass containers with 30px Backdrop Blur.
  - Level 2: Overlays (Modals/Pop-outs) with 60px Backdrop Blur and a more prominent white border.
- **Glows:** Instead of drop shadows, active elements (like a light being "on") should use an outer glow using the `secondary` or `tertiary` color with a 20% opacity and 15px-30px blur.
- **The "Light Edge":** Apply a 1px inner stroke to the top-left of containers to create a "specular highlight," making the glass feel physical and polished.

## Shapes

The shape language is ultra-soft and organic to counteract the "coldness" of the dark theme.

- **Containers:** All primary cards and glass panels use a `24px` (1.5rem) radius.
- **Interactive Elements:** Buttons and toggles use pill-shapes (fully rounded) to maximize the tactile, "squishy" feel mentioned in the brand vision.
- **Icons:** Use 3D rendered icons with soft edges or photorealistic elements with slightly rounded corners to match the UI's geometry.

## Components

### Buttons
- **Primary:** Pill-shaped, background is a gradient from Electric Cyan to Neon Orchid. Text is black for high contrast.
- **Secondary (Glass):** Pill-shaped, glass background (`#FFFFFF20`), 1px white border.

### Smart Cards
- Large `24px` rounded containers. 
- State change: When a device is "On," the border color changes to Electric Cyan and a subtle glow is applied to the background of the card.

### Input Fields
- Underlined style or ghost-input style with a very subtle glass bottom border. 
- Focus state: The border glows Electric Cyan.

### Toggles / Switches
- Large, tactile "pill" switches. 
- The "thumb" of the switch should have a soft 3D gradient to look like a physical glass or metallic bead.

### Glass Lists
- Vertical lists where each item is separated by a 1px glass line (`#FFFFFF10`). 
- Selection state: A soft violet glow behind the text.

### Additional Components
- **Radial Controller:** For temperature or light brightness, use a large circular glass dial with a glowing "handle" that follows the perimeter.
- **Status Chips:** Small, semi-transparent pill labels used for "Eco Mode" or "Security Armed" indicators.