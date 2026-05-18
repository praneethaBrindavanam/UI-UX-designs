---
name: Luminous Gratitude
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
  on-surface-variant: '#3c4a46'
  inverse-surface: '#263143'
  inverse-on-surface: '#ecf1ff'
  outline: '#6b7a76'
  outline-variant: '#bacac5'
  surface-tint: '#006b5f'
  primary: '#006b5f'
  on-primary: '#ffffff'
  primary-container: '#2dd4bf'
  on-primary-container: '#00574d'
  inverse-primary: '#3cddc7'
  secondary: '#795900'
  on-secondary: '#ffffff'
  secondary-container: '#ffc329'
  on-secondary-container: '#6f5100'
  tertiary: '#0060ac'
  on-tertiary: '#ffffff'
  tertiary-container: '#94c0ff'
  on-tertiary-container: '#004e8d'
  error: '#ba1a1a'
  on-error: '#ffffff'
  error-container: '#ffdad6'
  on-error-container: '#93000a'
  primary-fixed: '#62fae3'
  primary-fixed-dim: '#3cddc7'
  on-primary-fixed: '#00201c'
  on-primary-fixed-variant: '#005047'
  secondary-fixed: '#ffdf9f'
  secondary-fixed-dim: '#f9bd22'
  on-secondary-fixed: '#261a00'
  on-secondary-fixed-variant: '#5c4300'
  tertiary-fixed: '#d4e3ff'
  tertiary-fixed-dim: '#a4c9ff'
  on-tertiary-fixed: '#001c39'
  on-tertiary-fixed-variant: '#004883'
  background: '#f9f9ff'
  on-background: '#111c2d'
  surface-variant: '#d8e3fb'
typography:
  display:
    fontFamily: Plus Jakarta Sans
    fontSize: 48px
    fontWeight: '800'
    lineHeight: '1.1'
    letterSpacing: -0.02em
  display-mobile:
    fontFamily: Plus Jakarta Sans
    fontSize: 36px
    fontWeight: '800'
    lineHeight: '1.2'
  headline-lg:
    fontFamily: Plus Jakarta Sans
    fontSize: 32px
    fontWeight: '700'
    lineHeight: '1.2'
  headline-md:
    fontFamily: Plus Jakarta Sans
    fontSize: 24px
    fontWeight: '700'
    lineHeight: '1.3'
  body-lg:
    fontFamily: Quicksand
    fontSize: 20px
    fontWeight: '500'
    lineHeight: '1.6'
  body-md:
    fontFamily: Quicksand
    fontSize: 16px
    fontWeight: '500'
    lineHeight: '1.6'
  label-md:
    fontFamily: Plus Jakarta Sans
    fontSize: 14px
    fontWeight: '600'
    lineHeight: '1.4'
    letterSpacing: 0.05em
rounded:
  sm: 0.25rem
  DEFAULT: 0.5rem
  md: 0.75rem
  lg: 1rem
  xl: 1.5rem
  full: 9999px
spacing:
  base: 8px
  section-gap: 80px
  container-max: 1200px
  gutter: 24px
  margin-mobile: 20px
---

## Brand & Style
The design system is centered on the "Peak-End Rule," ensuring the final interaction a user has with a service—the "Thank You" moment—is the most memorable and positive. The brand personality is **exuberant, sincere, and effortless**. It avoids the sterile corporate aesthetic in favor of a **Warm Minimalism** that combines vast whitespace with playful, high-energy accents.

The visual style utilizes soft-edged geometry and a "breathable" layout to reduce cognitive load while evoking an emotional response of relief and appreciation. It leverages a modern, clean execution with subtle tactile touches to make the digital experience feel human and approachable.

## Colors
The palette is a "Vibrant Pastel" scheme designed to feel sunny and optimistic without straining the eyes.
- **Primary (Mint):** Used for success states and primary confirmation actions. It symbolizes growth and harmony.
- **Secondary (Sunny Yellow):** Reserved for "delight" moments, such as star icons, badges, or celebratory illustrations.
- **Tertiary (Soft Blue):** Used for secondary pathways or informational links to provide a grounding, calm contrast.
- **Neutral (Slate):** A deep, high-contrast navy is used for typography instead of pure black to maintain a premium, soft feel while ensuring WCAG AA accessibility.

## Typography
This design system employs a dual-typeface strategy to balance professional modernism with friendly charm. 

**Plus Jakarta Sans** is used for headings and labels. Its slightly wider stance and modern curves provide a confident, "open" feeling. **Quicksand** is used for all body and descriptive text; its rounded terminals reinforce the "cheerful" brand personality and make long-form gratitude messages feel like a personal note. 

Hierarchy is established through significant size stepping and the use of "ExtraBold" for primary headlines to create a strong visual anchor on the page.

## Layout & Spacing
The layout follows a **Fluid Centralized Model**. Content is primarily centered to create a sense of focus and celebration. 

- **Grid:** A 12-column grid is used for desktop, but most "Thank You" modules should occupy the central 6-8 columns to maintain white space.
- **Rhythm:** An 8px linear scale governs all padding and margins. 
- **Sectioning:** Large vertical gaps (80px+) are encouraged between the primary "Thank You" message and secondary "Next Steps" to prevent the user from feeling rushed.
- **Mobile:** On mobile, margins shrink to 20px, and elements stack vertically, maintaining the center-alignment for the primary hero icon and text.

## Elevation & Depth
Depth is created through **Tonal Layering** rather than heavy shadows. 
- **The Base:** The page background uses a very subtle off-white or tinted mint.
- **Surface Level:** Cards and containers use pure white (#FFFFFF) to "pop" forward.
- **Soft Depth:** Instead of standard grey shadows, use "Ambient Glows"—shadows with a 24px-40px blur, low opacity (10%), and a hint of the primary mint color. This makes elements feel like they are floating on a cushion of light rather than casting a heavy shadow.
- **Interactive Depth:** Buttons should use a slight 2px vertical offset on hover to simulate being "pressed" into a soft surface.

## Shapes
The shape language is **distinctly organic**. Sharp corners are strictly avoided to maintain the "friendly" and "safe" emotional tone. 
- **Standard Radius:** 0.5rem (8px) for small components like inputs.
- **Large Radius:** 1.5rem (24px) for cards and main containers.
- **Pill Shapes:** Used for all primary buttons and tags to emphasize the playful, approachable nature.
- **Illustrative Elements:** Any background decorations or blobs should use "squircle" or organic, non-geometric paths.

## Components
### Buttons
Primary buttons are pill-shaped, using the Primary Mint color with high-contrast Slate text. Hover states should involve a subtle scale-up (1.02x) rather than just a color change to feel more "bouncy" and responsive.

### Cards
Cards are the primary container for "What's Next" actions (e.g., "Back to Home", "Share on Social"). They feature a 24px corner radius, a 1px soft border (Mint-100), and the "Ambient Glow" shadow.

### Playful Illustrations
Every "Thank You" page should feature a hero illustration or animated Lottie file. These should be stylized, using the brand palette, featuring exaggerated proportions and "bouncy" physics.

### Feedback Toasts
If a user performs an action on the page (like copying a referral code), toasts should appear at the top-center, using the Secondary Yellow background to draw attention in a cheerful way.

### Input Fields
Used occasionally for "Join our Newsletter" on the thank you page. Inputs should have a thick 2px border that turns Primary Mint on focus, with the Quicksand typeface for placeholder text.