---
name: Radially Professional
colors:
  surface: '#faf8ff'
  surface-dim: '#d2d9f4'
  surface-bright: '#faf8ff'
  surface-container-lowest: '#ffffff'
  surface-container-low: '#f2f3ff'
  surface-container: '#eaedff'
  surface-container-high: '#e2e7ff'
  surface-container-highest: '#dae2fd'
  on-surface: '#131b2e'
  on-surface-variant: '#434655'
  inverse-surface: '#283044'
  inverse-on-surface: '#eef0ff'
  outline: '#737686'
  outline-variant: '#c3c6d7'
  surface-tint: '#0053db'
  primary: '#004ac6'
  on-primary: '#ffffff'
  primary-container: '#2563eb'
  on-primary-container: '#eeefff'
  inverse-primary: '#b4c5ff'
  secondary: '#712ae2'
  on-secondary: '#ffffff'
  secondary-container: '#8a4cfc'
  on-secondary-container: '#fffbff'
  tertiary: '#ad0033'
  on-tertiary: '#ffffff'
  tertiary-container: '#d22348'
  on-tertiary-container: '#ffecec'
  error: '#ba1a1a'
  on-error: '#ffffff'
  error-container: '#ffdad6'
  on-error-container: '#93000a'
  primary-fixed: '#dbe1ff'
  primary-fixed-dim: '#b4c5ff'
  on-primary-fixed: '#00174b'
  on-primary-fixed-variant: '#003ea8'
  secondary-fixed: '#eaddff'
  secondary-fixed-dim: '#d2bbff'
  on-secondary-fixed: '#25005a'
  on-secondary-fixed-variant: '#5a00c6'
  tertiary-fixed: '#ffdadb'
  tertiary-fixed-dim: '#ffb2b7'
  on-tertiary-fixed: '#40000d'
  on-tertiary-fixed-variant: '#92002a'
  background: '#faf8ff'
  on-background: '#131b2e'
  surface-variant: '#dae2fd'
typography:
  display-name:
    fontFamily: Manrope
    fontSize: 20px
    fontWeight: '700'
    lineHeight: 28px
    letterSpacing: -0.02em
  handle-sm:
    fontFamily: JetBrains Mono
    fontSize: 13px
    fontWeight: '500'
    lineHeight: 16px
    letterSpacing: -0.01em
  body-md:
    fontFamily: Manrope
    fontSize: 16px
    fontWeight: '400'
    lineHeight: 24px
  label-caps:
    fontFamily: Manrope
    fontSize: 12px
    fontWeight: '600'
    lineHeight: 16px
    letterSpacing: 0.05em
  headline-lg-mobile:
    fontFamily: Manrope
    fontSize: 28px
    fontWeight: '800'
    lineHeight: 34px
    letterSpacing: -0.03em
rounded:
  sm: 0.25rem
  DEFAULT: 0.5rem
  md: 0.75rem
  lg: 1rem
  xl: 1.5rem
  full: 9999px
spacing:
  unit: 4px
  xs: 4px
  sm: 8px
  md: 12px
  lg: 16px
  xl: 24px
  margin-mobile: 16px
  gutter-mobile: 12px
---

## Brand & Style

The design system is engineered for a mobile-first experience that balances professional utility with an approachable, human-centric aesthetic. It targets a modern workforce and social-professional audience, prioritizing clarity and identity.

The visual style is **Corporate Modern with a Soft Geometric twist**. It utilizes high-quality typography and ample whitespace to ensure the interface feels breathable, while employing subtle tonal layering to create a sense of organized depth. The emotional response should be one of reliability and ease, where the user's identity (via avatars) is the focal point of every interaction.

## Colors

The palette is anchored by a deep professional Navy neutral and a vibrant Blue primary. Secondary and Tertiary colors are reserved for high-impact actions and brand moments. 

A dedicated "Status Palette" is integrated into the design system to provide immediate visual feedback on user availability within profile components. These colors should always be paired with a high-contrast stroke when overlaid on avatars to ensure accessibility and visibility. 

The background follows a tiered grayscale approach:
- **Surface:** #FFFFFF (Main app background)
- **Surface-Muted:** #F8FAFC (Secondary containers/lists)
- **Surface-Overlay:** #F1F5F9 (Input backgrounds)

## Typography

Typography centers on **Manrope** for its unique balance of geometric precision and warm, rounded terminals, which mirrors the "soft geometric" brand pillar. 

- **Names & Headlines:** Use tighter letter spacing and heavier weights to create a strong visual anchor for user profiles.
- **Handles & Technical Data:** Use **JetBrains Mono** at small scales for handles (@username) or metadata to provide a distinct, "built" feel that separates identity from content.
- **Scale:** Maintain a strict vertical rhythm. Mobile body text is optimized at 16px for legibility, while labels use uppercase styling for hierarchy without increasing size.

## Layout & Spacing

This design system employs a **Tight Fluid Grid** model. Given the mobile focus, spacing is condensed to maximize information density without sacrificing touch targets.

- **Baseline Grid:** A 4px incremental scale ensures all elements align predictably.
- **Margins:** Standard mobile views use a 16px side margin. 
- **Component Spacing:** Use `md` (12px) for internal padding within cards and `sm` (8px) for spacing between related elements, such as an avatar and its associated text block.
- **Safe Areas:** Ensure all bottom-fixed elements account for device home-indicators with a minimum `xl` bottom padding.

## Elevation & Depth

Depth is communicated through **Tonal Layering** and **Soft Ambient Shadows**. 

1.  **Level 0 (Base):** Flat #FFFFFF background.
2.  **Level 1 (Cards):** Subtle 1px border (#E2E8F0) with no shadow, or a very soft 4px blur, 2% opacity black shadow.
3.  **Level 2 (Active/Floating):** Used for bottom sheets and floating action buttons. Uses a 12px blur, 8% opacity shadow tinted with the `neutral_color_hex`.

Avoid heavy blurs; the "soft geometric" feel comes from shape and color rather than dramatic physical depth.

## Shapes

The shape language is the core differentiator of this design system. 

- **General UI Elements:** Buttons, cards, and input fields use a standard `rounded` (0.5rem) or `rounded-lg` (1rem) corner radius.
- **Avatars:** Two specific tokens are provided. Use `avatar_circular` for primary user identities in lists. Use `avatar_squircle` (1rem) for "Sub-identities," such as organizations, groups, or secondary profile views to create visual distinction between person and entity.
- **Inputs:** Maintain a consistent 0.75rem (rounded-xl) for search bars to make them feel more interactive and "soft."

## Components

### Profile Avatars
The signature component. Must include a `status-indicator` slot at the bottom-right. The indicator should have a 2px stroke matching the background color to create a "cutout" effect.

### Buttons
- **Primary:** Solid fill using `primary_color_hex` with `rounded` (0.5rem) corners.
- **Ghost:** Transparent background with `headline_font` medium weight.
- **Size:** Minimum touch target of 44x44pt.

### Input Fields
Filled style using `Surface-Overlay`. No border in the default state, shifting to a 2px `primary_color_hex` border on focus. Label text should use the `label-caps` typography style.

### Lists & Cells
Use `gutter-mobile` for horizontal spacing between the avatar and the text stack. Lists should be separated by a light 1px divider (#F1F5F9) that is inset by the width of the avatar.

### Status Chips
Small, high-contrast pills using a 10% opacity version of the status colors for the background and the 100% opacity color for the text. Use `handle-sm` typography.