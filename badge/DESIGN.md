---
name: Vivid Achievement System
colors:
  surface: '#fcf8ff'
  surface-dim: '#dcd8e5'
  surface-bright: '#fcf8ff'
  surface-container-lowest: '#ffffff'
  surface-container-low: '#f5f2ff'
  surface-container: '#f0ecf9'
  surface-container-high: '#eae6f4'
  surface-container-highest: '#e4e1ee'
  on-surface: '#1b1b24'
  on-surface-variant: '#464555'
  inverse-surface: '#302f39'
  inverse-on-surface: '#f3effc'
  outline: '#777587'
  outline-variant: '#c7c4d8'
  surface-tint: '#4d44e3'
  primary: '#3525cd'
  on-primary: '#ffffff'
  primary-container: '#4f46e5'
  on-primary-container: '#dad7ff'
  inverse-primary: '#c3c0ff'
  secondary: '#855300'
  on-secondary: '#ffffff'
  secondary-container: '#fea619'
  on-secondary-container: '#684000'
  tertiary: '#571ac0'
  on-tertiary: '#ffffff'
  tertiary-container: '#6f3dd9'
  on-tertiary-container: '#e3d5ff'
  error: '#ba1a1a'
  on-error: '#ffffff'
  error-container: '#ffdad6'
  on-error-container: '#93000a'
  primary-fixed: '#e2dfff'
  primary-fixed-dim: '#c3c0ff'
  on-primary-fixed: '#0f0069'
  on-primary-fixed-variant: '#3323cc'
  secondary-fixed: '#ffddb8'
  secondary-fixed-dim: '#ffb95f'
  on-secondary-fixed: '#2a1700'
  on-secondary-fixed-variant: '#653e00'
  tertiary-fixed: '#e9ddff'
  tertiary-fixed-dim: '#d0bcff'
  on-tertiary-fixed: '#23005c'
  on-tertiary-fixed-variant: '#5516be'
  background: '#fcf8ff'
  on-background: '#1b1b24'
  surface-variant: '#e4e1ee'
typography:
  display-lg:
    fontFamily: Plus Jakarta Sans
    fontSize: 48px
    fontWeight: '800'
    lineHeight: 56px
    letterSpacing: -0.02em
  headline-lg:
    fontFamily: Plus Jakarta Sans
    fontSize: 32px
    fontWeight: '700'
    lineHeight: 40px
    letterSpacing: -0.01em
  headline-md:
    fontFamily: Plus Jakarta Sans
    fontSize: 24px
    fontWeight: '700'
    lineHeight: 32px
  body-lg:
    fontFamily: Plus Jakarta Sans
    fontSize: 18px
    fontWeight: '500'
    lineHeight: 28px
  body-md:
    fontFamily: Plus Jakarta Sans
    fontSize: 16px
    fontWeight: '400'
    lineHeight: 24px
  label-lg:
    fontFamily: Plus Jakarta Sans
    fontSize: 14px
    fontWeight: '600'
    lineHeight: 20px
    letterSpacing: 0.02em
  label-sm:
    fontFamily: Plus Jakarta Sans
    fontSize: 12px
    fontWeight: '700'
    lineHeight: 16px
  headline-lg-mobile:
    fontFamily: Plus Jakarta Sans
    fontSize: 28px
    fontWeight: '700'
    lineHeight: 36px
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
  lg: 40px
  xl: 64px
  container-max: 1200px
  gutter: 24px
---

## Brand & Style

The design system is centered on the concept of "Digital Trophies"—objects that feel valuable, tactile, and celebratory. The brand personality is exuberant and rewarding, designed to turn user milestones into moments of delight. 

The aesthetic blends **Glassmorphism** with **Tactile/Skeuomorphic** accents. UI elements utilize frosted-glass backgrounds to maintain a lightweight feel, while the badges themselves employ metallic gradients and multi-layered shadows to suggest physical depth and "collectibility." The overall experience should feel like an energetic, high-end gallery of personal accomplishments.

## Colors

The palette is anchored by four distinct "Achievement Tiers":
- **Primary (Blue/Indigo):** Standard milestones and functional UI actions.
- **Secondary (Gold):** Legendary or top-tier achievements.
- **Tertiary (Purple):** Rare, "Epic," or community-based rewards.
- **Success (Green):** Growth, health, and completion indicators.

Neutral tones are kept cool (Slate) to allow the vibrant achievement colors to pop. Every gradient should follow a "Light-Source" logic, with the top-left being slightly lighter than the bottom-right to simulate physical 3D volume.

## Typography

This design system utilizes **Plus Jakarta Sans** for its friendly, rounded terminals and contemporary feel. 

- **Headlines:** Use Bold (700) or ExtraBold (800) weights with slightly tight letter spacing to create a high-impact, punchy look for achievement titles.
- **Body:** Use Medium (500) weight for descriptions to maintain readability against glassmorphic backgrounds.
- **Labels:** Uppercase styling for "Tiers" or "Point Values" to create a clear distinction from narrative text.

## Layout & Spacing

The layout follows a **Fluid Grid** model based on an 8px rhythmic scale. 

- **Badge Grids:** Use a responsive CSS Grid with `repeat(auto-fill, minmax(140px, 1fr))` to allow badges to reflow naturally.
- **Margins:** Desktop views should maintain a 40px (lg) side margin, scaling down to 16px on mobile.
- **Stacking:** Elements within an achievement card (Icon -> Title -> Progress) should use consistent 12px (sm) vertical gaps.

## Elevation & Depth

Visual hierarchy is achieved through a combination of **Glassmorphism** and **Ambient Shadows**:

1.  **Level 0 (Surface):** The main background, ideally a soft gradient or a subtle pattern.
2.  **Level 1 (Cards):** Glassmorphic surfaces with a 12px backdrop blur and a 1px semi-transparent white stroke. 
3.  **Level 2 (Badges):** High-depth objects. These use "Compound Shadows"—one tight, darker shadow for contact, and one wide, colored "glow" shadow that inherits the badge's primary color (e.g., a gold badge casts a soft amber glow).
4.  **Level 3 (Modals/Pop-outs):** Deepest elevation with a 20% opacity black shadow and 40px blur to signify an "Unlocking" moment.

## Shapes

The design system emphasizes "Squircle" and circular geometry to reinforce the playful nature:
- **Containers/Cards:** Use `rounded-lg` (16px) to keep the UI soft but structured.
- **Badges:** Use a specialized 24px radius or full circles to differentiate them from standard UI components.
- **Interactive Elements:** Buttons and Chips are fully pill-shaped (999px) to invite interaction.
- **Inputs:** Use `rounded-md` (8px) for a slightly more formal, functional feel.

## Components

### Achievement Badges
The hero component. Badges consist of a central "Icon" (modern line-art or 3D illustration) encased in a metallic-gradient border. The background of the badge should use a radial gradient of the tier color (e.g., light gold to deep gold).

### Glass Cards
Used to house groups of badges. These must have `backdrop-filter: blur(12px)` and a thin, top-weighted white border to catch the "light."

### Progress Rings
For "In-Progress" achievements, use circular progress indicators with a thick (8px) stroke. The "track" should be a low-opacity version of the tier color, while the "indicator" is the vibrant solid color.

### Celebration Modals
When an achievement is unlocked, use a full-screen glass overlay. Add a "Confetti" particle system utilizing the Primary, Secondary, and Tertiary colors.

### Action Buttons
Primary buttons use a heavy drop shadow of their own color (e.g., Blue button with Blue shadow) to appear "lifted" off the glass surface. Use a subtle scale-down effect (95%) on click to mimic a physical button press.