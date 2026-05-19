---
name: Midnight Tech
colors:
  surface: '#0c1324'
  surface-dim: '#0c1324'
  surface-bright: '#33394c'
  surface-container-lowest: '#070d1f'
  surface-container-low: '#151b2d'
  surface-container: '#191f31'
  surface-container-high: '#23293c'
  surface-container-highest: '#2e3447'
  on-surface: '#dce1fb'
  on-surface-variant: '#c7c4d8'
  inverse-surface: '#dce1fb'
  inverse-on-surface: '#2a3043'
  outline: '#918fa1'
  outline-variant: '#464555'
  surface-tint: '#c3c0ff'
  primary: '#c3c0ff'
  on-primary: '#1d00a5'
  primary-container: '#4f46e5'
  on-primary-container: '#dad7ff'
  inverse-primary: '#4d44e3'
  secondary: '#bec6e0'
  on-secondary: '#283044'
  secondary-container: '#3f465c'
  on-secondary-container: '#adb4ce'
  tertiary: '#3cd7ff'
  on-tertiary: '#003642'
  tertiary-container: '#006980'
  on-tertiary-container: '#9ce6ff'
  error: '#ffb4ab'
  on-error: '#690005'
  error-container: '#93000a'
  on-error-container: '#ffdad6'
  primary-fixed: '#e2dfff'
  primary-fixed-dim: '#c3c0ff'
  on-primary-fixed: '#0f0069'
  on-primary-fixed-variant: '#3323cc'
  secondary-fixed: '#dae2fd'
  secondary-fixed-dim: '#bec6e0'
  on-secondary-fixed: '#131b2e'
  on-secondary-fixed-variant: '#3f465c'
  tertiary-fixed: '#b4ebff'
  tertiary-fixed-dim: '#3cd7ff'
  on-tertiary-fixed: '#001f27'
  on-tertiary-fixed-variant: '#004e5f'
  background: '#0c1324'
  on-background: '#dce1fb'
  surface-variant: '#2e3447'
typography:
  display-lg:
    fontFamily: Geist
    fontSize: 72px
    fontWeight: '700'
    lineHeight: '1.1'
    letterSpacing: -0.04em
  display-lg-mobile:
    fontFamily: Geist
    fontSize: 40px
    fontWeight: '700'
    lineHeight: '1.2'
    letterSpacing: -0.02em
  headline-lg:
    fontFamily: Geist
    fontSize: 32px
    fontWeight: '600'
    lineHeight: '1.2'
  headline-md:
    fontFamily: Geist
    fontSize: 24px
    fontWeight: '600'
    lineHeight: '1.3'
  body-lg:
    fontFamily: Geist
    fontSize: 18px
    fontWeight: '400'
    lineHeight: '1.6'
  body-md:
    fontFamily: Geist
    fontSize: 16px
    fontWeight: '400'
    lineHeight: '1.6'
  label-md:
    fontFamily: JetBrains Mono
    fontSize: 14px
    fontWeight: '500'
    lineHeight: '1.2'
    letterSpacing: 0.05em
  label-sm:
    fontFamily: JetBrains Mono
    fontSize: 12px
    fontWeight: '500'
    lineHeight: '1.2'
    letterSpacing: 0.1em
rounded:
  sm: 0.125rem
  DEFAULT: 0.25rem
  md: 0.375rem
  lg: 0.5rem
  xl: 0.75rem
  full: 9999px
spacing:
  unit: 8px
  container-max: 1280px
  gutter: 24px
  margin-mobile: 16px
  margin-desktop: 64px
  section-gap: 120px
---

## Brand & Style

The design system is engineered for high-stakes product launches and exclusive technological unveilings. It targets a sophisticated, tech-forward audience that values precision, innovation, and understated luxury. 

The aesthetic is "Midnight Tech," a fusion of **Minimalism** and **Glassmorphism**. It utilizes a dark-mode-first approach to create a cinematic atmosphere. Depth is achieved through layering translucent surfaces and "internal glows" rather than traditional drop shadows. The emotional response should be one of anticipation, prestige, and seamless technical mastery. Generous whitespace (or "dark space") is used to frame hero products and key messaging, ensuring every element feels intentional and high-end.

## Colors

The palette is anchored in deep, ink-like blacks and charcoal grays to provide a "void" that allows technical details to emerge. 

- **Primary (Electric Indigo):** Used for primary actions, critical state indicators, and subtle accent glows. It provides a vibrant, high-energy contrast to the dark surroundings.
- **Secondary (Deep Slate):** Acts as the foundation for surface containers and interactive elements.
- **Tertiary (Cyan Flare):** Reserved for data visualization, secondary highlights, or active states that require a "tech-readout" feel.
- **Neutral (The Void):** A rich, slightly blue-tinted black (`#020617`) used for the base background to avoid the flatness of pure black.

Colors should be applied using low-opacity fills (10-40%) on glass surfaces to maintain the "midnight" depth.

## Typography

This design system utilizes **Geist** for its relentless precision and architectural feel. Its geometric construction aligns with the "Midnight Tech" aesthetic, appearing clean and authoritative. 

**JetBrains Mono** is introduced as a supporting label font to provide a technical, "meta-data" character to small captions, timestamps, and technical specifications. 

Large display headers should use tight tracking and bold weights to feel impactful. Body copy remains airy with a generous line height to ensure readability against dark backgrounds. All labels and captions are set in uppercase with increased letter-spacing to emphasize their role as technical annotations.

## Layout & Spacing

The design system employs a **fixed-width, centered grid** for desktop to maintain an "editorial" feel, transitioning to a fluid layout for mobile devices. 

- **The Rhythm:** Based on an 8px base unit. Spacing between major sections should be expansive (120px+) to allow the brand to breathe and evoke a premium sense of scale.
- **The Grid:** A 12-column grid is used for desktop. Components generally span 4, 6, or 8 columns to avoid visual clutter.
- **Content Alignment:** Hero content is often center-aligned to create a focal point, while technical details are left-aligned on a secondary grid for "readout" clarity.

## Elevation & Depth

Depth in this design system is conveyed through **Glassmorphism** and **Tonal Layering** rather than traditional shadows.

1.  **The Base:** The bottom-most layer is the "Neutral" black.
2.  **Glass Containers:** Secondary surfaces use a semi-transparent slate fill (approx. 40% opacity) with a high-intensity backdrop blur (20px - 40px). 
3.  **Inner Glows:** Instead of drop shadows, elevated elements use a 1px subtle inner border (top and left) in a light indigo tint to simulate a light source from above.
4.  **Ambient Indigo:** High-priority cards may feature a faint, diffused Indigo glow (`blur: 80px, opacity: 15%`) positioned behind the element to create a sense of presence.

## Shapes

The shape language is "Soft-Technical." Elements use a subtle **0.25rem (4px)** radius as the default to maintain a sharp, engineered look. Larger containers or cards may scale up to **0.75rem (12px)** for a more modern, approachable feel. 

Pill shapes are reserved exclusively for status indicators or specific "tag" components to distinguish them from interactive buttons. Sharp 0px corners should be avoided to prevent the UI from feeling dated or overly aggressive.

## Components

- **Buttons:** Primary buttons use a solid Indigo fill with white text. Secondary buttons are "ghost" style with a 1px Indigo border and a subtle glass background. Hover states should trigger a slight increase in the glow intensity.
- **Chips/Tags:** Small, JetBrains Mono labels with a subtle 10% Indigo fill. No borders.
- **Input Fields:** Darker than the background with a 1px stroke that brightens to Electric Indigo on focus. Minimalist placeholder text in medium gray.
- **Cards:** The hallmark of the system. High backdrop blur, 1px subtle stroke (`#ffffff10`), and a slight vertical gradient from top-left to bottom-right.
- **Lists:** Separated by thin, low-opacity lines (`#ffffff05`). Items have a subtle glass hover state.
- **Product Reveal Modules:** Specialized components that use "light-sweep" animations (a moving linear gradient) across the glass surface to emphasize texture and depth.