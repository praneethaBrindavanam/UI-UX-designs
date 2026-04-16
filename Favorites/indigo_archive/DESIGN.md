# Design System Document: The Curated Archive

## 1. Overview & Creative North Star
**Creative North Star: "The Digital Concierge"**
This design system is built to transform a simple list of favorites into a high-end, editorial gallery. We move away from the "utility-first" look of standard apps and embrace the "curation-first" philosophy of premium lifestyle journals.

The experience is defined by **Atmospheric Depth** and **Intentional Asymmetry**. We do not use rigid, boxy grids that feel like spreadsheets. Instead, we use varying card heights, overlapping imagery, and bold typographic scales to create a rhythm that feels human and curated. The goal is to make the user feel like they are flipping through a bespoke coffee-table book of their own interests.

---

## 2. Colors: Tonal Depth & Category Accents
The palette is rooted in a deep, nocturnal base to allow the category-specific accents to "glow" with purpose.

### The "No-Line" Rule
**Strict Mandate:** Designers are prohibited from using 1px solid borders for sectioning. Structural boundaries must be defined solely through background color shifts or tonal transitions.
- **Example:** A list item does not have a bottom border; it sits as a `surface-container-low` element against a `surface` background.

### Surface Hierarchy & Nesting
Treat the UI as physical layers of frosted material.
*   **Base Layer:** `surface` (#0e0e0e) - The canvas.
*   **Secondary Layer:** `surface-container-low` (#131313) - Large grouping areas.
*   **Focus Layer:** `surface-container` (#1a1919) - Standard card backgrounds.
*   **Action Layer:** `surface-container-highest` (#262626) - Hover states or active selections.

### The "Glass & Gradient" Rule
To elevate beyond flat design, use **Glassmorphism** for floating navigation and overlays.
*   **Floating Elements:** Use `surface-container-high` with 80% opacity and a `24px` backdrop blur.
*   **Signature Textures:** Apply a subtle linear gradient from `primary` (#a4a6ff) to `primary-dim` (#6062f2) on hero CTAs to provide a "soulful" glow.

### Category Color Logic
*   **Teal (Secondary - Books):** Use `secondary` (#62fae3) for literature.
*   **Purple (Primary - Games):** Use `primary` (#a4a6ff) for interactive media.
*   **Orange (Tertiary - Podcasts):** Use `tertiary` (#ffa765) for audio content.

---

## 3. Typography: Editorial Authority
We utilize a triad of typefaces to establish a clear, sophisticated hierarchy.

*   **Display & Headlines (Manrope):** Use for category titles and large hero headers. The geometric nature of Manrope provides a modern, architectural feel. 
    *   *Scale:* `display-lg` (3.5rem) for empty states; `headline-md` (1.75rem) for category headings.
*   **Titles & Body (Plus Jakarta Sans):** Chosen for its high x-height and exceptional legibility in grid views. 
    *   *Scale:* `title-md` (1.125rem) for item names; `body-md` (0.875rem) for descriptions.
*   **Labels (Inter):** Reserved for metadata and utility text. 
    *   *Scale:* `label-md` (0.75rem) for timestamps, "Read Time," or "Episode Length."

---

## 4. Elevation & Depth
We eschew traditional drop shadows in favor of **Tonal Layering**.

*   **The Layering Principle:** Depth is achieved by "stacking." Place a `surface-container-lowest` card on a `surface-container-low` section to create a soft, natural lift.
*   **Ambient Shadows:** For "Floating" elements (like a FAB), use a highly diffused shadow: `0px 20px 40px rgba(0, 0, 0, 0.4)`. The shadow must feel like an occlusion of light, not a dark smudge.
*   **The "Ghost Border" Fallback:** If a border is required for accessibility, use `outline-variant` (#484847) at **15% opacity**. Never use 100% opaque borders.

---

## 5. Components

### Cards (The "Editorial Tile")
*   **Structure:** No borders. Use `md` (0.75rem) corner radius. 
*   **Visuals:** Backgrounds use `surface-container`. On hover, shift to `surface-container-high`.
*   **Content:** Avoid divider lines. Use `1.5rem` (xl) vertical spacing between meta-data blocks to separate content.

### Buttons (The "Luminous Action")
*   **Primary:** Gradient of `primary` to `primary-container`. Text: `on-primary` (#1100a3). Radius: `full`.
*   **Secondary:** Ghost style. Transparent background with a `Ghost Border` (outline-variant at 20%).
*   **Tertiary:** Text-only using `primary` color, reserved for low-emphasis actions.

### Category Chips
*   **State:** Pill-shaped (`full` radius). 
*   **Coloring:** For a "Books" chip, use a container of `on-secondary` at 10% opacity with `secondary` (#62fae3) text. This creates a sophisticated "tinted" look rather than a heavy solid block.

### Input Fields
*   **Styling:** Fill-only. Use `surface-container-highest` (#262626). 
*   **Indicator:** A 2px bottom bar in `primary` appears only on focus.

### Additional Component: The "Progressive Blur" Header
*   As the user scrolls, the top navigation should transition from transparent to `surface-container` with a `blur(12px)` effect, allowing the vibrant category colors of the content to bleed through softly as they pass underneath.

---

## 6. Do's and Don'ts

### Do
*   **Do** use asymmetrical spacing. If the left margin is 2rem, try a 3rem right margin for hero elements to create editorial tension.
*   **Do** lean into "High Contrast" typography. Pair a `display-sm` headline with a `label-sm` metadata tag immediately below it.
*   **Do** use `surface-tint` sparingly to add a subtle wash of color to large dark background areas.

### Don't
*   **Don't** use 1px dividers. If content feels cluttered, increase the white space using the `xl` (1.5rem) scale.
*   **Don't** use pure white (#ffffff) for body text. Use `on-surface-variant` (#adaaaa) to reduce eye strain and maintain the "premium" dark aesthetic.
*   **Don't** use standard "drop shadows" on cards. Rely on color steps between `surface` tiers to define edges.