---
name: Kinetic Community
colors:
  surface: '#f3faff'
  surface-dim: '#c7dde9'
  surface-bright: '#f3faff'
  surface-container-lowest: '#ffffff'
  surface-container-low: '#e6f6ff'
  surface-container: '#dbf1fe'
  surface-container-high: '#d5ecf8'
  surface-container-highest: '#cfe6f2'
  on-surface: '#071e27'
  on-surface-variant: '#3f4a3c'
  inverse-surface: '#1e333c'
  inverse-on-surface: '#dff4ff'
  outline: '#6f7a6b'
  outline-variant: '#becab9'
  surface-tint: '#006e1c'
  primary: '#006e1c'
  on-primary: '#ffffff'
  primary-container: '#4caf50'
  on-primary-container: '#003c0b'
  inverse-primary: '#78dc77'
  secondary: '#0061a4'
  on-secondary: '#ffffff'
  secondary-container: '#33a0fd'
  on-secondary-container: '#00355c'
  tertiary: '#a63360'
  on-tertiary: '#ffffff'
  tertiary-container: '#f26f9d'
  on-tertiary-container: '#690034'
  error: '#ba1a1a'
  on-error: '#ffffff'
  error-container: '#ffdad6'
  on-error-container: '#93000a'
  primary-fixed: '#94f990'
  primary-fixed-dim: '#78dc77'
  on-primary-fixed: '#002204'
  on-primary-fixed-variant: '#005313'
  secondary-fixed: '#d1e4ff'
  secondary-fixed-dim: '#9ecaff'
  on-secondary-fixed: '#001d36'
  on-secondary-fixed-variant: '#00497d'
  tertiary-fixed: '#ffd9e2'
  tertiary-fixed-dim: '#ffb1c7'
  on-tertiary-fixed: '#3e001c'
  on-tertiary-fixed-variant: '#861948'
  background: '#f3faff'
  on-background: '#071e27'
  surface-variant: '#cfe6f2'
typography:
  headline-xl:
    fontFamily: Inter
    fontSize: 40px
    fontWeight: '700'
    lineHeight: 48px
    letterSpacing: -0.02em
  headline-lg:
    fontFamily: Inter
    fontSize: 32px
    fontWeight: '700'
    lineHeight: 40px
    letterSpacing: -0.01em
  headline-lg-mobile:
    fontFamily: Inter
    fontSize: 28px
    fontWeight: '700'
    lineHeight: 36px
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
  label-md:
    fontFamily: Inter
    fontSize: 14px
    fontWeight: '600'
    lineHeight: 20px
    letterSpacing: 0.05em
  caption:
    fontFamily: Inter
    fontSize: 12px
    fontWeight: '400'
    lineHeight: 16px
rounded:
  sm: 0.25rem
  DEFAULT: 0.5rem
  md: 0.75rem
  lg: 1rem
  xl: 1.5rem
  full: 9999px
spacing:
  base: 8px
  xs: 4px
  sm: 12px
  md: 24px
  lg: 48px
  xl: 80px
  container-max: 1200px
  gutter: 24px
---

## Brand & Style

The design system is anchored in the concept of "Active Empathy." It balances the high-energy urgency of volunteer mobilization with the steady, reliable presence of a professional institution. The aesthetic is **Modern Corporate with a Humanist Touch**, prioritizing clarity, accessibility, and warmth.

The target audience ranges from Gen Z students seeking impact to retirees offering mentorship. Consequently, the UI must feel technologically current yet inherently intuitive. We utilize generous whitespace to reduce cognitive load and a "soft-surface" approach to make the digital environment feel welcoming and safe. The emotional response should be one of empowerment—moving the user from "I want to help" to "I am making a difference" with zero friction.

## Colors

The palette is functional and psychologically grounded. 

*   **Action Green (#4CAF50):** Used exclusively for primary calls-to-action and success states. It signals growth and the "go" signal for mobilization.
*   **Trust Blue (#2196F3):** Used for secondary actions, information links, and navigation accents. It provides a stabilizing, professional counterpoint to the vibrant green.
*   **Surface Neutrals:** The background uses a cool-toned light gray (#F5F7FA) to reduce eye strain compared to pure white, while maintaining a "clean slate" feel. 
*   **Typography & Grays:** We use a deep Slate Gray (#455A64) for body text rather than pure black to maintain the friendly, approachable tone while ensuring high contrast for accessibility.

## Typography

This design system utilizes **Inter** for all roles to leverage its exceptional legibility and systematic weight distribution. 

The hierarchy is built on a "Mobile-First Scaling" logic. Headlines use a tighter letter-spacing and heavier weights to appear grounded and authoritative. Body text uses a generous line-height (1.5x) to ensure long-form descriptions of volunteer opportunities are easily digestible. Use `label-md` specifically for category tags and small button text to create a distinct visual texture compared to standard body prose.

## Layout & Spacing

The layout follows a **Fluid-Fixed Hybrid** model. On desktop, content is contained within a 1200px central column to prevent line lengths from becoming unreadable. On mobile and tablet, the system shifts to a fluid fluid grid with 24px side margins.

We utilize an 8px baseline grid to ensure mathematical harmony between elements. "Generous Whitespace" is a core principle here: use `lg` (48px) or `xl` (80px) vertical padding between major sections to allow the UI to "breathe," signaling to the user that the platform is organized and calm.

## Elevation & Depth

Visual hierarchy is established through **Ambient Shadows** and **Tonal Layering**. 

*   **Level 0 (Background):** #F5F7FA. All page content sits here.
*   **Level 1 (Cards/Surface):** Pure White (#FFFFFF). These elements use a very soft, diffused shadow: `box-shadow: 0 4px 20px rgba(0, 0, 0, 0.05)`.
*   **Level 2 (Interactive/Floating):** Used for dropdowns and active cards. The shadow becomes slightly deeper: `box-shadow: 0 8px 30px rgba(0, 0, 0, 0.08)`.

Avoid harsh borders. Instead, use thin, 1px strokes in a slightly darker neutral (#E1E8ED) only when necessary to separate adjacent white elements.

## Shapes

The shape language is defined by **Soft Geometricism**. A standard corner radius of **12px** (0.75rem) is applied to buttons, input fields, and cards to reinforce the friendly and approachable brand personality.

*   **Small Components (Chips/Tags):** Use a full pill-shape (circular ends) to distinguish them from interactive buttons.
*   **Large Components (Modals/Hero Images):** Increase the radius to 24px to emphasize the "soft container" feel.

## Components

### Buttons
*   **Primary:** Background: Action Green; Text: White; Shadow: Subtle green tint on hover.
*   **Secondary:** Background: Transparent; Border: 2px Trust Blue; Text: Trust Blue.
*   **Ghost:** Text: Trust Blue; No border; Background becomes very light blue on hover.

### Cards
Cards are the primary container for volunteer "Opportunities." They must always feature a 12px border radius, a white background, and the Level 1 Ambient Shadow. Padding inside cards should be `md` (24px) to maintain the airy feel.

### Input Fields
Inputs use a light gray background (#ECEFF1) with no border in their default state. Upon focus, they transition to a white background with a 2px Trust Blue border and a soft blue outer glow.

### Chips & Badges
Used for skills (e.g., "Gardening," "Coding"). These should be pill-shaped with a low-opacity background of the secondary color (Trust Blue at 10% opacity) and dark blue text.

### Progress Indicators
For community goals, use a thick (8px) rounded progress bar using Action Green for the fill and a light neutral for the track. This reinforces the "growth" narrative.