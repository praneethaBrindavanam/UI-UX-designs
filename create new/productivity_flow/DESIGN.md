---
name: Productivity Flow
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
  on-surface-variant: '#424754'
  inverse-surface: '#293040'
  inverse-on-surface: '#edf0ff'
  outline: '#727785'
  outline-variant: '#c2c6d6'
  surface-tint: '#005ac2'
  primary: '#0058be'
  on-primary: '#ffffff'
  primary-container: '#2170e4'
  on-primary-container: '#fefcff'
  inverse-primary: '#adc6ff'
  secondary: '#4648d4'
  on-secondary: '#ffffff'
  secondary-container: '#6063ee'
  on-secondary-container: '#fffbff'
  tertiary: '#924700'
  on-tertiary: '#ffffff'
  tertiary-container: '#b75b00'
  on-tertiary-container: '#fffbff'
  error: '#ba1a1a'
  on-error: '#ffffff'
  error-container: '#ffdad6'
  on-error-container: '#93000a'
  primary-fixed: '#d8e2ff'
  primary-fixed-dim: '#adc6ff'
  on-primary-fixed: '#001a42'
  on-primary-fixed-variant: '#004395'
  secondary-fixed: '#e1e0ff'
  secondary-fixed-dim: '#c0c1ff'
  on-secondary-fixed: '#07006c'
  on-secondary-fixed-variant: '#2f2ebe'
  tertiary-fixed: '#ffdcc6'
  tertiary-fixed-dim: '#ffb786'
  on-tertiary-fixed: '#311400'
  on-tertiary-fixed-variant: '#723600'
  background: '#f9f9ff'
  on-background: '#141b2b'
  surface-variant: '#dce2f7'
typography:
  headline-xl:
    fontFamily: Inter
    fontSize: 36px
    fontWeight: '700'
    lineHeight: 44px
    letterSpacing: -0.02em
  headline-lg:
    fontFamily: Inter
    fontSize: 28px
    fontWeight: '600'
    lineHeight: 36px
    letterSpacing: -0.01em
  headline-md:
    fontFamily: Inter
    fontSize: 20px
    fontWeight: '600'
    lineHeight: 28px
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
  headline-lg-mobile:
    fontFamily: Inter
    fontSize: 24px
    fontWeight: '600'
    lineHeight: 32px
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
  2xl: 48px
  3xl: 64px
  gutter: 24px
  margin-mobile: 16px
  margin-desktop: 40px
---

## Brand & Style
The design system is rooted in **Minimalism** and **Modern Corporate** aesthetics, optimized for deep work and cognitive clarity. The brand personality is efficient, trustworthy, and focused, aiming to reduce "interface noise" so users can concentrate on their tasks.

The visual language utilizes heavy whitespace to create a sense of breathing room, ensuring that even data-dense screens feel manageable. The emotional response should be one of "calm control"—the UI acts as a reliable tool that recedes into the background until needed. All interactions are purposeful, avoiding unnecessary decorative elements in favor of functional clarity.

## Colors
The palette is dominated by a clean, high-contrast relationship between deep charcoal text and a soft off-white surface. 

- **Primary (#3B82F6):** Used exclusively for primary actions, progress indicators, and active states. It serves as the "signpost" for the user's next step.
- **Surface (#F9FAFB):** A cool gray used for the background to reduce screen glare compared to pure white, creating a softer environment for long-term use.
- **Neutral (#111827):** A high-contrast near-black for maximum legibility in typography and iconography.
- **Secondary (#6366F1):** An optional indigo used sparingly for accents, categorization, or secondary data visualizations to provide depth without distracting from the primary action.

## Typography
This design system utilizes **Inter** for all roles to leverage its exceptional legibility and systematic weight distribution. 

The hierarchy is strictly enforced through weight and scale. Headlines use slightly tighter letter spacing and heavier weights to feel grounded and authoritative. Body text maintains a generous line height (1.5x) to ensure readability during extended periods of focus. Labels use a slightly heavier weight and, in some instances, a subtle tracking increase to differentiate them from body content at smaller scales.

## Layout & Spacing
The layout follows a **Fluid Grid** philosophy using an 8px base unit. This ensures mathematical harmony between all elements.

- **Desktop:** A 12-column grid with 24px gutters. Content is typically contained within a maximum width of 1440px to prevent excessive line lengths.
- **Tablet:** An 8-column grid with 24px gutters.
- **Mobile:** A 4-column grid with 16px gutters and 16px side margins.

Spacing should prioritize vertical rhythm. Groups of related items (like form inputs) use `sm` or `md` spacing, while distinct sections use `xl` or `2xl` to clearly define boundaries without the need for heavy dividers.

## Elevation & Depth
Hierarchy is conveyed through **Tonal Layers** and **Ambient Shadows**. This design system avoids heavy gradients, preferring flat surfaces that are layered to show depth.

- **Level 0 (Base):** The main background surface (#F9FAFB).
- **Level 1 (Cards/Sidebar):** Pure white (#FFFFFF) surfaces. These use an extremely soft, diffused shadow (0px 4px 12px rgba(0, 0, 0, 0.03)) to appear slightly lifted.
- **Level 2 (Modals/Popovers):** Higher lift with a more pronounced shadow (0px 12px 24px rgba(0, 0, 0, 0.08)).
- **Outlines:** In addition to shadows, a very subtle 1px border (#E5E7EB) is used on cards and inputs to provide crisp definition against the soft gray background.

## Shapes
The shape language is consistently **Rounded**. The standard corner radius is 8px for standard components like buttons and input fields, while larger containers like cards use 12px-16px.

This specific level of roundedness (8px-12px) strikes a balance between the technical precision of sharp corners and the excessive playfulness of pill shapes. It feels modern and approachable while maintaining a professional "tool-like" quality.

## Components
- **Buttons:** Primary buttons are solid Blue (#3B82F6) with white text. Secondary buttons use a subtle gray outline or a ghost style with primary-colored text. All buttons have an 8px radius.
- **Input Fields:** Backgrounds are white with a 1px #E5E7EB border. On focus, the border transitions to Primary Blue with a 2px outer glow.
- **Cards:** White surfaces with 12px radius, a subtle 1px border, and a Level 1 shadow. Use generous internal padding (24px).
- **Chips/Tags:** Small, 4px radius or fully rounded. Used for status (e.g., "In Progress") with low-saturation background tints of the status color.
- **Lists:** Clean rows separated by thin 1px horizontal lines. High contrast for primary text, with metadata in a smaller, medium-gray font weight.
- **Checkboxes:** When checked, they fill with Primary Blue and a white checkmark. Use an 4px radius for a consistent but distinct look from circular radio buttons.