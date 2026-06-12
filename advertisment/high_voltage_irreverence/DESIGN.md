---
name: High-Voltage Irreverence
colors:
  surface: '#131313'
  surface-dim: '#131313'
  surface-bright: '#3a3939'
  surface-container-lowest: '#0e0e0e'
  surface-container-low: '#1c1b1b'
  surface-container: '#201f1f'
  surface-container-high: '#2a2a2a'
  surface-container-highest: '#353534'
  on-surface: '#e5e2e1'
  on-surface-variant: '#c4c9ac'
  inverse-surface: '#e5e2e1'
  inverse-on-surface: '#313030'
  outline: '#8e9379'
  outline-variant: '#444933'
  surface-tint: '#abd600'
  primary: '#ffffff'
  on-primary: '#283500'
  primary-container: '#c3f400'
  on-primary-container: '#556d00'
  inverse-primary: '#506600'
  secondary: '#c8c6c5'
  on-secondary: '#313030'
  secondary-container: '#474746'
  on-secondary-container: '#b7b5b4'
  tertiary: '#ffffff'
  on-tertiary: '#2f3131'
  tertiary-container: '#e2e2e2'
  on-tertiary-container: '#636565'
  error: '#ffb4ab'
  on-error: '#690005'
  error-container: '#93000a'
  on-error-container: '#ffdad6'
  primary-fixed: '#c3f400'
  primary-fixed-dim: '#abd600'
  on-primary-fixed: '#161e00'
  on-primary-fixed-variant: '#3c4d00'
  secondary-fixed: '#e5e2e1'
  secondary-fixed-dim: '#c8c6c5'
  on-secondary-fixed: '#1c1b1b'
  on-secondary-fixed-variant: '#474746'
  tertiary-fixed: '#e2e2e2'
  tertiary-fixed-dim: '#c6c6c7'
  on-tertiary-fixed: '#1a1c1c'
  on-tertiary-fixed-variant: '#454747'
  background: '#131313'
  on-background: '#e5e2e1'
  surface-variant: '#353534'
typography:
  display-lg:
    fontFamily: Anton
    fontSize: 96px
    fontWeight: '400'
    lineHeight: 100%
    letterSpacing: -0.02em
  headline-lg:
    fontFamily: Anton
    fontSize: 64px
    fontWeight: '400'
    lineHeight: 110%
  headline-lg-mobile:
    fontFamily: Anton
    fontSize: 48px
    fontWeight: '400'
    lineHeight: 110%
  subheader:
    fontFamily: Syne
    fontSize: 24px
    fontWeight: '800'
    lineHeight: 120%
  body-lg:
    fontFamily: Geist
    fontSize: 18px
    fontWeight: '400'
    lineHeight: 160%
  body-sm:
    fontFamily: Geist
    fontSize: 14px
    fontWeight: '400'
    lineHeight: 150%
  label-caps:
    fontFamily: Syne
    fontSize: 12px
    fontWeight: '700'
    lineHeight: 100%
    letterSpacing: 0.1em
spacing:
  base: 4px
  xs: 8px
  sm: 16px
  md: 24px
  lg: 48px
  xl: 80px
  gutter: 20px
  margin-mobile: 16px
  margin-desktop: 64px
---

## Brand & Style
The design system is engineered to capture the raw energy of late-night productivity and digital subcultures. It targets a demographic that thrives after dark—gamers, creators, and night-owls—who demand a brand that speaks with volume and wit. 

The aesthetic is rooted in **Neo-Brutalism**, characterized by high-contrast interfaces, unapologetic typography, and a "sticker-bomb" digital ethos. We avoid the polished, sterile look of traditional tech in favor of something that feels alive, slightly chaotic, and undeniably bold. The visual language uses heavy strokes and flat planes to create a sense of tactile urgency, mirroring the immediate "kick" of the beverage.

## Colors
The palette is built on extreme contrast to ensure legibility under low-light conditions and to demand attention in crowded digital feeds.

- **Primary (Electric Lime):** This is the high-voltage core of the brand. It is used for calls to action, critical highlights, and brand moments that need to "pop" off the screen.
- **Secondary (Deep Charcoal):** Our primary background color. It provides a deep, matte canvas that allows the Electric Lime to vibrate visually.
- **Tertiary (High-Contrast White):** Used primarily for body text and punchy secondary accents to maintain a clean, readable hierarchy.
- **Semantic Accents:** Functional colors (Success/Error) should be heavily saturated to match the intensity of the primary palette.

## Typography
Typography is the primary voice of the design system. It is loud, condensed, and authoritative.

- **Headlines:** We use **Anton** for its aggressive, condensed presence. It should almost always be displayed in uppercase to reinforce the "Conquer" persona.
- **Secondary Display:** **Syne** is utilized for subheaders and distinctive labels. Its wider, expressive character provides a counterweight to the narrowness of Anton.
- **Body Copy:** **Geist** provides a technical, mono-inspired clarity that appeals to a tech-savvy audience. It keeps the irreverent tone grounded in professional legibility.

## Layout & Spacing
The layout follows a **Rigid Grid** philosophy. We use a 12-column system for desktop and a 4-column system for mobile. 

Spacing is intentional and "boxy." Avoid fluid, airy transitions; instead, use hard dividers and clear-cut sections. Elements should feel like they are locked into a grid, utilizing a 4px baseline rhythm. Gutters are kept tight to maintain a high-density, high-energy feel. Large "hero" sections should use the `xl` spacing to create moments of impact between dense information blocks.

## Elevation & Depth
This design system rejects soft shadows and ambient blurs. Depth is achieved through **Hard Offsets** and **Stark Layers**.

- **Hard Shadows:** Use solid, 100% opacity black offsets (usually 4px or 8px) to lift elements like buttons and cards. This creates a "pop-out" effect common in comic books and street art.
- **Tonal Layering:** The primary background is the deepest layer. Secondary containers use a slightly lighter charcoal to indicate grouping.
- **High-Contrast Outlines:** Every container and interactive element must have a defined border (2px minimum). Use the Primary color for active states and White for inactive states.

## Shapes
The shape language is strictly **Sharp (0)**. There are no rounded corners in the design system. This reinforces the aggressive, "no-nonsense" brand identity. All buttons, input fields, cards, and images must feature 90-degree angles. This geometric rigidity contrasts with the fluid, irreverent copywriting to create a unique tension in the UI.

## Components
- **Buttons:** Large-scale, rectangular blocks with a 2px black border and a 4px hard shadow. The "hover" state should involve the shadow disappearing as the button "depresses" (translates XY by 4px).
- **Cards:** Use a thick 2px white border against the deep charcoal background. Include a "tag" in the top-right corner using the `label-caps` typography style.
- **Input Fields:** High-contrast white backgrounds with black text for maximum focus. The focus state should trigger a thick Electric Lime border.
- **Chips/Badges:** Small, sharp-edged rectangles with `label-caps` text. Use these for flavor profiles or "Late Night" status indicators.
- **Lists:** Separated by 2px solid dividers. Use the Electric Lime as a bullet point or icon accent.
- **Stickers:** A unique component for this design system—non-interactive graphic elements (funny quotes, "Conquer" seals) that can be rotated at slight angles (3-5 degrees) to break the grid and add humor.