# Design System Strategy: The Elevated Explorer

## 1. Overview & Creative North Star: "The Digital Curator"
This design system moves away from the cluttered, transactional nature of traditional travel booking and toward the refined, spacious feel of a high-end editorial magazine. Our Creative North Star is **The Digital Curator**. 

We do not just show lists; we present destinations as curated exhibits. To achieve this, we break the "standard template" look through **intentional asymmetry**—using staggered image grids and oversized typography that overlaps container edges. By embracing white space as a functional element rather than "empty" space, we create an atmosphere of luxury, trust, and breathing room.

## 2. Color & Surface Architecture
The palette is rooted in a "Vibrant Professionalism." We use blue not as a utility, but as a signature accent that guides the eye.

### The "No-Line" Rule
**Explicit Instruction:** 1px solid borders are strictly prohibited for sectioning or card definition. Boundaries must be defined through background tonal shifts. Use `surface-container-low` for a section background sitting on a `surface` base. If an element needs to stand out, use `surface-container-lowest` (#ffffff) to create a natural, "lifted" feel against the slightly tinted `surface` (#faf8ff).

### Surface Hierarchy & Nesting
Treat the UI as a series of stacked, physical layers. 
- **Base Layer:** `surface` (#faf8ff)
- **Content Sections:** `surface-container-low` (#f2f3ff)
- **Interactive Cards:** `surface-container-lowest` (#ffffff)
- **Top-Level Modals/Sheets:** `surface-bright` (#faf8ff)

### The "Glass & Gradient" Rule
To avoid a flat, "Bootstrap" appearance, use **Glassmorphism** for floating elements like navigation bars or search overlays. Apply `surface` at 80% opacity with a `24px` backdrop blur. For primary CTAs, use a subtle linear gradient transitioning from `primary` (#0050cb) to `primary_container` (#0066ff) at a 135-degree angle to provide "soul" and depth.

## 3. Typography: Editorial Authority
We pair the geometric precision of **Plus Jakarta Sans** for headlines with the high readability of **Inter** for utility and body text.

*   **Display & Headlines (Plus Jakarta Sans):** These are your "Editorial Voice." Use `display-lg` (3.5rem) for hero destination titles. Don't be afraid to use tight letter-spacing (-0.02em) to give it a premium, compressed look.
*   **Body & Labels (Inter):** These are your "Utility Voice." Use `body-md` (0.875rem) for descriptions. Ensure a line height of at least 1.6 for body text to maintain the "Airy" aesthetic.
*   **Hierarchy Tip:** Use `tertiary` (#a33200) for small "Discovery" labels (e.g., "Trending Now") to provide a high-contrast spark against the sea of blue and white.

## 4. Elevation & Depth: Tonal Layering
We reject heavy, muddy shadows. Depth is an atmosphere, not a drop-shadow effect.

*   **The Layering Principle:** A `surface-container-lowest` card placed on a `surface-container-low` background creates a "Ghost Lift." This is our primary method of separation.
*   **Ambient Shadows:** For floating elements (like a "Book Now" bar), use a multi-layered shadow:
    *   Shadow 1: `0px 4px 20px rgba(25, 27, 36, 0.04)`
    *   Shadow 2: `0px 12px 40px rgba(25, 27, 36, 0.08)`
*   **The Ghost Border Fallback:** If accessibility requires a border, use `outline_variant` (#c2c6d8) at **15% opacity**. It should be felt, not seen.
*   **Roundedness:** Stick to the `xl` (1.5rem / 24px) for large imagery and `lg` (1rem / 16px) for standard cards to maintain the "Gentle" promise of the brief.

## 5. Components & Components

### Buttons
*   **Primary:** Gradient fill (`primary` to `primary_container`), `xl` roundedness, white text. No shadow on rest; subtle `primary_fixed` glow on hover.
*   **Secondary:** `surface-container-high` background with `on_secondary_container` text. No border.
*   **Tertiary:** Purely typographic using `primary` color, with a `2.5` spacing unit (0.85rem) horizontal padding.

### Cards & Discovery Lists
*   **Rule:** Forbid divider lines. Use `spacing-6` (2rem) of vertical white space to separate list items.
*   **Imagery:** Images must use `rounded-xl`. Overlay destination names using a `surface` glassmorphism badge in the bottom-left corner, rather than a full-width text bar.

### Input Fields (Search)
*   **Style:** Use `surface-container-lowest` with a "Ghost Border." On focus, the border transitions to `primary` at 40% opacity, and the shadow increases to the Ambient Shadow spec. Use `label-md` for floating labels.

### Additional Travel Components
*   **The "Vibe" Chip:** A selection chip using `secondary_container` with `on_secondary_container` text. Used for filtering "Beach," "Mountain," or "Urban."
*   **Price Floating Action Button (FAB):** A small, high-elevation circle using `tertiary` to highlight the best price in a search result, breaking the blue/white rhythm.

## 6. Do's and Don'ts

### Do:
*   **Do** use asymmetrical image heights (e.g., one tall 3:4 image next to two 1:1 square images) to create a gallery feel.
*   **Do** bleed high-quality imagery off the edge of the screen in mobile carousels to signal horizontal scroll.
*   **Do** use `primary_fixed` (#dae1ff) as a background for "Tips" or "Insight" callouts to keep them distinct but trustworthy.

### Don't:
*   **Don't** use 100% black text. Always use `on_surface` (#191b24) to keep the contrast sophisticated, not harsh.
*   **Don't** use standard 8px rounding. It looks like a default framework. Stick to our `lg` (16px) and `xl` (24px) tokens.
*   **Don't** crowd the edges. If a container feels full, increase padding using the `spacing-5` (1.7rem) or `spacing-6` (2rem) tokens.