---
name: Clinical Precision
colors:
  surface: '#f9f9ff'
  surface-dim: '#cfdaf1'
  surface-bright: '#f9f9ff'
  surface-container-lowest: '#ffffff'
  surface-container-low: '#f0f3ff'
  surface-container: '#e7eeff'
  surface-container-high: '#dee8ff'
  surface-container-highest: '#d8e3fa'
  on-surface: '#111c2c'
  on-surface-variant: '#424752'
  inverse-surface: '#263142'
  inverse-on-surface: '#ebf1ff'
  outline: '#727783'
  outline-variant: '#c2c6d4'
  surface-tint: '#005db6'
  primary: '#00478d'
  on-primary: '#ffffff'
  primary-container: '#005eb8'
  on-primary-container: '#c8daff'
  inverse-primary: '#a9c7ff'
  secondary: '#006b5e'
  on-secondary: '#ffffff'
  secondary-container: '#7cf7e2'
  on-secondary-container: '#007164'
  tertiary: '#43484c'
  on-tertiary: '#ffffff'
  tertiary-container: '#5b6063'
  on-tertiary-container: '#d6dade'
  error: '#ba1a1a'
  on-error: '#ffffff'
  error-container: '#ffdad6'
  on-error-container: '#93000a'
  primary-fixed: '#d6e3ff'
  primary-fixed-dim: '#a9c7ff'
  on-primary-fixed: '#001b3d'
  on-primary-fixed-variant: '#00468c'
  secondary-fixed: '#7cf7e2'
  secondary-fixed-dim: '#5ddac6'
  on-secondary-fixed: '#00201c'
  on-secondary-fixed-variant: '#005047'
  tertiary-fixed: '#dfe3e7'
  tertiary-fixed-dim: '#c3c7cb'
  on-tertiary-fixed: '#171c1f'
  on-tertiary-fixed-variant: '#43474b'
  background: '#f9f9ff'
  on-background: '#111c2c'
  surface-variant: '#d8e3fa'
typography:
  display-lg:
    fontFamily: Inter
    fontSize: 48px
    fontWeight: '700'
    lineHeight: 56px
    letterSpacing: -0.02em
  headline-lg:
    fontFamily: Inter
    fontSize: 32px
    fontWeight: '600'
    lineHeight: 40px
    letterSpacing: -0.01em
  headline-lg-mobile:
    fontFamily: Inter
    fontSize: 24px
    fontWeight: '600'
    lineHeight: 32px
  headline-md:
    fontFamily: Inter
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
  body-sm:
    fontFamily: Inter
    fontSize: 14px
    fontWeight: '400'
    lineHeight: 20px
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
  sm: 0.125rem
  DEFAULT: 0.25rem
  md: 0.375rem
  lg: 0.5rem
  xl: 0.75rem
  full: 9999px
spacing:
  base: 8px
  xs: 4px
  sm: 12px
  md: 24px
  lg: 48px
  xl: 64px
  gutter: 24px
  margin-mobile: 16px
  margin-desktop: 40px
---

## Brand & Style

The design system is anchored in the principles of **Clinical Precision** and **Human-Centric Care**. The brand personality is authoritative yet approachable, evoking an emotional response of safety, reliability, and calm efficiency. 

The style utilizes a **Modern Corporate** aesthetic with heavy leanings toward **Minimalism**. By prioritizing whitespace and a systematic information hierarchy, the interface reduces cognitive load for healthcare professionals and patients alike. Visual clutter is ruthlessly eliminated to ensure that critical medical data is always the focal point. The result is a high-utility environment that feels both technologically advanced and deeply trustworthy.

## Colors

This design system utilizes a palette engineered for legibility and professional rigor. 

- **Primary (Trustworthy Blue):** Used for primary actions, navigation headers, and brand-critical elements. It signifies stability and institutional knowledge.
- **Secondary (Healing Teal):** Used for wellness-related highlights, secondary actions, and positive affirmations. It balances the "clinical" blue with a sense of vitality and recovery.
- **Neutral Grays:** A sophisticated range of cool grays provides the structural scaffolding. Backgrounds utilize the lightest tints to define work areas without the harshness of pure white.
- **Semantic Palette:** Specific high-contrast colors are reserved for status logic (Confirmed, Pending, Cancelled) to ensure immediate recognition in fast-paced medical environments.

## Typography

The design system employs **Inter** exclusively to ensure maximum readability across diverse digital displays. The typographic scale is optimized for high information density, typical of patient records and diagnostic dashboards.

- **Headlines:** Use Semi-Bold (600) weights to provide clear section anchors.
- **Body Text:** Standardized at 16px for optimal reading comfort, with 14px used for secondary metadata.
- **Labels:** Small, uppercase labels with slightly increased letter spacing are used for data field descriptors to distinguish them from the data itself.
- **Responsive Handling:** Large display types scale down on mobile to maintain structural integrity without forcing excessive scrolling.

## Layout & Spacing

The layout philosophy follows a **Fixed-Fluid Hybrid Grid**. Content is housed in a 12-column grid on desktop with a maximum container width of 1440px to prevent line lengths from becoming unreadable.

- **The 8px Rhythm:** All spacing—from internal component padding to the gaps between sections—is a multiple of 8px. This ensures a mathematical harmony and predictability across the UI.
- **Desktop:** 12-column grid, 24px gutters, 40px outer margins.
- **Tablet:** 8-column grid, 16px gutters, 24px outer margins.
- **Mobile:** 4-column grid, 16px gutters, 16px outer margins. Content stacks vertically, prioritizing patient identifiers and immediate actions at the top of the viewport.

## Elevation & Depth

To maintain a clean, clinical feel, the design system avoids heavy shadows and skeuomorphic effects. Depth is achieved through **Tonal Layering** and **Low-Contrast Outlines**.

- **Surface Tiers:** The base background is the lightest neutral gray. Interactive cards and containers sit on top in pure white (#FFFFFF).
- **Outlines:** Containers use a 1px solid border (#E2E8F0) to define boundaries without the visual weight of a shadow.
- **Subtle Elevation:** For temporary overlays like dropdowns or modals, a "Medic-Shadow" is applied: a very soft, diffused blur (12px blur, 4% opacity) with a slight blue tint to maintain brand cohesion.
- **Focused State:** Elements being interacted with receive a 2px Primary Blue stroke, ensuring clear visual feedback for accessibility.

## Shapes

The design system uses a **Soft (Level 1)** shape language. A corner radius of 4px (0.25rem) is the standard for buttons, input fields, and small components. Larger containers like cards utilize 8px (0.5rem).

This precise, minimal rounding provides a modern touch that feels professional and technical, avoiding the "playful" nature of highly rounded corners while remaining more inviting than sharp, 0px corners. It strikes the perfect balance for a regulated healthcare environment.

## Components

- **Buttons:** Primary buttons are high-contrast (Primary Blue with White text). Secondary buttons use an outlined style. All buttons have a minimum height of 44px for touch accessibility.
- **Status Badges:** Compact, pill-shaped indicators. Confirmed (Teal background, Dark Green text), Pending (Amber background, Dark Brown text), and Cancelled (Soft Red background, Dark Red text).
- **Patient Cards:** The core unit of the system. They feature a 1px border, 8px rounded corners, and a clear hierarchy: Patient Name (Headline-MD), ID Number (Label-SM), and current status badge in the top right.
- **Input Fields:** Clean, rectangular boxes with 4px rounded corners. Labels sit above the field in Label-MD style. Error states are indicated by a 2px Red stroke and a supportive error message below the field.
- **Data Tables:** High-density tables with subtle horizontal dividers. No vertical lines. Row hover states use Tertiary Gray (#F0F4F8) to assist with horizontal scanning.
- **Progress Indicators:** Linear bars using the Healing Teal color to show completion of patient intake or medical sequences.