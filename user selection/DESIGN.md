---
name: Cinematic Premium
colors:
  surface: '#141313'
  surface-dim: '#141313'
  surface-bright: '#3a3939'
  surface-container-lowest: '#0e0e0e'
  surface-container-low: '#1c1b1b'
  surface-container: '#201f1f'
  surface-container-high: '#2b2a2a'
  surface-container-highest: '#353434'
  on-surface: '#e5e2e1'
  on-surface-variant: '#c4c7c7'
  inverse-surface: '#e5e2e1'
  inverse-on-surface: '#313030'
  outline: '#8e9192'
  outline-variant: '#444748'
  surface-tint: '#c8c6c5'
  primary: '#c8c6c5'
  on-primary: '#313030'
  primary-container: '#0f0f0f'
  on-primary-container: '#7d7b7b'
  inverse-primary: '#5f5e5e'
  secondary: '#c6c6c7'
  on-secondary: '#2f3131'
  secondary-container: '#454747'
  on-secondary-container: '#b4b5b5'
  tertiary: '#cac6c3'
  on-tertiary: '#32302f'
  tertiary-container: '#100f0e'
  on-tertiary-container: '#7e7b79'
  error: '#ffb4ab'
  on-error: '#690005'
  error-container: '#93000a'
  on-error-container: '#ffdad6'
  primary-fixed: '#e5e2e1'
  primary-fixed-dim: '#c8c6c5'
  on-primary-fixed: '#1c1b1b'
  on-primary-fixed-variant: '#474646'
  secondary-fixed: '#e2e2e2'
  secondary-fixed-dim: '#c6c6c7'
  on-secondary-fixed: '#1a1c1c'
  on-secondary-fixed-variant: '#454747'
  tertiary-fixed: '#e6e1df'
  tertiary-fixed-dim: '#cac6c3'
  on-tertiary-fixed: '#1d1b1a'
  on-tertiary-fixed-variant: '#484645'
  background: '#141313'
  on-background: '#e5e2e1'
  surface-variant: '#353434'
typography:
  display-lg:
    fontFamily: Inter
    fontSize: 48px
    fontWeight: '800'
    lineHeight: '1.1'
    letterSpacing: -0.02em
  headline-md:
    fontFamily: Inter
    fontSize: 32px
    fontWeight: '700'
    lineHeight: '1.2'
  title-sm:
    fontFamily: Inter
    fontSize: 20px
    fontWeight: '600'
    lineHeight: '1.4'
  body-base:
    fontFamily: Inter
    fontSize: 16px
    fontWeight: '400'
    lineHeight: '1.6'
  label-caps:
    fontFamily: Inter
    fontSize: 12px
    fontWeight: '700'
    lineHeight: '1.0'
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
  gutter: 24px
  margin-edge: 48px
  container-max: 1440px
  stack-sm: 16px
  stack-md: 32px
  stack-lg: 64px
---

## Brand & Style

The design system is engineered to evoke a cinematic, high-end theater experience. It targets a sophisticated audience that values immersion and ease of discovery. The visual language leans heavily into **Glassmorphism** and **Minimalism**, creating a sense of depth that mimics light reflecting off glass in a dark room. 

The emotional response is one of "focused luxury"—where the interface recedes to let the content shine, yet feels tactile and premium when interacted with. By utilizing deep charcoal foundations and vibrant profile-specific accents, the system provides a personalized environment that feels exclusive to each user. High-contrast focus states ensure accessibility remains a priority without compromising the sleek, modern aesthetic.

## Colors

This design system is built on a dark-mode-default foundation. The primary background is a deep, singular charcoal (#0F0F0F) to maximize the "infinite black" effect on OLED screens. 

Typography and iconography are strictly white (#FFFFFF) or high-opacity grays to maintain crisp readability. Three vibrant accents—Electric Blue, Sunset Orange, and Royal Purple—are reserved for profile-specific personalization and active state highlights. Semantic colors (Success, Warning, Error) should be used sparingly, prioritized only for critical feedback loops, allowing the profile accents to dominate the visual hierarchy.

## Typography

The design system utilizes **Inter** for its incredible clarity and modern, geometric feel. Headlines use a Bold or Extra-Bold weight with tighter letter-spacing to create a "blocky," high-impact cinematic look. Body copy remains clean and legible with standard leading. For metadata—such as film genres, ratings, or timestamps—uppercase labels with increased letter-spacing are used to differentiate technical information from narrative content.

## Layout & Spacing

The layout philosophy follows a **Fluid Grid** model with generous margins to ensure the content never feels cramped. A 12-column grid is standard for desktop, collapsing to 4 columns for mobile. 

The spacing rhythm is strictly 8px-based. Margins at the screen edges are intentionally wide (48px+) to create a "letterboxed" feel, focusing the user's eye on the center of the screen. Elements within a card or module use tighter 16px padding, while large sections are separated by 64px gaps to allow the UI to breathe.

## Elevation & Depth

Hierarchy is established through **Glassmorphism** rather than traditional drop shadows. Surfaces are layered using "Glass" containers: semi-transparent white overlays (8-12% opacity) with a background blur (16px to 32px). 

When an element is focused or hovered, it "lifts" by increasing the background blur intensity and adding a high-contrast 2px border using the user's profile accent color. This creates a tactile, illuminated effect where the active element appears to glow against the deep charcoal background. Secondary elevation is achieved by stacking these translucent layers, where each higher tier has a slightly higher opacity and stronger blur.

## Shapes

The design system utilizes a soft, ultra-rounded shape language. Standard containers and cards feature a **16px (1rem)** radius, while larger hero sections or modals may increase this to **24px (1.5rem)**. Buttons and input fields follow the `rounded-lg` (1rem) standard to ensure a consistent, friendly, and premium feel. This high degree of rounding balances the high-contrast typography and creates a more "organic" interface that feels modern and approachable.

## Components

- **Buttons**: Primary buttons are solid white with black text. Secondary buttons use the glassmorphic style (translucent background, white border). Focused buttons receive a thick, 3px outline in the user's accent color.
- **Cards**: Movie and show thumbnails must have 16px rounded corners. Upon hover, the card scales up 5% and displays a glassmorphic overlay containing the title and play button.
- **Chips/Badges**: Small, semi-transparent capsules with 100px (pill) rounding. Used for categories, quality tags (4K, HDR), and ratings.
- **Input Fields**: Ghost-style inputs with a subtle white bottom border. On focus, the border transitions to the accent color and a subtle glass background appears.
- **Lists**: Horizontal scrolling rows ("Carousels") with no visible scrollbars. The end of the row should fade into the background color using a linear gradient.
- **Progress Bars**: Used for "Continue Watching." A thin 4px track in 20% white, with the active progress filled in the user's profile accent color.
- **Profile Pickers**: Circular avatars with a high-contrast glowing ring (2px) using the specific profile's accent color.