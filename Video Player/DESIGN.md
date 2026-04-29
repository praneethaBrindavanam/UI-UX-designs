---
name: Cinema Neon
colors:
  surface: '#111415'
  surface-dim: '#111415'
  surface-bright: '#373a3b'
  surface-container-lowest: '#0c0f10'
  surface-container-low: '#191c1d'
  surface-container: '#1d2021'
  surface-container-high: '#282a2b'
  surface-container-highest: '#323536'
  on-surface: '#e1e3e4'
  on-surface-variant: '#b9cacb'
  inverse-surface: '#e1e3e4'
  inverse-on-surface: '#2e3132'
  outline: '#849495'
  outline-variant: '#3b494b'
  surface-tint: '#00dbe9'
  primary: '#dbfcff'
  on-primary: '#00363a'
  primary-container: '#00f0ff'
  on-primary-container: '#006970'
  inverse-primary: '#006970'
  secondary: '#dcb8ff'
  on-secondary: '#480081'
  secondary-container: '#7701d0'
  on-secondary-container: '#dcb7ff'
  tertiary: '#f9f5f5'
  on-tertiary: '#313030'
  tertiary-container: '#dcd9d8'
  on-tertiary-container: '#605f5e'
  error: '#ffb4ab'
  on-error: '#690005'
  error-container: '#93000a'
  on-error-container: '#ffdad6'
  primary-fixed: '#7df4ff'
  primary-fixed-dim: '#00dbe9'
  on-primary-fixed: '#002022'
  on-primary-fixed-variant: '#004f54'
  secondary-fixed: '#efdbff'
  secondary-fixed-dim: '#dcb8ff'
  on-secondary-fixed: '#2c0051'
  on-secondary-fixed-variant: '#6700b5'
  tertiary-fixed: '#e5e2e1'
  tertiary-fixed-dim: '#c8c6c5'
  on-tertiary-fixed: '#1c1b1b'
  on-tertiary-fixed-variant: '#474646'
  background: '#111415'
  on-background: '#e1e3e4'
  surface-variant: '#323536'
typography:
  headline-lg:
    fontFamily: Space Grotesk
    fontSize: 32px
    fontWeight: '700'
    lineHeight: 40px
    letterSpacing: -0.02em
  headline-md:
    fontFamily: Space Grotesk
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
  label-lg:
    fontFamily: Space Grotesk
    fontSize: 14px
    fontWeight: '600'
    lineHeight: 20px
    letterSpacing: 0.05em
  label-sm:
    fontFamily: Space Grotesk
    fontSize: 12px
    fontWeight: '500'
    lineHeight: 16px
    letterSpacing: 0.1em
rounded:
  sm: 0.25rem
  DEFAULT: 0.5rem
  md: 0.75rem
  lg: 1rem
  xl: 1.5rem
  full: 9999px
spacing:
  touch-target-min: 48px
  container-padding: 20px
  stack-gap-sm: 8px
  stack-gap-md: 16px
  stack-gap-lg: 24px
  edge-margin: 16px
---

## Brand & Style

This design system is engineered for an immersive, cinematic mobile experience. The brand personality is technical, high-performance, and futuristic, aimed at enthusiasts who demand a premium viewing environment. 

The aesthetic blends **Minimalism** with **Glassmorphism**. By stripping away unnecessary chrome and utilizing deep black backgrounds, the focus remains entirely on the content. Interactive elements utilize translucent layers and vibrant accents to guide the user without breaking immersion. The emotional response is one of precision and sophistication—a digital private theater that feels responsive and high-end.

## Colors

The palette is built on a foundation of absolute blacks (`#000000`) to maximize OLED display efficiency and contrast. 

- **Primary (Electric Blue):** Used for active states, playback progress, and critical action highlights.
- **Secondary (Electric Purple):** Used for secondary interactions, such as volume levels or category tags.
- **Surface Colors:** Deep grays (`#121212`, `#1E1E1E`) are used to define subtle boundaries between panels.
- **Semantic Colors:** Warning and error states should utilize the Primary Blue but shifted in hue toward red only when critical, otherwise maintaining the neon aesthetic through high-saturation variants.

## Typography

This design system uses a dual-font strategy to balance technical character with readability. 

**Space Grotesk** is used for headlines and labels to reinforce the futuristic, geometric aesthetic. It should be used sparingly for metadata (timecodes, resolution labels) to provide a "dashboard" feel. 

**Inter** is utilized for all body text and descriptions. Its neutral, utilitarian design ensures maximum legibility against dark backgrounds, even at smaller scales or during fast-paced interactions. All typography must maintain a minimum contrast ratio of 7:1 against the background.

## Layout & Spacing

The layout follows a **fluid grid** model optimized for landscape and portrait mobile orientations. 

- **Safe Zones:** High priority is placed on keeping controls within the natural "thumb zone" of a mobile device. 
- **Touch Targets:** No interactive element (buttons, toggles, seeker heads) shall be smaller than 48x48px to ensure ease of use during playback.
- **Spacing Rhythm:** An 8px linear scale is used for all internal padding and margins. 
- **Content Overlay:** Player controls are positioned as a floating layer with a 20px margin from the screen edge to prevent accidental system gesture triggers (like "swipe to go home").

## Elevation & Depth

Visual hierarchy is established through **Glassmorphism** and **Tonal Layers**.

1.  **Base Layer:** The video content or an absolute black surface.
2.  **Backdrop Layer:** Overlays (menus, settings) use a 20px background blur with a 40% opacity fill of the surface gray. 
3.  **Accent Glow:** Active elements like the playhead or selected menu items emit a soft, diffused outer glow (12px blur, 20% opacity) using the Primary Electric Blue hex.
4.  **Borders:** Instead of heavy shadows, use 1px "ghost" borders with 10% white opacity to define the edges of floating cards or menus against the dark background.

## Shapes

The design system adopts a **Rounded** shape language to soften the high-contrast technical aesthetic. 

- **Buttons & Controls:** Use 1rem (16px) corner radius for a comfortable, modern feel.
- **Progress Bars:** Seek bars and volume sliders utilize fully rounded (pill-shaped) caps to emphasize the fluid nature of time and sound.
- **Cards:** Content thumbnails and detail panels use a 1.5rem (24px) radius to create a distinct "window" effect.

## Components

### Buttons & Icons
- **Playback Controls:** Centered icons (Play/Pause/Skip) are large (64px+) with high-stroke weights (2px to 2.5px).
- **Primary Buttons:** Solid Electric Blue fill with black text for maximum contrast.
- **Ghost Buttons:** Transparent fill with a 1px border for secondary actions like "Share" or "Report."

### Progress Bar (The Seeker)
- **Track:** 4px height, dark gray (20% white opacity).
- **Progress:** 4px height, Electric Blue.
- **Playhead (Thumb):** A 16px circular glow-pulse that expands to 24px when actively being dragged (touched).

### Chips & Metadata
- **Tags:** Small, pill-shaped containers for resolution (4K, HDR) or genre. Use Secondary Purple for specific highlights like "Live" or "New."

### Lists & Navigation
- **Subtitles/Audio Menus:** Translucent bottom sheets with 16px bottom-to-top slide animations. Items are separated by subtle 1px dividers.

### Custom Component: Gesture Overlays
- When double-tapping to seek, a semi-transparent ripple effect should radiate from the touch point, displaying a "+10s" or "-10s" label in Space Grotesk.