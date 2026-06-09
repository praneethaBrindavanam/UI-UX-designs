---
name: Lumina Modern
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
  on-surface-variant: '#464555'
  inverse-surface: '#2e3132'
  inverse-on-surface: '#f0f1f2'
  outline: '#777587'
  outline-variant: '#c7c4d8'
  surface-tint: '#4d44e3'
  primary: '#3525cd'
  on-primary: '#ffffff'
  primary-container: '#4f46e5'
  on-primary-container: '#dad7ff'
  inverse-primary: '#c3c0ff'
  secondary: '#006c49'
  on-secondary: '#ffffff'
  secondary-container: '#6cf8bb'
  on-secondary-container: '#00714d'
  tertiary: '#7e3000'
  on-tertiary: '#ffffff'
  tertiary-container: '#a44100'
  on-tertiary-container: '#ffd2be'
  error: '#ba1a1a'
  on-error: '#ffffff'
  error-container: '#ffdad6'
  on-error-container: '#93000a'
  primary-fixed: '#e2dfff'
  primary-fixed-dim: '#c3c0ff'
  on-primary-fixed: '#0f0069'
  on-primary-fixed-variant: '#3323cc'
  secondary-fixed: '#6ffbbe'
  secondary-fixed-dim: '#4edea3'
  on-secondary-fixed: '#002113'
  on-secondary-fixed-variant: '#005236'
  tertiary-fixed: '#ffdbcc'
  tertiary-fixed-dim: '#ffb695'
  on-tertiary-fixed: '#351000'
  on-tertiary-fixed-variant: '#7b2f00'
  background: '#f8f9fa'
  on-background: '#191c1d'
  surface-variant: '#e1e3e4'
typography:
  display-lg:
    fontFamily: Manrope
    fontSize: 32px
    fontWeight: '800'
    lineHeight: 40px
    letterSpacing: -0.02em
  headline-md:
    fontFamily: Manrope
    fontSize: 24px
    fontWeight: '700'
    lineHeight: 32px
    letterSpacing: -0.01em
  headline-sm:
    fontFamily: Manrope
    fontSize: 20px
    fontWeight: '600'
    lineHeight: 28px
  body-lg:
    fontFamily: Manrope
    fontSize: 16px
    fontWeight: '400'
    lineHeight: 24px
  body-md:
    fontFamily: Manrope
    fontSize: 14px
    fontWeight: '400'
    lineHeight: 20px
  label-md:
    fontFamily: Manrope
    fontSize: 12px
    fontWeight: '600'
    lineHeight: 16px
    letterSpacing: 0.05em
  display-lg-mobile:
    fontFamily: Manrope
    fontSize: 28px
    fontWeight: '800'
    lineHeight: 36px
rounded:
  sm: 0.25rem
  DEFAULT: 0.5rem
  md: 0.75rem
  lg: 1rem
  xl: 1.5rem
  full: 9999px
spacing:
  base: 4px
  xs: 8px
  sm: 16px
  md: 24px
  lg: 32px
  xl: 48px
  container-margin: 20px
  gutter: 16px
---

## Brand & Style
The design system is engineered for a multi-category content browser that prioritizes visual clarity and content immersion. The brand personality is **sophisticated, versatile, and effortless**, acting as a high-end gallery frame for diverse subjects ranging from botanical photography to professional profiles.

The UI utilizes a **Corporate Modern** foundation infused with **Minimalist** principles. It relies on generous white space and a disciplined "content-first" hierarchy. By minimizing UI chrome and using subtle depth, the design system ensures that the interface remains invisible, allowing high-quality imagery to provide the emotional character of the experience.

**Target Audience:**
- Curators and collectors of digital content.
- Users seeking a high-signal, low-noise browsing experience.
- Professionals looking for a polished, reliable interface.

## Colors
The color strategy employs a **Neutral-Dominant** palette to ensure maximum versatility across disparate content categories (plants, people, products).

- **Primary (Indigo):** Used sparingly for high-intent actions, active navigation states, and primary buttons. It provides an energetic pulse within the neutral layout.
- **Secondary (Emerald):** Reserved for organic categories (Plants) or success states, providing a natural counterpoint to the indigo.
- **Neutrals:** A range of soft greys and crisp whites create the "Surface" and "Background" layers. `Neutral-50` (#F9FAFB) is the standard canvas color to reduce eye strain compared to pure white.
- **Contrast:** High-contrast text (#111827) ensures AA accessibility for all typographic levels.

## Typography
This design system uses **Manrope** as the sole typeface to maintain a modern, systematic, and highly readable appearance. 

- **Headlines:** Use tighter letter spacing and heavier weights (700-800) to create a strong visual anchor for content sections.
- **Body:** Set with a comfortable line height (1.5x) to ensure legibility during long-form reading in product descriptions or bio sections.
- **Labels:** Small caps or slightly tracked-out uppercase are used for category tags (e.g., "BOTANY", "FASHION") to distinguish metadata from content.

## Layout & Spacing
The layout follows a **Fluid Mobile-First** philosophy based on an 8px grid system. 

- **Safe Zones:** A standard 20px margin is applied to the left and right of all mobile screens to prevent content from hitting the bezel.
- **Rhythm:** Vertical rhythm is maintained using 24px (md) gaps between unrelated sections and 16px (sm) gaps between related card elements.
- **Aspect Ratios:** Imagery must adhere to specific ratios: 4:5 for professional portraits, 1:1 for product listings, and 16:9 for wide category banners. This consistency prevents visual "jumping" as the user scrolls.

## Elevation & Depth
Depth is communicated through **Tonal Layering** and **Soft Ambient Shadows**. This design system avoids harsh borders in favor of subtle elevation to define interactive surfaces.

- **Level 0 (Background):** #F9FAFB. The base canvas.
- **Level 1 (Cards):** Pure #FFFFFF with a 12% opacity shadow (Y: 4px, Blur: 20px). This makes cards appear to "float" slightly above the background.
- **Level 2 (Active/Modals):** Pure #FFFFFF with a 18% opacity shadow (Y: 10px, Blur: 30px). Used for bottom sheets and expanded views.
- **Backdrop:** A 40% opacity black overlay with a 10px background blur is used when modals are active to maintain focus.

## Shapes
The shape language is defined by **Soft Continuity**. 

- **Standard Radius:** 16px (rounded-lg) is the default for content cards and large containers, creating an approachable and organic feel.
- **Buttons:** Use 12px or fully rounded pill-shapes depending on the context. Primary action buttons should use 12px to maintain a structural look, while category chips use the pill shape.
- **Inner Elements:** Nested elements (like images inside a card) should have a slightly smaller radius (12px) to maintain visual nesting harmony.

## Components
Consistent component behavior is critical for a content browser:

- **Cards:** The primary vehicle for content. Should feature a 16px corner radius, no border, and a subtle drop shadow. Imagery should be top-aligned with no padding against the card edge.
- **Category Chips:** Pill-shaped, light-grey background (#F3F4F6) with `label-md` typography. When active, transition to the Primary Indigo with white text.
- **Buttons:** High-emphasis buttons are solid Primary Indigo. Low-emphasis buttons use a ghost style with a 1px neutral border.
- **Input Fields:** Soft grey backgrounds with 12px corner radius. Focus states are indicated by a 2px Primary Indigo border.
- **Navigation:** A clean bottom tab bar using 24px linear icons with labels. The active icon should be Primary Indigo.
- **Image Overlays:** Use a subtle bottom-to-top gradient (0% to 60% black) when text needs to be placed directly over imagery to ensure legibility.