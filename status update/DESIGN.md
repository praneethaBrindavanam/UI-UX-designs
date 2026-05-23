---
name: Clarity & Pulse
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
  on-surface-variant: '#434653'
  inverse-surface: '#2e3132'
  inverse-on-surface: '#f0f1f2'
  outline: '#737784'
  outline-variant: '#c3c6d5'
  surface-tint: '#2559bd'
  primary: '#00327d'
  on-primary: '#ffffff'
  primary-container: '#0047ab'
  on-primary-container: '#a5bdff'
  inverse-primary: '#b1c5ff'
  secondary: '#006c49'
  on-secondary: '#ffffff'
  secondary-container: '#6cf8bb'
  on-secondary-container: '#00714d'
  tertiary: '#4f3000'
  on-tertiary: '#ffffff'
  tertiary-container: '#6e4400'
  on-tertiary-container: '#ffae3c'
  error: '#ba1a1a'
  on-error: '#ffffff'
  error-container: '#ffdad6'
  on-error-container: '#93000a'
  primary-fixed: '#dae2ff'
  primary-fixed-dim: '#b1c5ff'
  on-primary-fixed: '#001946'
  on-primary-fixed-variant: '#00419e'
  secondary-fixed: '#6ffbbe'
  secondary-fixed-dim: '#4edea3'
  on-secondary-fixed: '#002113'
  on-secondary-fixed-variant: '#005236'
  tertiary-fixed: '#ffddb8'
  tertiary-fixed-dim: '#ffb95f'
  on-tertiary-fixed: '#2a1700'
  on-tertiary-fixed-variant: '#653e00'
  background: '#f8f9fa'
  on-background: '#191c1d'
  surface-variant: '#e1e3e4'
typography:
  headline-lg:
    fontFamily: Inter
    fontSize: 32px
    fontWeight: '700'
    lineHeight: 40px
    letterSpacing: -0.02em
  headline-lg-mobile:
    fontFamily: Inter
    fontSize: 24px
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
  body-sm:
    fontFamily: Inter
    fontSize: 14px
    fontWeight: '400'
    lineHeight: 20px
  label-bold:
    fontFamily: Inter
    fontSize: 12px
    fontWeight: '600'
    lineHeight: 16px
    letterSpacing: 0.05em
  label-md:
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
  base: 4px
  xs: 4px
  sm: 8px
  md: 16px
  lg: 24px
  xl: 32px
  margin-mobile: 16px
  gutter-mobile: 12px
---

## Brand & Style

The design system is centered on the principles of **Functional Minimalism** and **Immediate Comprehension**. Designed primarily for status updates and real-time notifications, the brand personality is dependable, transparent, and calm. It avoids visual clutter to ensure that critical information remains the focal point.

The aesthetic utilizes a modern corporate style with a touch of warmth. It leverages high-contrast typography against clean, expansive off-white surfaces to reduce cognitive load. The emotional response should be one of "controlled urgency"—users should feel informed and in control without being overwhelmed by the interface.

## Colors

The palette is strictly functional, mapping specific hues to system states to ensure universal recognition.

*   **Primary (Cobalt Blue):** Used for information, active states, and primary actions. It represents stability and focus.
*   **Success (Emerald Green):** Dedicated to positive outcomes, completed tasks, and healthy system status.
*   **Warning (Amber):** Utilized for non-blocking issues or items requiring attention.
*   **Error (Rose Red):** Reserved for critical failures, destructive actions, and immediate blocking alerts.
*   **Neutral:** A range of off-whites and cool grays used for backgrounds and borders to maintain a "breathable" interface.

All state colors must maintain a contrast ratio of at least 4.5:1 against the background for accessibility.

## Typography

This design system utilizes **Inter** for its exceptional legibility on mobile screens and neutral, systematic tone. 

The type hierarchy is designed to guide the eye toward the most critical status update first. Headlines use tighter letter spacing and heavier weights to feel "anchored," while body text maintains a generous line height to improve scanning speed. Small labels use a medium weight or uppercase styling to differentiate them from primary content without requiring larger font sizes.

## Layout & Spacing

The system follows a strict **4px baseline grid**. For mobile layouts, the primary container uses a 16px side margin. 

Spacing is used to group related information:
*   **8px (sm):** Between internal elements of a notification (e.g., icon and title).
*   **16px (md):** Between distinct list items or notification cards.
*   **24px (lg):** Between logical sections of the app.

Layouts should be fluid within the 16px margins, ensuring that cards and notifications expand to the full width of the viewport for maximum readability.

## Elevation & Depth

Visual hierarchy is established through a combination of **Tonal Layers** and **Ambient Shadows**.

1.  **Background:** The lowest layer, using `#F9FAFB` (Off-white).
2.  **Surface:** White (`#FFFFFF`) cards sit atop the background.
3.  **Elevation:** A single, soft shadow style is used for interactive or floating elements. Shadows should be highly diffused: `0px 4px 12px rgba(0, 0, 0, 0.05)`. 

Avoid heavy borders or deep shadows. Depth is used only to separate the "notification" from the "canvas."

## Shapes

The shape language is friendly and modern, utilizing **Soft Rounded Corners**. 

Standard components like cards and input fields use a **1rem (16px)** corner radius to create a distinct, approachable look that feels comfortable on mobile devices. Smaller elements like buttons or tags may scale down to 8px, but the primary container identity is defined by the 16px radius.

## Components

### Notifications & Cards
The primary component. Each card must feature a 16px corner radius and a 2px left-hand accent border corresponding to the state color (e.g., Emerald for success). Icons should be placed in the top left to allow for immediate color/glyph recognition.

### Buttons
Primary buttons use the Cobalt Blue background with white text. Ghost buttons are used for secondary actions to maintain hierarchy. All buttons feature a 12px-16px corner radius to match the container language.

### Chips & Tags
Used for categories or status labels. These should use a subtle, desaturated version of the state color as a background (e.g., 10% opacity Emerald) with the full-strength color for the text.

### Input Fields
Inputs should be clean, using a 1px border in a light gray (`#E5E7EB`). When focused, the border shifts to the Cobalt Blue (Primary) with a subtle glow.

### Status Indicators
Small circular "pills" used within lists. These are purely color-driven to provide a quick heat-map of system health without requiring text labels in tight spaces.