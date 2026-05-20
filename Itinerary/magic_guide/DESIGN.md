---
name: Magic Guide
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
  on-surface-variant: '#5e3f3a'
  inverse-surface: '#2e3132'
  inverse-on-surface: '#f0f1f2'
  outline: '#936e69'
  outline-variant: '#e8bdb6'
  surface-tint: '#c00000'
  primary: '#a20000'
  on-primary: '#ffffff'
  primary-container: '#d00000'
  on-primary-container: '#ffded9'
  inverse-primary: '#ffb4a8'
  secondary: '#2559bf'
  on-secondary: '#ffffff'
  secondary-container: '#6995ff'
  on-secondary-container: '#002c73'
  tertiary: '#654a00'
  on-tertiary: '#ffffff'
  tertiary-container: '#836100'
  on-tertiary-container: '#ffe2a9'
  error: '#ba1a1a'
  on-error: '#ffffff'
  error-container: '#ffdad6'
  on-error-container: '#93000a'
  primary-fixed: '#ffdad4'
  primary-fixed-dim: '#ffb4a8'
  on-primary-fixed: '#410000'
  on-primary-fixed-variant: '#930000'
  secondary-fixed: '#dae2ff'
  secondary-fixed-dim: '#b2c5ff'
  on-secondary-fixed: '#001847'
  on-secondary-fixed-variant: '#0040a0'
  tertiary-fixed: '#ffdf9e'
  tertiary-fixed-dim: '#fabd00'
  on-tertiary-fixed: '#261a00'
  on-tertiary-fixed-variant: '#5b4300'
  background: '#f8f9fa'
  on-background: '#191c1d'
  surface-variant: '#e1e3e4'
typography:
  headline-lg:
    fontFamily: Plus Jakarta Sans
    fontSize: 32px
    fontWeight: '700'
    lineHeight: 40px
    letterSpacing: -0.02em
  headline-lg-mobile:
    fontFamily: Plus Jakarta Sans
    fontSize: 26px
    fontWeight: '700'
    lineHeight: 32px
    letterSpacing: -0.01em
  headline-md:
    fontFamily: Plus Jakarta Sans
    fontSize: 24px
    fontWeight: '600'
    lineHeight: 30px
  headline-sm:
    fontFamily: Plus Jakarta Sans
    fontSize: 20px
    fontWeight: '600'
    lineHeight: 26px
  body-lg:
    fontFamily: Montserrat
    fontSize: 16px
    fontWeight: '400'
    lineHeight: 24px
  body-md:
    fontFamily: Montserrat
    fontSize: 14px
    fontWeight: '400'
    lineHeight: 20px
  label-md:
    fontFamily: Montserrat
    fontSize: 12px
    fontWeight: '600'
    lineHeight: 16px
    letterSpacing: 0.05em
  button:
    fontFamily: Montserrat
    fontSize: 16px
    fontWeight: '700'
    lineHeight: 20px
rounded:
  sm: 0.25rem
  DEFAULT: 0.5rem
  md: 0.75rem
  lg: 1rem
  xl: 1.5rem
  full: 9999px
spacing:
  base: 8px
  container-padding: 20px
  stack-gap: 16px
  inline-gap: 12px
  section-margin: 32px
---

## Brand & Style

The design system is built to evoke the wonder and excitement of a theme park visit while maintaining the rigorous organization required for a complex itinerary. The brand personality is **magical, spirited, and dependable**. It bridges the gap between high-energy entertainment and a high-utility travel tool.

The visual style is a hybrid of **Modern Minimalism** and **Tactile Playfulness**. We utilize clean, white space to prevent information overload, while introducing "magical" moments through vibrant color accents, soft geometry, and subtle motion. The interface should feel like a premium concierge service that hasn't forgotten how to have fun.

## Colors

The palette is rooted in iconic park imagery. **Mickey Red** serves as our primary action color, used for high-priority buttons and critical alerts. **Magic Blue** provides a calming, professional foundation for secondary actions and navigation elements.

**Golden Yellow** and **Castle Lavender** are used sparingly as celebratory accents—marking completed tasks, special "hidden gems," or premium features. Backgrounds should remain a crisp, clean white or very light gray (#F8F9FA) to ensure the vibrant primary colors pop without causing visual fatigue.

## Typography

This design system uses a dual-type approach to balance personality with legibility. **Plus Jakarta Sans** is utilized for headlines; its soft, rounded terminals provide a friendly and approachable "storytelling" feel.

**Montserrat** is used for all functional UI text, body copy, and labels. Its geometric precision ensures high readability during outdoor use (high-glare environments) while maintaining a modern, energetic tone. Use tight letter-spacing for large headlines and generous tracking for small uppercase labels to improve scanability.

## Layout & Spacing

The design system employs a **Fluid Grid** model optimized for mobile-first interaction. We use an 8px base unit to maintain a consistent rhythmic scale.

- **Margins:** A standard 20px safe area is maintained on the left and right edges of the screen.
- **Card Spacing:** Elements within cards use a 12px internal padding, while the cards themselves are separated by 16px vertical gaps to create a clear "Adventure Feed."
- **Touch Targets:** All interactive elements (buttons, checkboxes) must maintain a minimum height of 48px to accommodate users on the move.

## Elevation & Depth

To create an organized yet whimsical feel, the design system utilizes **Ambient Shadows** and **Tonal Layering**. 

Cards should appear slightly "lifted" off the white background using a soft, diffused shadow (Blur: 15px, Y: 4px, Opacity: 8%) tinted slightly with Magic Blue to avoid a "muddy" gray look. This creates a clear physical metaphor for items that can be tapped or swiped. Interactive elements like "Book Now" buttons use a slightly deeper shadow on press to provide tactile feedback, mimicking a physical button being pushed.

## Shapes

The shape language is defined by **Rounded** geometry. There are no sharp corners in this design system, as sharp angles conflict with the "friendly and safe" brand promise of a family-centric app.

- **Standard Elements:** Buttons and input fields use a 0.5rem (8px) radius.
- **Containers:** Large info cards and modals use 1rem (16px) radius to feel like approachable, soft objects.
- **Icons:** Use a consistent 2px stroke weight with rounded caps and joins to match the typography.

## Components

### Buttons
Primary buttons are pill-shaped or heavily rounded, using the Mickey Red background with white text. For "Magical Actions" (like viewing a photo pass), use a gradient transition from Magic Blue to Castle Lavender.

### Cards
"Adventure Cards" are the primary vessel for information. They feature a white background, soft shadow, and a subtle 1px border (#E0E0E0). If a card represents a "completed" attraction, the border transitions to Magic Blue.

### Checkboxes & Progress
Checkboxes for "To-Do" lists should be oversized (24x24px). When checked, they trigger a brief "sparkle" animation using Golden Yellow star motifs. Progress bars are thick (8px) with a rounded Magic Blue fill and a "sparkle" icon that travels at the tip of the progress indicator.

### Input Fields
Fields should have a light neutral background (#F1F3F5) and transition to a Magic Blue border when focused. Placeholder text should be friendly and conversational (e.g., "Where to next, Explorer?").

### Chips & Tags
Use chips for ride categories (e.g., "Thrill," "Slow Ride"). These should use desaturated versions of the accent colors (e.g., pale lavender) with dark text to maintain accessibility while adding a splash of color.