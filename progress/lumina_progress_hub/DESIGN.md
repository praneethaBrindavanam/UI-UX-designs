---
name: Lumina Progress Hub
colors:
  surface: '#131313'
  surface-dim: '#131313'
  surface-bright: '#393939'
  surface-container-lowest: '#0e0e0e'
  surface-container-low: '#1c1b1b'
  surface-container: '#201f1f'
  surface-container-high: '#2a2a2a'
  surface-container-highest: '#353534'
  on-surface: '#e5e2e1'
  on-surface-variant: '#bacac5'
  inverse-surface: '#e5e2e1'
  inverse-on-surface: '#313030'
  outline: '#859490'
  outline-variant: '#3c4a46'
  surface-tint: '#3cddc7'
  primary: '#57f1db'
  on-primary: '#003731'
  primary-container: '#2dd4bf'
  on-primary-container: '#00574d'
  inverse-primary: '#006b5f'
  secondary: '#ddb7ff'
  on-secondary: '#490080'
  secondary-container: '#6f00be'
  on-secondary-container: '#d6a9ff'
  tertiary: '#ffcdd1'
  on-tertiary: '#67001f'
  tertiary-container: '#ffa5ae'
  on-tertiary-container: '#912038'
  error: '#ffb4ab'
  on-error: '#690005'
  error-container: '#93000a'
  on-error-container: '#ffdad6'
  primary-fixed: '#62fae3'
  primary-fixed-dim: '#3cddc7'
  on-primary-fixed: '#00201c'
  on-primary-fixed-variant: '#005047'
  secondary-fixed: '#f0dbff'
  secondary-fixed-dim: '#ddb7ff'
  on-secondary-fixed: '#2c0051'
  on-secondary-fixed-variant: '#6900b3'
  tertiary-fixed: '#ffdadc'
  tertiary-fixed-dim: '#ffb2b9'
  on-tertiary-fixed: '#400010'
  on-tertiary-fixed-variant: '#891933'
  background: '#131313'
  on-background: '#e5e2e1'
  surface-variant: '#353534'
typography:
  headline-xl:
    fontFamily: Inter
    fontSize: 40px
    fontWeight: '800'
    lineHeight: 48px
    letterSpacing: -0.02em
  headline-lg:
    fontFamily: Inter
    fontSize: 32px
    fontWeight: '700'
    lineHeight: 40px
    letterSpacing: -0.01em
  headline-lg-mobile:
    fontFamily: Inter
    fontSize: 28px
    fontWeight: '700'
    lineHeight: 36px
  headline-md:
    fontFamily: Inter
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
  label-caps:
    fontFamily: JetBrains Mono
    fontSize: 12px
    fontWeight: '700'
    lineHeight: 16px
    letterSpacing: 0.1em
  data-display:
    fontFamily: JetBrains Mono
    fontSize: 20px
    fontWeight: '500'
    lineHeight: 24px
rounded:
  sm: 0.25rem
  DEFAULT: 0.5rem
  md: 0.75rem
  lg: 1rem
  xl: 1.5rem
  full: 9999px
spacing:
  base: 4px
  xs: 8px
  sm: 12px
  md: 16px
  lg: 24px
  xl: 32px
  2xl: 48px
  gutter: 16px
  margin-mobile: 20px
---

## Brand & Style

This design system is built for a high-performance progress tracking environment. The brand personality is **motivational, precise, and tech-forward**, designed to make data entry and habit monitoring feel like an interactive, rewarding experience. It targets high-achievers who value both aesthetic sophistication and functional clarity.

The visual style is a hybrid of **Modern Corporate** and **Glassmorphism**. It utilizes deep layers of dark surfaces to create a "command center" feel, punctuated by vibrant, glowing accents that signify life and momentum. The interface should feel like a premium physical device—smooth, responsive, and tactile—while maintaining the ethereal qualities of translucent glass and light-based indicators.

## Colors

The palette is anchored by a deep charcoal base to minimize eye strain and maximize the pop of functional colors. 

- **Neutral Background (#121212):** The foundation of the app, providing a high-contrast canvas.
- **Action Teal (#2DD4BF):** Dedicated to media consumption, productivity tasks, and "doing" states.
- **Intellect Purple (#A855F7):** Reserved for reading, learning, and cognitive growth tracking.
- **Vitality Coral (#FB7185):** Used for fitness, health metrics, and physical energy levels.

Semantic colors for success (Green), warning (Amber), and error (Red) should be used sparingly, ensuring they do not compete with the three core category accents.

## Typography

The typography system prioritizes legibility and data precision. **Inter** is the primary typeface for all UI elements and prose, providing a neutral and modern feel. 

For counters, percentages, and time-stamps, the design system utilizes **JetBrains Mono**. This monospaced choice ensures that numeric data remains perfectly aligned during real-time updates (tabular figures), reinforcing the "tech-forward" and "precise" brand pillars. 

- Use `headline-xl` for primary dashboard titles.
- Use `label-caps` for category headers and small metadata.
- Apply `data-display` to all progress percentages and metric values.

## Layout & Spacing

This design system follows a **fluid grid** logic optimized for mobile-first interactions. All spacing is derived from a 4px baseline grid to ensure mathematical harmony.

- **Margins:** Standard mobile views use a 20px side margin to provide breathing room on edge-to-edge displays.
- **Vertical Rhythm:** Content blocks are typically separated by `lg` (24px) or `xl` (32px) units.
- **Internal Padding:** Cards and containers use `md` (16px) or `lg` (24px) padding depending on the density of the information.
- **Touch Targets:** All interactive elements must maintain a minimum height of 48px.

## Elevation & Depth

Hierarchy is established through **Glassmorphism** and **Tonal Layering**. 

1.  **Base Layer:** The deepest level is the `#121212` background.
2.  **Surface Layer:** Semi-transparent cards (using `rgba(255, 255, 255, 0.05)`) sit above the background with a 20px backdrop-blur. 
3.  **Active Indicators:** Elements representing active progress or "on" states utilize a subtle **inner glow** and an outer **ambient shadow** tinted with the category color (e.g., a Teal glow for Action cards).
4.  **Borders:** Cards use a 1px solid stroke at 10% white opacity to define edges against the dark background, simulating a thin glass rim.

## Shapes

The shape language is consistently **Rounded**, striking a balance between the clinical sharpness of data and the approachability of a lifestyle app.

- **Default Corners:** 0.5rem (8px) for buttons and small input fields.
- **Large Containers:** 1rem (16px) for cards and modals (`rounded-lg`).
- **Progress Bars:** Use fully pill-shaped caps (3rem/`rounded-xl`) to signify fluidity and movement.
- **Selection States:** When a category is active, the shape may expand slightly or use a more pronounced corner radius to indicate focus.

## Components

### Buttons
- **Primary:** Solid background using the category accent color with black text for maximum contrast.
- **Secondary/Ghost:** 1px accent border with transparent center and accent-colored text.
- **Shape:** Rounded-md (8px).

### Progress Cards
- **Construction:** Glassmorphic background with backdrop-blur. 
- **Header:** Title in Inter Bold, Metric in JetBrains Mono.
- **Visualization:** A linear progress bar at the bottom of the card or a circular gauge in the center.

### Chips & Tags
- Used for sub-categories. 
- **Style:** Subtle dark-grey fill with white text, or low-opacity accent fill (e.g., 15% Teal) for active filters.

### Input Fields
- Underlined or subtly boxed with `#1E1E1E` fill. 
- The cursor and active bottom-border should glow with the Action Teal accent.

### Navigation Bar
- A floating "dock" style bar with high backdrop-blur. 
- Icons use high-stroke weights (2px) and active states include a small glowing dot beneath the icon in the primary accent.