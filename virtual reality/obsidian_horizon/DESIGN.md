---
name: Obsidian Horizon
colors:
  surface: '#131315'
  surface-dim: '#131315'
  surface-bright: '#39393b'
  surface-container-lowest: '#0e0e10'
  surface-container-low: '#1c1b1d'
  surface-container: '#201f21'
  surface-container-high: '#2a2a2c'
  surface-container-highest: '#353437'
  on-surface: '#e5e1e4'
  on-surface-variant: '#b9cacb'
  inverse-surface: '#e5e1e4'
  inverse-on-surface: '#313032'
  outline: '#849495'
  outline-variant: '#3b494b'
  surface-tint: '#00dbe9'
  primary: '#dbfcff'
  on-primary: '#00363a'
  primary-container: '#00f0ff'
  on-primary-container: '#006970'
  inverse-primary: '#006970'
  secondary: '#ebb2ff'
  on-secondary: '#520072'
  secondary-container: '#b600f8'
  on-secondary-container: '#fff6fc'
  tertiary: '#e5ffba'
  on-tertiary: '#223600'
  tertiary-container: '#a2ef00'
  on-tertiary-container: '#456900'
  error: '#ffb4ab'
  on-error: '#690005'
  error-container: '#93000a'
  on-error-container: '#ffdad6'
  primary-fixed: '#7df4ff'
  primary-fixed-dim: '#00dbe9'
  on-primary-fixed: '#002022'
  on-primary-fixed-variant: '#004f54'
  secondary-fixed: '#f8d8ff'
  secondary-fixed-dim: '#ebb2ff'
  on-secondary-fixed: '#320047'
  on-secondary-fixed-variant: '#74009f'
  tertiary-fixed: '#a9f900'
  tertiary-fixed-dim: '#94db00'
  on-tertiary-fixed: '#121f00'
  on-tertiary-fixed-variant: '#334f00'
  background: '#131315'
  on-background: '#e5e1e4'
  surface-variant: '#353437'
typography:
  display-lg:
    fontFamily: Sora
    fontSize: 48px
    fontWeight: '800'
    lineHeight: '1.1'
    letterSpacing: -0.02em
  display-lg-mobile:
    fontFamily: Sora
    fontSize: 32px
    fontWeight: '800'
    lineHeight: '1.2'
  headline-md:
    fontFamily: Sora
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
    lineHeight: '1.5'
  label-mono:
    fontFamily: JetBrains Mono
    fontSize: 14px
    fontWeight: '500'
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
  margin-desktop: 64px
  margin-mobile: 24px
  z-layer-step: 20px
---

## Brand & Style
The brand personality is immersive, high-fidelity, and forward-looking. It targets power users and digital pioneers who operate in spatial environments. The UI evokes a sense of deep focus and "flow state" by utilizing a Dark-mode first approach that minimizes eye strain in VR while highlighting critical data through luminous accents.

The design style is a hybrid of **Glassmorphism** and **Cyber-Minimalism**. It uses deep obsidian surfaces with high-transparency frosted layers to simulate physical depth in a 3D space. Visual interest is driven by light-emitting properties—glows, blurs, and vibrant neon strokes—rather than traditional flat colors.

## Colors
The palette is built on a foundation of "Deep Obsidian" (`#0A0A0C`) to ensure infinite depth in VR headsets. 

- **Primary (Electric Blue):** Used for active states, primary actions, and "interactive" light sources.
- **Secondary (Cyber Purple):** Used for supplemental data, secondary interactive elements, and ambient background gradients.
- **Tertiary (Lime Green):** Reserved for success states, critical notifications, and high-contrast system feedback.
- **Neutral:** A range of semi-transparent greys used for glass panel surfaces and subtle borders.

All colors should be implemented with a "glow" property (0-15px spread) when in an active or hovered state to simulate light emission in a spatial environment.

## Typography
The typography system uses a tri-font approach to balance personality and technical precision. **Sora** provides a geometric, futuristic feel for large headers. **Geist** ensures maximum legibility for body text and descriptive content. **JetBrains Mono** is used for technical readouts, labels, and metadata to reinforce the high-tech, "under-the-hood" aesthetic.

In spatial environments, avoid font sizes smaller than 14px to prevent aliasing issues. Headlines should use "Outer Glow" text shadows when layered over complex backgrounds.

## Layout & Spacing
The layout follows a **Fluid Grid** model designed for a 120-degree field of view. Elements are positioned using a dynamic 8px scale. 

In a VR context, "depth spacing" (the Z-axis) is as critical as X and Y. Panels should be separated by `z-layer-step` units to create a clear stack order. 
- **Desktop/Large Scale:** Content spans a wide, curved container to accommodate peripheral vision.
- **Mobile/Narrow Scale:** Content collapses into a single vertical stack, increasing the size of touch/gaze targets to ensure accuracy.

## Elevation & Depth
Elevation is achieved through **Glassmorphism** and **Volumetric Lighting**.
1.  **Backdrop Blur:** All floating panels must use a `20px` to `40px` backdrop-blur filter.
2.  **Tonal Layers:** Deep surfaces use a 40% opacity obsidian fill. Higher surfaces use a 10% opacity white "shine" overlay.
3.  **Luminous Outlines:** Use 1px solid borders with 20% opacity of the Primary color. On hover, the border opacity should increase to 100% with an outer glow.
4.  **Shadows:** Do not use traditional black shadows. Use "Ambient Glows"—diffused, low-opacity colored shadows (matching the element's accent color) to simulate light reflecting onto the background.

## Shapes
The shape language uses a "Rounded" (`0.5rem`) base to feel approachable yet structured. Interactive elements like buttons and chips should feel like precision-machined physical objects. 

Avoid sharp 90-degree corners to prevent visual "harshness" in high-contrast VR settings. Use `rounded-xl` (`1.5rem`) for large container panels to create a softer, more organic perimeter for the user's field of view.

## Components
- **Buttons:** High-gloss surfaces. Primary buttons feature a solid Primary-to-Secondary gradient fill. Secondary buttons are "ghost" style with a 1px Primary border that glows on gaze/hover.
- **Input Fields:** Semi-transparent "well" styles. The focus state should trigger a scanning-line animation or a subtle pulse of the Primary color.
- **Cards:** Use the glassmorphism stack. Headers should be separated from the body by a 1px semi-transparent horizontal line.
- **Chips:** Highly rounded (Pill-shaped) with monospaced labels. Use tertiary colors for status indicators.
- **Gaze Reticle:** A dynamic component that scales and pulses when hovering over interactive elements.
- **HUD Overlays:** Persistent elements that use minimal opacity (5-10%) until interacted with, preventing "burn-in" fatigue.