---
name: Vivid Velocity
colors:
  surface: '#131313'
  surface-dim: '#131313'
  surface-bright: '#3a3939'
  surface-container-lowest: '#0e0e0e'
  surface-container-low: '#1c1b1b'
  surface-container: '#201f1f'
  surface-container-high: '#2a2a2a'
  surface-container-highest: '#353534'
  on-surface: '#e5e2e1'
  on-surface-variant: '#c2caad'
  inverse-surface: '#e5e2e1'
  inverse-on-surface: '#313030'
  outline: '#8c9479'
  outline-variant: '#434933'
  surface-tint: '#a0d800'
  primary: '#ffffff'
  on-primary: '#253600'
  primary-container: '#b7f700'
  on-primary-container: '#506e00'
  inverse-primary: '#4b6700'
  secondary: '#dcb8ff'
  on-secondary: '#480081'
  secondary-container: '#7701d0'
  on-secondary-container: '#dcb7ff'
  tertiary: '#ffffff'
  on-tertiary: '#313030'
  tertiary-container: '#e5e2e1'
  on-tertiary-container: '#656464'
  error: '#ffb4ab'
  on-error: '#690005'
  error-container: '#93000a'
  on-error-container: '#ffdad6'
  primary-fixed: '#b7f700'
  primary-fixed-dim: '#a0d800'
  on-primary-fixed: '#141f00'
  on-primary-fixed-variant: '#374e00'
  secondary-fixed: '#efdbff'
  secondary-fixed-dim: '#dcb8ff'
  on-secondary-fixed: '#2c0051'
  on-secondary-fixed-variant: '#6700b5'
  tertiary-fixed: '#e5e2e1'
  tertiary-fixed-dim: '#c8c6c5'
  on-tertiary-fixed: '#1c1b1b'
  on-tertiary-fixed-variant: '#474746'
  background: '#131313'
  on-background: '#e5e2e1'
  surface-variant: '#353534'
typography:
  display-lg:
    fontFamily: Anybody
    fontSize: 72px
    fontWeight: '800'
    lineHeight: '1.1'
    letterSpacing: -0.04em
  headline-lg:
    fontFamily: Anybody
    fontSize: 48px
    fontWeight: '700'
    lineHeight: '1.2'
    letterSpacing: -0.02em
  headline-lg-mobile:
    fontFamily: Anybody
    fontSize: 32px
    fontWeight: '700'
    lineHeight: '1.2'
    letterSpacing: -0.02em
  headline-md:
    fontFamily: Anybody
    fontSize: 24px
    fontWeight: '600'
    lineHeight: '1.3'
  body-lg:
    fontFamily: Plus Jakarta Sans
    fontSize: 18px
    fontWeight: '400'
    lineHeight: '1.6'
  body-md:
    fontFamily: Plus Jakarta Sans
    fontSize: 16px
    fontWeight: '400'
    lineHeight: '1.6'
  label-sm:
    fontFamily: Geist
    fontSize: 12px
    fontWeight: '600'
    lineHeight: '1'
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
  gutter: 24px
  margin-mobile: 16px
  margin-desktop: 64px
  container-max: 1280px
---

## Brand & Style
The design system is engineered for a high-energy giveaway platform that balances the adrenaline of "winning" with the sophistication of a premium service. The brand personality is electric, urgent, and rewarding, designed to evoke a sense of immediate possibility and exclusive access.

The design style is **High-Contrast Modern**, utilizing a deep, obsidian-like neutral base to make vibrant accent colors "pop" with neon-like intensity. We employ elements of **Glassmorphism** for secondary surfaces to maintain a sense of depth and modern tech-forwardness, while bold, oversized typography ensures that the value proposition—the prize—is never missed. The emotional response should be a mix of excitement (the win) and trust (the platform's premium nature).

## Colors
The palette is dominated by a high-contrast dark mode to create a premium, "nightlife" or "gaming" excitement. 

- **Primary (Electric Lime):** Used for primary calls to action, winner announcements, and critical "Enter Now" triggers. It demands attention against the dark backdrop.
- **Secondary (Vivid Violet):** Used for progressive bars, secondary accents, and premium tier signifiers. It adds a sophisticated, mysterious depth to the high-energy lime.
- **Neutral/Background:** The "Obsidian" base (#0F0F0F) provides a matte, low-glare surface that allows the vibrant colors to glow.
- **Surface:** Layered containers use #1A1A1A to create subtle separation from the background.

## Typography
The typography strategy uses **Anybody** for headlines to leverage its variable weight and width, creating an aggressive, high-impact editorial feel. It should be used in "ExtraBold" or "Black" weights for prize amounts and countdowns.

**Plus Jakarta Sans** provides a friendly, approachable counter-balance for body copy, ensuring the terms and conditions or product descriptions remain legible and inviting. **Geist** is reserved for technical labels, metadata, and mono-spaced utility text (like "Entries: 4,500"), providing a precise, developer-grade finish to the UI.

## Layout & Spacing
This design system utilizes a **12-column fluid grid** for desktop and a **4-column grid** for mobile. The spacing rhythm is strictly based on an 8px scale to maintain visual mathematical harmony.

Large "Hero" sections for featured giveaways should use aggressive internal padding (80px+) to create a sense of scale and importance. Content cards should utilize a consistent 24px gutter to prevent the interface from feeling cluttered, despite the bold colors and type.

## Elevation & Depth
Depth is created through **Tonal Layering** rather than traditional shadows.
- **Level 0 (Base):** #0F0F0F.
- **Level 1 (Cards/Sections):** #1A1A1A with a subtle 1px border (#2A2A2A).
- **Level 2 (Popovers/Overlays):** Glassmorphism effect—Backdrop blur (20px) with a semi-transparent fill (rgba(26, 26, 26, 0.7)).

For interactive elements like primary buttons, a "Glow" effect is used: a soft, 20px blur of the Primary color at 30% opacity, simulating a light source emitting from the button.

## Shapes
The shape language is **Rounded (0.5rem base)**. This softens the aggressive nature of the high-contrast colors and bold typography, making the platform feel like a friendly, modern app rather than a harsh gambling site. 

Large containers and cards should use `rounded-xl` (1.5rem) to create a "containerized" feel that looks intentional and premium. Buttons should strictly follow the `rounded-lg` (1rem) standard for a tactile, pill-adjacent appearance.

## Components
- **Buttons:** Primary buttons use the Primary Color (Lime) with black text. On hover, they should scale 5% and increase their outer glow. Secondary buttons are ghost-style with a 2px Violet border.
- **Giveaway Cards:** Featured giveaways use a full-bleed image background with a gradient overlay (Bottom to Top: #0F0F0F to Transparent). The prize title is set in `headline-lg`.
- **Progress Bars:** For "Limited Time" or "Entries Remaining," use a Secondary Color (Violet) track with a Primary Color (Lime) fill to show progress/urgency.
- **Input Fields:** Dark fills (#1A1A1A) with 1px borders that glow Primary Color when focused. 
- **Chips/Badges:** Small, high-contrast pills (e.g., "LIVE" in Red, "ENDING SOON" in Lime) using `label-sm` Geist typography.
- **Timer Components:** Large, monospaced (Geist) numbers to emphasize the urgency of the countdown.