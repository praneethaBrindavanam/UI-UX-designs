# Design System Strategy: The Cinematic Companion

## 1. Overview & Creative North Star
**Creative North Star: "The Digital Projectionist"**

This design system is built to bridge the gap between the physical living room and the digital interface. It moves away from the "data-heavy app" aesthetic and toward a "high-end gallery" experience. The goal is to make the user feel like they are interacting with the light of the screen itself, rather than a rigid software interface.

By utilizing **intentional asymmetry**—such as offset headline placements and overlapping poster art—we break the traditional "grid-jail" of mobile apps. Content should feel like it is floating in a deep, infinite space, using **tonal depth** and **glassmorphism** to create a sense of cinematic immersion.

---

## 2. Colors: Depth and Luminance
The palette is rooted in the absence of light, using deep charcoals to allow the content (movie posters, trailers, and UI accents) to vibrate.

### The "No-Line" Rule
**Prohibition of 1px solid borders:** To maintain a premium, cinematic feel, do not use borders to define sections. Use background color shifts. For example, a `surface-container-low` section sitting on a `surface` background creates a natural boundary without the "cheapening" effect of a stroke.

### Surface Hierarchy & Nesting
Think of the UI as layers of dark glass. 
- **Backdrop:** `background` (#0e0e0f).
- **Primary Layout Blocks:** `surface-container` (#1a191b).
- **Floating Interactive Elements:** `surface-container-high` (#201f21).
- **Nested Content (within cards):** `surface-container-lowest` (#000000) for high-contrast wells.

### The "Glass & Gradient" Rule
Floating overlays (Modals, Navigation Bars, and Detail Cards) must use a **Glassmorphism effect**. Combine `surface-variant` with a 60-80% opacity and a `backdrop-filter: blur(20px)`. 

### Signature Textures
Main Action Buttons should not be flat. Use a linear gradient from `primary` (#81ecff) to `primary-container` (#00e3fd) at a 135-degree angle. This mimics the "glow" of a high-end OLED display.

---

## 3. Typography: Editorial Authority
We use a dual-font strategy to balance character with extreme legibility.

- **Display & Headlines (Manrope):** Bold, wide apertures. Used for show titles and major category headers. It conveys the "Editorial" feel of a film magazine.
- **Body & Labels (Inter):** Highly legible, neutral. Used for synopsis text, metadata (release years, ratings), and button labels.

**Hierarchy of Intent:**
- **Display-LG (3.5rem):** Reserved for hero titles only. Use tight letter-spacing (-2%).
- **Headline-SM (1.5rem):** The standard for "Continue Watching" or "Trending" headers.
- **Body-MD (0.875rem):** The workhorse for all long-form descriptions. Use `on-surface-variant` to reduce eye strain in dark mode.

---

## 4. Elevation & Depth: Tonal Layering
Traditional drop shadows look muddy on dark themes. We use light and transparency instead.

### The Layering Principle
Achieve depth by stacking tiers. Place a `surface-container-lowest` card inside a `surface-container-low` section. This creates "recessed" depth, making the card look like it’s set into the UI.

### Ambient Shadows
If an element must float (e.g., a "Remote Control" FAB), use a large, diffused shadow:
- **X: 0, Y: 12, Blur: 40px.**
- **Color:** A tinted version of the primary glow (e.g., `primary` at 8% opacity).

### The "Ghost Border" Fallback
If a border is required for accessibility (e.g., in focused states), use a **Ghost Border**. Use the `outline-variant` token (#484849) at **20% opacity**. Never use 100% opaque borders.

---

## 5. Components: The Cinematic Primitive

### Buttons
- **Primary:** Gradient-filled (`primary` to `primary-container`), `full` roundedness. Text: `on-primary-fixed` (Inter Bold).
- **Secondary:** Semi-transparent glass. Background: `surface-variant` at 40% opacity with `backdrop-filter`. No border.
- **Tertiary:** Text-only in `primary` color. Used for "See All" or "Dismiss."

### Cards & Lists: The Separation Rule
**Forbid the use of divider lines.** To separate movies in a list:
1. Use **Vertical White Space** (Spacing `6` or `8`).
2. Use **Subtle Background Shifts**. Each list item should be its own `surface-container-low` block with a `3` (1rem) margin.

### The "Active State" Chip
Chips should use `secondary-container` for the background and `on-secondary-container` for the text. Use `md` (0.75rem) roundedness to differentiate from the `full` roundedness of primary buttons.

### Specific App Components:
- **The Playback Scrubber:** A custom `primary` gradient track with a `surface-bright` thumb. 
- **The Remote Module:** A large, nested `surface-container-highest` panel with glassmorphism, floating at the bottom of the viewport.

---

## 6. Do’s and Don’ts

### Do:
- **Do** overlap elements. Let a movie poster bleed out of a card container slightly onto the background to create 3D depth.
- **Do** use `on-surface-variant` (#adaaab) for secondary metadata to create a clear visual hierarchy.
- **Do** use `sm` (0.25rem) or `md` (0.75rem) roundedness for content (Posters/Thumbnails) and `full` for interactive UI (Buttons).

### Don’t:
- **Don't** use pure white (#ffffff) for body text over long paragraphs. It causes "halving" (visual vibration) on dark backgrounds. Use `on-surface` or `on-surface-variant`.
- **Don't** use "Drop Shadows" on cards. Use tonal shifts between `surface-container` tiers instead.
- **Don't** use standard system icons. Use sleek, thin-stroke (1.5px) outline-style icons to match the editorial typography.

### Accessibility Note:
While we utilize glassmorphism and low-contrast borders, ensure that all interactive text (Buttons and Titles) meets a minimum contrast ratio of 4.5:1 against their respective containers using the `primary` and `on-surface` tokens.