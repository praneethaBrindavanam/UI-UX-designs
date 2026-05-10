---
name: Modern Coastal
colors:
  surface: '#fbf8ff'
  surface-dim: '#d5d8f9'
  surface-bright: '#fbf8ff'
  surface-container-lowest: '#ffffff'
  surface-container-low: '#f4f2ff'
  surface-container: '#ececff'
  surface-container-high: '#e5e6ff'
  surface-container-highest: '#dee0ff'
  on-surface: '#161a32'
  on-surface-variant: '#404850'
  inverse-surface: '#2b2f48'
  inverse-on-surface: '#f0efff'
  outline: '#707881'
  outline-variant: '#bfc7d1'
  surface-tint: '#006399'
  primary: '#005d90'
  on-primary: '#ffffff'
  primary-container: '#0077b6'
  on-primary-container: '#f3f7ff'
  inverse-primary: '#94ccff'
  secondary: '#645d55'
  on-secondary: '#ffffff'
  secondary-container: '#e8ded3'
  on-secondary-container: '#686259'
  tertiary: '#57595b'
  on-tertiary: '#ffffff'
  tertiary-container: '#707273'
  on-tertiary-container: '#f7f8f9'
  error: '#ba1a1a'
  on-error: '#ffffff'
  error-container: '#ffdad6'
  on-error-container: '#93000a'
  primary-fixed: '#cde5ff'
  primary-fixed-dim: '#94ccff'
  on-primary-fixed: '#001d32'
  on-primary-fixed-variant: '#004b74'
  secondary-fixed: '#ebe1d6'
  secondary-fixed-dim: '#cec5ba'
  on-secondary-fixed: '#1f1b14'
  on-secondary-fixed-variant: '#4c463e'
  tertiary-fixed: '#e1e3e4'
  tertiary-fixed-dim: '#c5c7c8'
  on-tertiary-fixed: '#191c1d'
  on-tertiary-fixed-variant: '#454748'
  background: '#fbf8ff'
  on-background: '#161a32'
  surface-variant: '#dee0ff'
typography:
  display-lg:
    fontFamily: Playfair Display
    fontSize: 48px
    fontWeight: '700'
    lineHeight: 56px
    letterSpacing: -0.02em
  display-lg-mobile:
    fontFamily: Playfair Display
    fontSize: 36px
    fontWeight: '700'
    lineHeight: 44px
  headline-md:
    fontFamily: Playfair Display
    fontSize: 32px
    fontWeight: '600'
    lineHeight: 40px
  headline-sm:
    fontFamily: Playfair Display
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
  body-sm:
    fontFamily: Inter
    fontSize: 14px
    fontWeight: '400'
    lineHeight: 20px
  label-bold:
    fontFamily: Inter
    fontSize: 14px
    fontWeight: '600'
    lineHeight: 16px
    letterSpacing: 0.05em
rounded:
  sm: 0.25rem
  DEFAULT: 0.5rem
  md: 0.75rem
  lg: 1rem
  xl: 1.5rem
  full: 9999px
spacing:
  unit: 8px
  container-max: 1280px
  gutter: 24px
  margin-desktop: 64px
  margin-mobile: 20px
  stack-sm: 12px
  stack-md: 24px
  stack-lg: 48px
---

## Brand & Style

The design system is anchored in a "Modern Coastal" aesthetic, targeting affluent travelers seeking a blend of luxury and relaxation. The personality is refined yet approachable—evoking the serenity of a high-end seaside resort. 

The style utilizes **Minimalism** enriched with **Tactile** elements. It relies on generous whitespace (the "air") to allow property imagery to breathe, while using soft, organic depth to make the interface feel tangible and trustworthy. The emotional goal is to reduce the cognitive load of travel planning, replacing it with a sense of calm and anticipation.

## Colors

The palette mimics the natural transition from shore to sea. 

- **Soft White (#F8F9FA):** Used for primary page backgrounds to maintain an airy, expansive feel.
- **Sandy Neutral (#EAE0D5):** Applied to secondary surfaces, search bars, and subtle dividers to ground the design in warmth.
- **Ocean Blue (#0077B6):** Reserved exclusively for primary actions, CTAs, and critical interactive states. It provides high contrast against the lighter tones to drive conversion.
- **Deep Slate Neutral (#4A4E69):** Used for body text and icons to ensure high legibility without the harshness of pure black.

## Typography

This design system employs a high-contrast typographic pairing to signal luxury and clarity.

- **Headings:** **Playfair Display** is used for all editorial content and property titles. The serif nature adds a layer of sophistication and "boutique" feeling. Use tighter letter spacing for larger display sizes to maintain a premium look.
- **Body & UI:** **Inter** is utilized for all functional text, descriptions, and data. Its neutral, geometric form ensures maximum readability during the booking process.
- **Labels:** Small labels and overlines should use Inter in semi-bold with a slight tracking increase (5%) for a clean, architectural feel.

## Layout & Spacing

The layout follows a **fixed-width centered grid** for desktop to evoke the feeling of a high-end travel magazine, transitioning to a fluid layout for mobile devices.

- **Desktop:** 12-column grid with a 1280px max-width. Large 64px outer margins reinforce the "airy" brand pillar.
- **Tablet:** 8-column grid with 32px margins.
- **Mobile:** 4-column grid with 20px margins.
- **Rhythm:** An 8px linear scale is used for all spatial relationships. Vertical stacking uses larger gaps (48px+) between major sections to prevent the UI from feeling cluttered or "salesy."

## Elevation & Depth

Hierarchy is established through **Ambient Shadows** and **Tonal Layering**. 

- **Base Layer:** Soft White (#F8F9FA).
- **Surface Layer:** Sandy Neutral (#EAE0D5) used for inset cards or subtle grouping.
- **Elevated States:** Property cards and modals use very soft, diffused shadows (Blur: 20px, Spread: 0, Y-Offset: 4px) with a 5% opacity of the Ocean Blue color to create a "glowing" lift rather than a muddy gray shadow.
- **Interactions:** On hover, cards should subtly lift (Y-offset increases) to provide tactile feedback without breaking the elegant aesthetic.

## Shapes

The shape language is consistently soft and organic.

- **Standard Elements:** Buttons, input fields, and small UI components use a **8px (0.5rem)** radius.
- **Large Containers:** Property cards, image galleries, and modals use a **16px (1rem)** radius to appear friendly and modern.
- **Full Rounding:** Search pills and "Check Availability" floating bars use a **pill-shape (100px)** to differentiate them as the primary functional tools of the platform.

## Components

- **Buttons:** Primary CTAs use a solid Ocean Blue fill with white text. Secondary buttons use a transparent background with an Ocean Blue border (2px). Hover states should include a slight darkening of the blue (#023E8A).
- **Cards:** Property cards are the most critical component. They feature a 1:1 or 4:3 aspect ratio image with a 16px corner radius, a subtle ambient shadow, and the price clearly indicated in a bold Inter weight.
- **Inputs:** Search and filter inputs use the Sandy Neutral (#EAE0D5) as a background fill with 0px borders to look integrated and modern. Focus states are highlighted by an Ocean Blue 2px bottom-border.
- **Chips/Filters:** Rounded pill-shapes with a light neutral fill. Selected states use Ocean Blue with white text.
- **Specialty Component - The Booking Bar:** A persistent, high-elevation floating bar at the bottom of mobile screens (or sidebar on desktop) that holds the primary "Book Now" action and price summary, ensuring the path to conversion is always accessible.