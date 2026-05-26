---
name: Precision Data Interface
colors:
  surface: '#f8f9fb'
  surface-dim: '#d9dadc'
  surface-bright: '#f8f9fb'
  surface-container-lowest: '#ffffff'
  surface-container-low: '#f3f4f6'
  surface-container: '#edeef0'
  surface-container-high: '#e7e8ea'
  surface-container-highest: '#e1e2e4'
  on-surface: '#191c1e'
  on-surface-variant: '#434654'
  inverse-surface: '#2e3132'
  inverse-on-surface: '#f0f1f3'
  outline: '#737685'
  outline-variant: '#c3c6d6'
  surface-tint: '#0c56d0'
  primary: '#003d9b'
  on-primary: '#ffffff'
  primary-container: '#0052cc'
  on-primary-container: '#c4d2ff'
  inverse-primary: '#b2c5ff'
  secondary: '#535f73'
  on-secondary: '#ffffff'
  secondary-container: '#d4e0f8'
  on-secondary-container: '#576377'
  tertiary: '#7b2600'
  on-tertiary: '#ffffff'
  tertiary-container: '#a33500'
  on-tertiary-container: '#ffc6b2'
  error: '#ba1a1a'
  on-error: '#ffffff'
  error-container: '#ffdad6'
  on-error-container: '#93000a'
  primary-fixed: '#dae2ff'
  primary-fixed-dim: '#b2c5ff'
  on-primary-fixed: '#001848'
  on-primary-fixed-variant: '#0040a2'
  secondary-fixed: '#d7e3fb'
  secondary-fixed-dim: '#bbc7de'
  on-secondary-fixed: '#101c2d'
  on-secondary-fixed-variant: '#3b475b'
  tertiary-fixed: '#ffdbcf'
  tertiary-fixed-dim: '#ffb59b'
  on-tertiary-fixed: '#380d00'
  on-tertiary-fixed-variant: '#812800'
  background: '#f8f9fb'
  on-background: '#191c1e'
  surface-variant: '#e1e2e4'
typography:
  display-lg:
    fontFamily: Inter
    fontSize: 32px
    fontWeight: '600'
    lineHeight: 40px
    letterSpacing: -0.02em
  headline-md:
    fontFamily: Inter
    fontSize: 24px
    fontWeight: '600'
    lineHeight: 32px
    letterSpacing: -0.01em
  title-sm:
    fontFamily: Inter
    fontSize: 18px
    fontWeight: '500'
    lineHeight: 24px
  body-md:
    fontFamily: Inter
    fontSize: 14px
    fontWeight: '400'
    lineHeight: 20px
  body-sm:
    fontFamily: Inter
    fontSize: 13px
    fontWeight: '400'
    lineHeight: 18px
  data-tabular:
    fontFamily: Inter
    fontSize: 13px
    fontWeight: '400'
    lineHeight: 16px
  label-caps:
    fontFamily: Inter
    fontSize: 11px
    fontWeight: '700'
    lineHeight: 16px
    letterSpacing: 0.05em
  code-sm:
    fontFamily: JetBrains Mono
    fontSize: 12px
    fontWeight: '400'
    lineHeight: 16px
rounded:
  sm: 0.125rem
  DEFAULT: 0.25rem
  md: 0.375rem
  lg: 0.5rem
  xl: 0.75rem
  full: 9999px
spacing:
  base: 4px
  xs: 4px
  sm: 8px
  md: 16px
  lg: 24px
  xl: 32px
  gutter: 16px
  margin-mobile: 16px
  margin-desktop: 32px
---

## Brand & Style

The design system is engineered for high-density data environments where clarity, speed of cognition, and functional hierarchy are paramount. The target audience consists of analysts, researchers, and administrators who interact with complex datasets for extended periods. 

The aesthetic follows a **Modern Minimalism** approach, stripping away ornamental flourishes to prioritize content. It utilizes a systematic "Utility-First" philosophy, where every visual element serves a functional purpose. The emotional response is one of calm authority, reliability, and precision. We achieve this through generous white space in non-data areas, rigorous alignment, and a sophisticated use of neutral tones to let data visualizations and interactive states stand out.

## Colors

This design system utilizes a palette of **Functional Blues** and **Neutral Grays** to create a structured, professional environment. 

- **Primary Blue:** Reserved strictly for primary actions, active states, and essential navigational cues. It is high-contrast to ensure immediate recognition.
- **Neutral Grays:** Used for structural elements like borders, backgrounds, and secondary text. This range allows for subtle layering without visual clutter.
- **High-Contrast Text:** The primary text color is a deep navy-charcoal, ensuring maximum legibility against light backgrounds. 
- **System States:** Success (Green), Warning (Amber), and Error (Red) colors are used sparingly and are slightly desaturated to maintain the professional tone of the design system.

## Typography

The typography system is built on **Inter**, selected for its exceptional legibility in digital interfaces and its neutral, systematic character. 

For data rows and tables, we employ tabular numbers (`tnum`) to ensure columns of figures align vertically, aiding rapid scanning. A clear hierarchy is established by using varying weights rather than aggressive size jumps. 

**Mobile Adaptation:**
- `display-lg` scales down to 24px on mobile devices.
- `headline-md` scales down to 20px on mobile devices.
- Table-based data transitions to card-based layouts on small screens, maintaining the `body-sm` size for maximum information density.

## Layout & Spacing

This design system utilizes a **Fixed Grid** model for main content areas to maintain a controlled reading line, while sidebars and data tables can expand fluently.

- **Rhythm:** A strict 4px baseline grid governs all spacing.
- **Density:** To accommodate large lists, we use a "Comfortable Dense" approach. Table rows should have a height of 40px (Standard) or 32px (Compact).
- **Desktop:** 12-column grid with a max-width of 1440px. 24px gutters.
- **Tablet:** 8-column grid with 16px margins.
- **Mobile:** 4-column grid with 16px margins. 

Data-heavy views should prioritize horizontal space, often requiring sidebars to collapse into icon-only states to maximize the primary data canvas.

## Elevation & Depth

To maintain a clean and professional look, depth is communicated through **Tonal Layers** and **Low-Contrast Outlines** rather than heavy shadows.

- **Surface Levels:** The primary background uses a subtle off-white/gray (`#F4F5F7`). Cards and data containers use pure white (`#FFFFFF`) to pop forward.
- **Borders:** Subtle 1px borders in `#DFE1E6` define boundaries between elements. 
- **Shadows:** Use a single, highly-diffused ambient shadow for floating elements like modals or dropdown menus: `0px 4px 12px rgba(9, 30, 66, 0.15)`. 
- **Interaction:** Hover states on rows or buttons are indicated by a slight shift in background color (e.g., `#EBECF0`) rather than a change in elevation.

## Shapes

The shape language is **Soft (0.25rem)**, reflecting a professional and systematic character.

- **Standard Elements:** Buttons, input fields, and checkboxes use a 4px (0.25rem) radius.
- **Containers:** Large cards or modals use an 8px (0.5rem) radius to soften the layout's perimeter.
- **Selection Indicators:** Active states in navigation or pagination use sharp-edged vertical bars or fully square-off corners where they meet container edges to reinforce the grid-based structure.

## Components

### Buttons & Inputs
- **Primary Button:** Solid Blue background, White text. No gradient.
- **Secondary Button:** Subtle gray background (`#F4F5F7`) with Primary Blue text.
- **Input Fields:** 1px border, 4px radius. On focus, the border changes to Primary Blue with a 2px soft outer glow.

### Data Tables
- **Header:** `label-caps` typography, light gray background, 1px bottom border.
- **Rows:** Alternating zebra striping is avoided in favor of a clear hover state (`#F4F5F7`).
- **Cells:** Vertical alignment is centered. Numeric data is right-aligned.

### Pagination
- **Active State:** Solid Primary Blue background with white text.
- **Hover State:** Light blue tint (`#DEEBFF`) background.
- **Structure:** Includes "First/Last" icons, "Jump to Page" text input, and a "Results per page" dropdown menu. Elements are separated by 4px of spacing.

### Chips & Badges
- Used for status indicators. Use a "Subtle" style: light background with dark text in the same color family (e.g., Light Green background with Dark Green text for "Success").