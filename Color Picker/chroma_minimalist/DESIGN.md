---
name: Chroma Minimalist
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
  on-surface-variant: '#414755'
  inverse-surface: '#2e3132'
  inverse-on-surface: '#f0f1f2'
  outline: '#717786'
  outline-variant: '#c1c6d7'
  surface-tint: '#005bc1'
  primary: '#0058bc'
  on-primary: '#ffffff'
  primary-container: '#0070eb'
  on-primary-container: '#fefcff'
  inverse-primary: '#adc6ff'
  secondary: '#4648d4'
  on-secondary: '#ffffff'
  secondary-container: '#6063ee'
  on-secondary-container: '#fffbff'
  tertiary: '#9e3d00'
  on-tertiary: '#ffffff'
  tertiary-container: '#c64f00'
  on-tertiary-container: '#fffbff'
  error: '#ba1a1a'
  on-error: '#ffffff'
  error-container: '#ffdad6'
  on-error-container: '#93000a'
  primary-fixed: '#d8e2ff'
  primary-fixed-dim: '#adc6ff'
  on-primary-fixed: '#001a41'
  on-primary-fixed-variant: '#004493'
  secondary-fixed: '#e1e0ff'
  secondary-fixed-dim: '#c0c1ff'
  on-secondary-fixed: '#07006c'
  on-secondary-fixed-variant: '#2f2ebe'
  tertiary-fixed: '#ffdbcc'
  tertiary-fixed-dim: '#ffb595'
  on-tertiary-fixed: '#351000'
  on-tertiary-fixed-variant: '#7c2e00'
  background: '#f8f9fa'
  on-background: '#191c1d'
  surface-variant: '#e1e3e4'
typography:
  display-lg:
    fontFamily: Inter
    fontSize: 48px
    fontWeight: '700'
    lineHeight: '1.1'
    letterSpacing: -0.02em
  h1:
    fontFamily: Inter
    fontSize: 32px
    fontWeight: '600'
    lineHeight: '1.2'
    letterSpacing: -0.01em
  h2:
    fontFamily: Inter
    fontSize: 24px
    fontWeight: '600'
    lineHeight: '1.3'
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
  body-sm:
    fontFamily: Inter
    fontSize: 14px
    fontWeight: '400'
    lineHeight: '1.5'
  label-md:
    fontFamily: Inter
    fontSize: 14px
    fontWeight: '600'
    lineHeight: '1'
    letterSpacing: 0.02em
  label-sm:
    fontFamily: Inter
    fontSize: 12px
    fontWeight: '500'
    lineHeight: '1'
  mono-label:
    fontFamily: Space Grotesk
    fontSize: 13px
    fontWeight: '500'
    lineHeight: '1'
    letterSpacing: 0.05em
rounded:
  sm: 0.125rem
  DEFAULT: 0.25rem
  md: 0.375rem
  lg: 0.5rem
  xl: 0.75rem
  full: 9999px
spacing:
  unit: 4px
  xs: 4px
  sm: 8px
  md: 16px
  lg: 24px
  xl: 48px
  panel-width: 320px
  gutter: 12px
---

## Brand & Style

This design system is built for a color-focused creative tool where the user's content is the protagonist. The brand personality is precise, sophisticated, and invisible—functioning as a high-end gallery space that elevates the vibrant hues it contains. 

The aesthetic leverages **Minimalism** with a focus on high-utility density. By utilizing "white space" that is actually a sophisticated palette of soft, cool grays, the interface reduces cognitive load and prevents UI-induced color fatigue. The emotional response is one of professional clarity and creative freedom, ensuring that the tool feels like a precise instrument rather than a toy.

## Colors

The palette is intentionally restrained to preserve the integrity of the user's color work. The "Crisp White" canvas serves as the primary workspace, while a tiered system of "Soft Grays" (Surface-low to high) defines the periphery and utility panels. 

Primary and secondary colors are used sparingly, reserved for active states, primary actions, and system feedback. For accessibility indicators, high-contrast tokens are provided to ensure that color-blind users can navigate color-intensive data via iconography and text labels.

## Typography

This design system utilizes **Inter** for its neutral, systematic, and highly legible qualities. The typographic scale is optimized for toolbars and property inspectors where information density is high. 

A secondary monospaced font is introduced for HEX codes and coordinate values to ensure visual stability when numbers change. Letter spacing is slightly tightened on large headings for a premium feel and widened on small labels to maintain legibility against gray backgrounds.

## Layout & Spacing

The layout philosophy follows a **Fixed Grid** for utility panels and property inspectors, with a **Fluid Canvas** for the main creative area. This ensures that the tools remain in a predictable, muscle-memory location while the creative workspace maximizes available screen real estate.

Spacing is based on a 4px baseline grid. Use 16px (md) for standard padding within cards and panels, and 8px (sm) for internal element grouping. Wide 48px margins (xl) should be used to separate major functional areas, creating the "gallery" feel.

## Elevation & Depth

Visual hierarchy is established primarily through **Tonal Layers** rather than heavy shadows. 
- **Level 0 (Canvas):** Pure white (#FFFFFF), the base workspace.
- **Level 1 (Panels):** Soft gray (#F9FAFB) with a 1px border (#F3F4F6) to define the workspace boundaries.
- **Level 2 (Popovers/Modals):** Subtle ambient shadows are used here to indicate temporary focus. Shadows should be ultra-diffused: `0 10px 30px rgba(0,0,0,0.04)`.
- **Level 3 (Interactive Elements):** Buttons and swatches use a crisp 1px border to separate them from the surface, creating a "flat-but-tactile" feel.

## Shapes

The shape language is **Soft** (roundedness 1). This choice balances the technical precision of the tool with an approachable, modern feel. 

- **Swatches:** Use `rounded-lg` (0.5rem) to make color chips feel like physical objects.
- **Controls/Inputs:** Use base `rounded` (0.25rem) for a crisp, professional look.
- **Floating Toolbars:** Use `rounded-xl` (0.75rem) to distinguish them from anchored panels.

## Components

### Color Swatches
Large, rounded squares with a subtle 1px inner stroke to ensure white or light yellow colors don't bleed into the background. Active states are indicated by a 2px blue ring with a 2px white gap (offset).

### Color Sliders
Track height of 6px with a circular, 20px diameter handle. The handle must have a white fill and a soft shadow to remain visible when positioned over any color. The track itself should use a gradient representation of the attribute (e.g., Hue, Saturation).

### Accessibility Indicators
Small, high-contrast badges (Checkmark, X, or Contrast Ratio text) that appear next to color combinations. Use "WCAG AA" or "WCAG AAA" labels in the `label-sm` typographic style.

### Buttons
- **Primary:** Solid fill with white text.
- **Secondary:** Ghost style with a light gray border (#D1D5DB) and dark text.
- **Icon-only:** Used for tools (Eyedropper, Brush). 32x32px hit area with a soft gray hover state.

### Input Fields
Compact 32px height for property panels. Use `mono-label` for numeric values. Borders are light gray, turning primary blue on focus.

### Cards
Used for "Palette Collections." Flat design with a subtle 1px border. No shadows unless the card is being dragged/reordered.