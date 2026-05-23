---
name: Aura Onboarding
colors:
  surface: '#f9f9ff'
  surface-dim: '#cfdaf2'
  surface-bright: '#f9f9ff'
  surface-container-lowest: '#ffffff'
  surface-container-low: '#f0f3ff'
  surface-container: '#e7eeff'
  surface-container-high: '#dee8ff'
  surface-container-highest: '#d8e3fb'
  on-surface: '#111c2d'
  on-surface-variant: '#3d4947'
  inverse-surface: '#263143'
  inverse-on-surface: '#ecf1ff'
  outline: '#6d7a77'
  outline-variant: '#bcc9c6'
  surface-tint: '#006a61'
  primary: '#00685f'
  on-primary: '#ffffff'
  primary-container: '#008378'
  on-primary-container: '#f4fffc'
  inverse-primary: '#6bd8cb'
  secondary: '#0058be'
  on-secondary: '#ffffff'
  secondary-container: '#2170e4'
  on-secondary-container: '#fefcff'
  tertiary: '#525e5c'
  on-tertiary: '#ffffff'
  tertiary-container: '#6b7775'
  on-tertiary-container: '#f3fffc'
  error: '#ba1a1a'
  on-error: '#ffffff'
  error-container: '#ffdad6'
  on-error-container: '#93000a'
  primary-fixed: '#89f5e7'
  primary-fixed-dim: '#6bd8cb'
  on-primary-fixed: '#00201d'
  on-primary-fixed-variant: '#005049'
  secondary-fixed: '#d8e2ff'
  secondary-fixed-dim: '#adc6ff'
  on-secondary-fixed: '#001a42'
  on-secondary-fixed-variant: '#004395'
  tertiary-fixed: '#d8e5e2'
  tertiary-fixed-dim: '#bcc9c6'
  on-tertiary-fixed: '#121e1c'
  on-tertiary-fixed-variant: '#3d4947'
  background: '#f9f9ff'
  on-background: '#111c2d'
  surface-variant: '#d8e3fb'
typography:
  headline-lg:
    fontFamily: Inter
    fontSize: 30px
    fontWeight: '700'
    lineHeight: 38px
    letterSpacing: -0.02em
  headline-lg-mobile:
    fontFamily: Inter
    fontSize: 26px
    fontWeight: '700'
    lineHeight: 32px
    letterSpacing: -0.02em
  headline-md:
    fontFamily: Inter
    fontSize: 20px
    fontWeight: '600'
    lineHeight: 28px
  body-lg:
    fontFamily: Inter
    fontSize: 16px
    fontWeight: '400'
    lineHeight: 24px
  label-md:
    fontFamily: Inter
    fontSize: 14px
    fontWeight: '600'
    lineHeight: 20px
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
  margin-mobile: 1.5rem
  gutter-mobile: 1rem
  stack-sm: 0.5rem
  stack-md: 1rem
  stack-lg: 2rem
  touch-target-min: 3rem
---

## Brand & Style

The design system is centered on the concept of "Approachable Reliability." It targets users during the high-friction moment of registration, aiming to reduce anxiety through a "Friendly Professional" aesthetic. 

The style utilizes **Corporate Modern** principles—refined, balanced, and predictable—but softens them with generous whitespace and a calming color palette. The UI should feel like a guided conversation rather than a technical hurdle. Every transition should be smooth, and every interaction should feel intentional and supportive, evoking an emotional response of clarity and trust.

## Colors

The palette is anchored by **Teal (Primary)** to represent growth and stability, and **Soft Blue (Secondary)** to instill a sense of calm. 

- **Primary (#0D9488):** Used for primary actions and active progress states.
- **Secondary (#3B82F6):** Used for accent elements and subtle interactive highlights.
- **Surface/Tertiary (#F0FDFA):** A very soft teal tint used for input backgrounds and container fills to keep the interface feeling "airy."
- **Neutral (#1E293B):** A deep slate used for high-contrast typography to ensure maximum legibility against light backgrounds.
- **Background:** The default page background is a clean, neutral white (#FFFFFF) to maximize the "Clean & Modern" aesthetic.

## Typography

This design system utilizes **Inter** exclusively to leverage its exceptional legibility and neutral, modern character. 

Hierarchy is established through tight letter-spacing on headlines and generous line-heights for body copy. Headlines use a bold weight to anchor the page, while labels are kept clear and slightly heavier (`600`) to ensure they are easily scannable above input fields. Mobile-specific scaling is applied to the largest headlines to prevent awkward text wrapping on smaller viewports.

## Layout & Spacing

The layout follows a **Fluid Grid** model optimized for mobile-first delivery. 

- **Margins:** A standard 24px (1.5rem) side margin ensures content does not feel cramped against the screen edges.
- **Rhythm:** An 8px linear scale drives all vertical spacing. "Stack" tokens define the distance between related elements (label to input = `stack-sm`) and unrelated sections (input to button = `stack-lg`).
- **Touch Targets:** All interactive elements maintain a minimum height of 48px to ensure accessibility for users of all motor abilities.

## Elevation & Depth

To maintain a "Friendly Professional" feel, depth is created using **Ambient Shadows** and **Tonal Layers** rather than harsh borders.

- **Surface Tiers:** Primary containers (like cards) sit on Level 1, using a very soft, diffused shadow (0px 4px 12px, 5% opacity Neutral) to appear slightly lifted.
- **Interactive Depth:** Input fields use a subtle inner stroke (1px, Primary at 10% opacity) rather than a shadow, creating a recessed, tactile feel that invites typing.
- **Focus States:** When active, inputs gain a soft Primary-colored glow (4px spread) to guide the user's attention.

## Shapes

The shape language is consistently **Rounded** (Level 2). 

This 8px base radius applies to input fields, buttons, and container cards. This specific level of roundedness strikes a balance—it is soft enough to feel "friendly" and "inviting," but structured enough to maintain a "professional" and "modern" corporate identity. Progress bars and toggle tracks use the `rounded-xl` (24px) setting to create pill-shaped forms that contrast against the more rectangular inputs.

## Components

### Buttons
- **Primary:** Full-width, 56px height, Primary Teal fill, White text. Bold weight.
- **Secondary:** Transparent background, Primary Teal border (1px), centered text.

### Input Fields
- **Container:** 56px height, `tertiary` background color, 8px corner radius.
- **Labels:** Positioned outside the field, using `label-md` for high visibility.
- **States:** Error states use a soft coral (#F87171) for both the border and a small helper text below the field.

### Progress Bars
- **Style:** Stepped horizontal bar.
- **Active Step:** Primary Teal.
- **Inactive Step:** 10% opacity Primary Teal.
- **Animation:** Smooth width transition (300ms ease-in-out) between registration steps.

### Chips
- Used for selectable interests or tags. Small, 32px height, `rounded-xl`, with a subtle Secondary Blue tint when selected.

### Cards
- Used for grouping related form sections. White background, 16px padding, and Level 1 Ambient Shadow.