---
name: Paper & Ink Productivity
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
  on-surface-variant: '#464652'
  inverse-surface: '#27313f'
  inverse-on-surface: '#eaf1ff'
  outline: '#777683'
  outline-variant: '#c7c5d4'
  surface-tint: '#4f54b4'
  primary: '#15157d'
  on-primary: '#ffffff'
  primary-container: '#2e3192'
  on-primary-container: '#9da1ff'
  inverse-primary: '#c0c1ff'
  secondary: '#5e5f56'
  on-secondary: '#ffffff'
  secondary-container: '#e4e3d7'
  on-secondary-container: '#64655c'
  tertiary: '#222935'
  on-tertiary: '#ffffff'
  tertiary-container: '#383f4c'
  on-tertiary-container: '#a3aab9'
  error: '#ba1a1a'
  on-error: '#ffffff'
  error-container: '#ffdad6'
  on-error-container: '#93000a'
  primary-fixed: '#e1e0ff'
  primary-fixed-dim: '#c0c1ff'
  on-primary-fixed: '#04006d'
  on-primary-fixed-variant: '#373a9b'
  secondary-fixed: '#e4e3d7'
  secondary-fixed-dim: '#c7c7bc'
  on-secondary-fixed: '#1b1c15'
  on-secondary-fixed-variant: '#46473f'
  tertiary-fixed: '#dce2f3'
  tertiary-fixed-dim: '#c0c7d6'
  on-tertiary-fixed: '#151c27'
  on-tertiary-fixed-variant: '#404754'
  background: '#f8f9ff'
  on-background: '#121c2a'
  surface-variant: '#d9e3f6'
typography:
  display:
    fontFamily: Inter
    fontSize: 24px
    fontWeight: '700'
    lineHeight: 32px
    letterSpacing: -0.02em
  headline-md:
    fontFamily: Inter
    fontSize: 18px
    fontWeight: '600'
    lineHeight: 24px
    letterSpacing: -0.01em
  body-lg:
    fontFamily: Inter
    fontSize: 16px
    fontWeight: '400'
    lineHeight: 24px
    letterSpacing: 0em
  body-sm:
    fontFamily: Inter
    fontSize: 14px
    fontWeight: '400'
    lineHeight: 20px
    letterSpacing: 0em
  label-caps:
    fontFamily: Inter
    fontSize: 12px
    fontWeight: '600'
    lineHeight: 16px
    letterSpacing: 0.05em
  helper-text:
    fontFamily: Inter
    fontSize: 12px
    fontWeight: '400'
    lineHeight: 16px
    letterSpacing: 0em
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
  md: 16px
  lg: 24px
  xl: 32px
  widget-margin: 12px
  stack-gap: 12px
---

## Brand & Style

The design system is centered on the concept of "Digital Tactility." It bridges the gap between the physical comfort of a premium paper notebook and the efficiency of a modern digital interface. The brand personality is focused, dependable, and quiet, aiming to reduce cognitive load for the user.

The style is **Minimalist with Tactile accents**. It avoids unnecessary ornamentation, favoring whitespace and clear structural hierarchy. By using a warm, non-white base, the UI feels less like a glowing screen and more like a tool. Subtle shadows and precise geometry ensure the system feels contemporary rather than nostalgic.

## Colors

The palette is anchored by **Paper (#FDFCF0)**, a warm, off-white yellow that serves as the primary background to reduce eye strain. **Deep Indigo (#2E3192)** acts as the "Ink," reserved for primary actions, active states, and critical information.

Grays are utilized to provide structure without the harshness of pure black. **Soft Gray (#F3F4F6)** defines secondary containers, while **Neutral Gray (#6B7280)** handles metadata and deactivated states. This high-contrast relationship between the warm base and the cool indigo accent ensures immediate visual recognition of interactive elements.

## Typography

The design system utilizes **Inter** for its exceptional legibility and neutral character. To maintain the professional "productivity" feel, the typographic scale is tight and functional.

- **Headlines:** Use semi-bold weights with slight negative letter-spacing to appear "tight" like printed headers.
- **Body:** Standardized at 14px and 16px for optimal balance between information density and readability on mobile screens.
- **Labels:** Small caps are used sparingly for category headers or section labels to provide a distinct visual break from task descriptions.

## Layout & Spacing

This design system uses a **contextual layout model** optimized for widget constraints. It relies on a 4px baseline grid to ensure all elements align vertically. 

The standard internal padding for components is **16px (md)**, while nested elements like list items use **12px (stack-gap)** to create a sense of grouped information. Layouts should prioritize vertical stacking to fit narrow widget widths, using "safe margins" of 12px from the widget edge to ensure content doesn't feel cramped against the system UI.

## Elevation & Depth

Hierarchy is achieved through **Tonal Layers** supplemented by **Ambient Shadows**. 

1. **Base Layer:** The "Paper" background (#FDFCF0).
2. **Raised Layer:** Cards and interactive containers use a pure white background or a slightly lighter tint of paper, paired with a very soft, diffused shadow (Offset: 0, 4px; Blur: 12px; Color: Indigo at 4% opacity).
3. **Interactive Depth:** When a user presses a component, it should appear to "sink" by removing the shadow or slightly darkening the background color, mimicking the physical act of pressing on a page.

## Shapes

The shape language is characterized by **Medium Roundedness**. A standard radius of **8px to 12px** is applied to all primary containers and buttons. This avoids the "toy-like" feel of fully pill-shaped elements while remaining friendlier and more integrated into modern OS environments than sharp corners.

Small internal elements like checkboxes or tags should use a smaller **4px** radius to maintain a crisp, sharp appearance at scale.

## Components

- **Buttons:** Primary buttons are filled with Deep Indigo and use white text. Secondary buttons use a "ghost" style with an Indigo border or a soft gray background.
- **Task Cards:** Use a subtle 1px border (#E5E7EB) rather than a heavy shadow to define boundaries on the paper background.
- **Checkboxes:** When checked, the box should fill with Deep Indigo. The "unchecked" state is a simple 2px stroke in soft gray.
- **Chips/Tags:** Use a slightly darker "Paper" tint (#F3F2E0) with Indigo text for high-contrast categorization.
- **Input Fields:** Minimalist design with a bottom-border only, mimicking the ruled lines of a notebook, which transforms into a full 1px Indigo stroke upon focus.
- **Progress Bars:** Thin, 4px height tracks in soft gray with a Deep Indigo fill to show task completion.