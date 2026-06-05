---
name: Premium Editorial
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
  on-surface-variant: '#45464d'
  inverse-surface: '#2d3133'
  inverse-on-surface: '#eff1f3'
  outline: '#76777d'
  outline-variant: '#c6c6cd'
  surface-tint: '#565e74'
  primary: '#000000'
  on-primary: '#ffffff'
  primary-container: '#131b2e'
  on-primary-container: '#7c839b'
  inverse-primary: '#bec6e0'
  secondary: '#b6191a'
  on-secondary: '#ffffff'
  secondary-container: '#d9352f'
  on-secondary-container: '#fffbff'
  tertiary: '#000000'
  on-tertiary: '#ffffff'
  tertiary-container: '#0d1c2e'
  on-tertiary-container: '#77859a'
  error: '#ba1a1a'
  on-error: '#ffffff'
  error-container: '#ffdad6'
  on-error-container: '#93000a'
  primary-fixed: '#dae2fd'
  primary-fixed-dim: '#bec6e0'
  on-primary-fixed: '#131b2e'
  on-primary-fixed-variant: '#3f465c'
  secondary-fixed: '#ffdad6'
  secondary-fixed-dim: '#ffb4ab'
  on-secondary-fixed: '#410002'
  on-secondary-fixed-variant: '#93000b'
  tertiary-fixed: '#d5e3fc'
  tertiary-fixed-dim: '#b9c7df'
  on-tertiary-fixed: '#0d1c2e'
  on-tertiary-fixed-variant: '#3a485b'
  background: '#f7f9fb'
  on-background: '#191c1e'
  surface-variant: '#e0e3e5'
typography:
  display-lg:
    fontFamily: Playfair Display
    fontSize: 48px
    fontWeight: '700'
    lineHeight: 56px
    letterSpacing: -0.02em
  headline-lg:
    fontFamily: Playfair Display
    fontSize: 32px
    fontWeight: '700'
    lineHeight: 40px
  headline-lg-mobile:
    fontFamily: Playfair Display
    fontSize: 28px
    fontWeight: '700'
    lineHeight: 34px
  headline-md:
    fontFamily: Playfair Display
    fontSize: 24px
    fontWeight: '600'
    lineHeight: 32px
  body-lg:
    fontFamily: Source Sans Three
    fontSize: 18px
    fontWeight: '400'
    lineHeight: 28px
  body-md:
    fontFamily: Source Sans Three
    fontSize: 16px
    fontWeight: '400'
    lineHeight: 24px
  label-caps:
    fontFamily: Archivo Narrow
    fontSize: 12px
    fontWeight: '700'
    lineHeight: 16px
    letterSpacing: 0.05em
  caption:
    fontFamily: Source Sans Three
    fontSize: 14px
    fontWeight: '400'
    lineHeight: 20px
spacing:
  base: 4px
  stack-xs: 8px
  stack-sm: 16px
  stack-md: 24px
  stack-lg: 40px
  container-margin: 20px
  gutter: 16px
---

## Brand & Style

The design system is anchored in the tradition of high-end journalism, prioritizing clarity, authority, and longevity. The target audience consists of discerning readers who value deep-dive reporting and a focused, distraction-free environment. 

The aesthetic is a blend of **Minimalism** and **High-Contrast Boldness**. It leverages heavy whitespace to allow the content to breathe, while using sharp, deliberate strokes and high-contrast typography to establish a clear information hierarchy. The emotional response should be one of calm confidence—a digital sanctuary for intellectual engagement that feels as deliberate and curated as a printed broadsheet.

## Colors

This design system utilizes a restricted, high-contrast palette to maintain an authoritative tone. 

- **Primary**: A deep, "Ink" blue-black (#0F172A) used for headlines and primary UI elements.
- **Secondary (Accent)**: A "Heritage Crimson" (#B91C1C) reserved for breaking news labels, category markers, and critical calls to action.
- **Neutral**: A crisp white background complemented by "Paper" off-whites (#F8FAFC) for container backgrounds and a range of functional grays (#475569) for secondary metadata and borders.

The default mode is light, optimizing legibility for long-form reading, though a dark "Midnight" mode may be implemented using the same primary color as the surface.

## Typography

Typography is the core of this design system. We use a "tri-axis" font strategy:
1. **Playfair Display**: Used for headlines and display text to evoke the elegance of a masthead.
2. **Source Sans Three**: A highly legible, humanist sans-serif for body copy, ensuring comfort during extended reading sessions.
3. **Archivo Narrow**: A condensed sans-serif used for utility labels, categories, and metadata to save horizontal space and provide a modern, technical contrast.

Optical sizing is critical; larger headlines should utilize tighter letter spacing, while small labels require increased tracking for readability.

## Layout & Spacing

The layout follows a **Fixed-Fluid Hybrid** model. On mobile devices, a single-column layout is utilized with 20px side margins to prevent text from hitting the screen edges. 

The vertical rhythm is based on a 4px baseline grid. Headlines are separated from body text by 16px (`stack-sm`), while distinct articles or sections are separated by 40px (`stack-lg`) to provide a clear mental break. Narrative components (images, pull quotes) should bleed to the container margin or occasionally break the margin for visual interest.

## Elevation & Depth

This design system avoids shadows in favor of **Tonal Layers** and **Low-Contrast Outlines**. 

Hierarchy is established through the physical stacking of elements and the use of subtle 1px borders (#E2E8F0). 
- **Surface**: The base layer is pure white.
- **Section Dividers**: Thin, horizontal lines create "shelves" for content.
- **Overlays**: Modals and menus use a very slight backdrop blur (5px) with a solid border to maintain the "paper" feel rather than a digital "glass" feel.

## Shapes

The shape language is strictly **Sharp (0)**. To maintain an authoritative and traditional editorial feel, all containers, buttons, and images utilize 90-degree corners. This evokes the feeling of a cut newspaper or a structured magazine layout. Avoid any rounding of UI elements, as it softens the brand's serious and professional tone.

## Components

### Buttons
Primary buttons are solid `primary_color_hex` with white uppercase `label-caps` text. Secondary buttons are outlined with a 1px border. No rounded corners.

### Chips / Category Labels
Small, rectangular boxes with a thin border or a light gray background. Use `label-caps` for the category name (e.g., "POLITICS", "TECHNOLOGY").

### Cards
Article cards should rely on typography rather than containers. Use a thin horizontal rule above the headline. The headline (`headline-md`) should be prominent, followed by a concise body summary.

### Input Fields
Minimalist design with only a bottom border (1px). Focus state shifts the border color to the accent Crimson.

### Pull Quotes
Set in `headline-md` italic, indented from the main body text, with a 2px vertical accent bar of `primary_color_hex` on the left side.

### Navigation
A clean top bar featuring the masthead in the center, with a simple "hamburger" menu and search icon. Use high-contrast icons with a 2pt stroke weight.