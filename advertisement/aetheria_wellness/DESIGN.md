---
name: Aetheria Wellness
colors:
  surface: '#faf9f7'
  surface-dim: '#dadad8'
  surface-bright: '#faf9f7'
  surface-container-lowest: '#ffffff'
  surface-container-low: '#f4f3f1'
  surface-container: '#efeeec'
  surface-container-high: '#e9e8e6'
  surface-container-highest: '#e3e2e0'
  on-surface: '#1a1c1b'
  on-surface-variant: '#434843'
  inverse-surface: '#2f3130'
  inverse-on-surface: '#f1f1ef'
  outline: '#737973'
  outline-variant: '#c3c8c1'
  surface-tint: '#4d6453'
  primary: '#061b0e'
  on-primary: '#ffffff'
  primary-container: '#1b3022'
  on-primary-container: '#819986'
  inverse-primary: '#b4cdb8'
  secondary: '#566252'
  on-secondary: '#ffffff'
  secondary-container: '#d4e1cd'
  on-secondary-container: '#586454'
  tertiary: '#2b0f01'
  on-tertiary: '#ffffff'
  tertiary-container: '#44230e'
  on-tertiary-container: '#ba886c'
  error: '#ba1a1a'
  on-error: '#ffffff'
  error-container: '#ffdad6'
  on-error-container: '#93000a'
  primary-fixed: '#d0e9d4'
  primary-fixed-dim: '#b4cdb8'
  on-primary-fixed: '#0b2013'
  on-primary-fixed-variant: '#364c3c'
  secondary-fixed: '#d9e6d2'
  secondary-fixed-dim: '#bdcab7'
  on-secondary-fixed: '#141e12'
  on-secondary-fixed-variant: '#3e4a3b'
  tertiary-fixed: '#ffdbc9'
  tertiary-fixed-dim: '#f3ba9c'
  on-tertiary-fixed: '#311302'
  on-tertiary-fixed-variant: '#643d26'
  background: '#faf9f7'
  on-background: '#1a1c1b'
  surface-variant: '#e3e2e0'
typography:
  display-lg:
    fontFamily: ebGaramond
    fontSize: 48px
    fontWeight: '500'
    lineHeight: '1.1'
    letterSpacing: -0.02em
  display-lg-mobile:
    fontFamily: ebGaramond
    fontSize: 36px
    fontWeight: '500'
    lineHeight: '1.2'
    letterSpacing: -0.01em
  headline-md:
    fontFamily: ebGaramond
    fontSize: 32px
    fontWeight: '500'
    lineHeight: '1.2'
  headline-sm:
    fontFamily: ebGaramond
    fontSize: 24px
    fontWeight: '500'
    lineHeight: '1.3'
  body-lg:
    fontFamily: manrope
    fontSize: 18px
    fontWeight: '400'
    lineHeight: '1.6'
  body-md:
    fontFamily: manrope
    fontSize: 16px
    fontWeight: '400'
    lineHeight: '1.6'
  label-md:
    fontFamily: manrope
    fontSize: 14px
    fontWeight: '600'
    lineHeight: '1.2'
    letterSpacing: 0.05em
  label-sm:
    fontFamily: manrope
    fontSize: 12px
    fontWeight: '500'
    lineHeight: '1.2'
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
  xl: 80px
  container-max: 1200px
  gutter: 24px
---

## Brand & Style

The design system is anchored in the concept of "Quiet Strength." It prioritizes mental clarity and physical restoration over the aggressive, high-intensity aesthetics typical of the fitness industry. The target audience seeks a holistic approach to wellness—integrating mindfulness, movement, and recovery into a premium lifestyle.

The visual style is **Minimalist with Tactile warmth**. It leverages significant whitespace (negative space) to reduce cognitive load, allowing the user to focus on their progress without distraction. Borrowing from high-end editorial design, the system uses large, evocative imagery paired with sophisticated typography. The interface should feel like a sanctuary: breathable, balanced, and intentional.

## Colors

The palette is derived from natural elements to evoke grounding and tranquility. 

- **Primary (Deep Forest Green):** Used for primary actions, navigation backgrounds, and high-level headings. It represents stability and growth.
- **Secondary (Soft Sage):** Used for subtle backgrounds, secondary buttons, and success states. It provides a calming contrast to the deep forest green.
- **Tertiary (Warm Clay):** An accent color used sparingly for progress indicators, call-to-outs, and active states. It adds a human, earth-bound warmth to the cooler greens.
- **Neutral (Off-White):** The primary canvas color. Avoid pure white (#FFFFFF) to reduce eye strain and maintain a soft, premium feel.
- **Text:** Main body text utilizes a deep, desaturated charcoal with green undertones to maintain harmony with the palette.

## Typography

This design system employs a sophisticated serif-sans pairing to balance tradition with modernity.

- **Headings (ebGaramond):** These should be treated with editorial care. Use `display-lg` for hero sections and mindful quotes. The classic proportions of the serif font evoke a sense of timelessness and wisdom.
- **Body & UI (manrope):** A highly legible, modern sans-serif. It handles data-heavy sections like workout stats or nutritional info with professional clarity.
- **Labels:** Use uppercase for small labels to create a clear hierarchy and a sense of organized structure.

## Layout & Spacing

The layout philosophy is **Spacious and Unconstrained**. 

- **Grid:** A 12-column fixed grid for desktop (centered, max-width 1200px) and a fluid 4-column grid for mobile.
- **Rhythm:** Use the `lg` (48px) and `xl` (80px) spacing units to separate major sections. This "breathable" approach prevents the UI from feeling cluttered, reinforcing the brand's tranquil nature.
- **Padding:** Content containers should use generous internal padding (`md` or `lg`) to ensure elements never feel cramped against their borders.

## Elevation & Depth

To maintain a minimalist and high-end aesthetic, this design system avoids heavy drop shadows. Depth is communicated through **Tonal Layering** and **Soft Ambient Occlusion**:

- **Surface Tiers:** Use subtle shifts in background color (e.g., Off-white to a very pale Sage) to define nested content.
- **Shadows:** When necessary (such as for floating action buttons or elevated cards), use extremely diffused, low-opacity shadows (#1B3022 at 5-8% opacity) with a large blur radius (20px+).
- **Outlines:** Use thin (1px) borders in a slightly darker shade of the background color for cards, rather than shadows, to maintain a "flat-plus" look.

## Shapes

The shape language is **Soft and Organic**. 

We avoid sharp, aggressive corners in favor of gentle radii that feel approachable and safe. 
- **Standard UI elements:** (Buttons, Inputs) use a `0.25rem` radius for a professional, "soft-square" look.
- **Feature Cards & Large Containers:** Use `rounded-lg` (0.5rem) to create a distinct, modern container feel.
- **Interactive Pill Elements:** Chips and progress bars should use fully rounded (pill-shaped) ends to emphasize fluidity and movement.

## Components

- **Buttons:** Primary buttons are solid Deep Forest Green with Off-white text. Secondary buttons use a Sage outline or clear background. All buttons should have generous horizontal padding (min 24px) to feel substantial yet elegant.
- **Inputs:** Form fields should be minimalist, using only a bottom border or a very light Sage background. Active states are indicated by the Deep Forest Green border and the Warm Clay cursor/caret.
- **Cards:** Cards are used to group related content like "Daily Mindfulness" or "Yoga Flow." They should feature high-quality imagery with an overlay of ebGaramond text.
- **Chips:** Used for tags (e.g., "15 min," "Restorative," "Intermediate"). These are pill-shaped with a light Sage background and Deep Forest Green text.
- **Progress Indicators:** Use the Warm Clay color for progress bars and rings. The warmth of the clay against the cool greens creates a clear visual focus on the user's personal growth.
- **Lists:** Clean, spacious lists with thin Soft Sage dividers. Use manrope for list items to ensure high legibility during movement.