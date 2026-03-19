# Design System Document: The Luminous Overlay

## 1. Overview & Creative North Star: "The Ethereal Lens"
The Creative North Star for this design system is **"The Ethereal Lens."** We are moving away from the "app-in-a-box" aesthetic toward a UI that feels like a series of sophisticated, semi-transparent layers floating over a deep, intelligent base. 

Mobile overlays should never feel like an interruption; they should feel like a focused refinement of the current context. By utilizing intentional asymmetry, high-contrast typography, and depth-driven layering, we create a "High-End Editorial" experience that prioritizes content clarity and premium tactile feedback. We reject the rigid, bordered grid in favor of tonal transitions and breathing room.

---

## 2. Colors & Surface Architecture
Our palette centers on a sophisticated interplay between a deep, authoritative Blue (`primary: #0054cd`) and a vibrant, modern Teal (`secondary: #00696b`).

### The "No-Line" Rule
**Explicit Instruction:** Designers are prohibited from using 1px solid borders for sectioning or containment. 
*   **The Alternative:** Boundaries must be defined solely through background color shifts. For example, a `surface-container-low` (#f0f4f8) card sitting on a `surface` (#f6fafe) background. This creates a soft, sophisticated edge that feels "grown" rather than "drawn."

### Surface Hierarchy & Nesting
Treat the UI as a physical stack of fine materials.
*   **Base Layer:** Use `surface` (#f6fafe) for the overall application background.
*   **Secondary Content:** Use `surface-container-low` (#f0f4f8) for secondary grouping.
*   **Primary Overlays/Cards:** Use `surface-container-lowest` (#ffffff) to provide the highest natural "pop" against the background.
*   **Nesting:** When placing an element inside an overlay, use `surface-container-high` (#e4e9ed) to create an inset, "etched" look for input fields or secondary actions.

### The "Glass & Gradient" Rule
To achieve a signature look, floating overlays must utilize **Glassmorphism**.
*   **Implementation:** Use `surface` at 80% opacity with a `backdrop-blur` of 20px. 
*   **Signature Textures:** Main CTAs should not be flat. Apply a subtle linear gradient from `primary` (#0054cd) to `primary-container` (#316ee9) at a 135-degree angle. This adds "visual soul" and a sense of curvature to the button.

---

## 3. Typography: The Editorial Voice
We use a dual-font strategy to balance character with utility. **Manrope** provides a modern, geometric flair for high-impact moments, while **Inter** ensures maximum legibility for functional data.

*   **Display & Headlines (Manrope):** Use `display-lg` (3.5rem) and `headline-md` (1.75rem) with tight letter-spacing (-0.02em). These should be `on-surface` (#171c1f) to command attention. Use intentional asymmetry by left-aligning large headlines while right-aligning subtext to create a dynamic visual path.
*   **Titles & Body (Inter):** `title-md` (1.125rem) serves as the anchor for card headers. `body-md` (0.875rem) is the workhorse for all instructional text, utilizing `on-surface-variant` (#414754) to create a soft contrast.
*   **Labels (Inter):** Use `label-md` (0.75rem) in All Caps with +0.05em tracking for category tags or small metadata, ensuring they don't get lost despite their size.

---

## 4. Elevation & Depth: Tonal Layering
Traditional drop shadows are often "muddy." In this system, depth is a product of light and material.

*   **The Layering Principle:** Instead of a shadow, place a `surface-container-lowest` (#ffffff) element on a `surface-dim` (#d6dade) background. The change in luminance provides all the separation the human eye needs.
*   **Ambient Shadows:** For high-level overlays (modals/drawers), use an extra-diffused shadow: `box-shadow: 0 12px 40px rgba(23, 28, 31, 0.06)`. Note the 6% opacity; it should be felt, not seen.
*   **The "Ghost Border" Fallback:** If accessibility requirements demand a container edge, use a "Ghost Border": `outline-variant` (#c1c6d7) at **15% opacity**.
*   **Glassmorphism Depth:** When an overlay appears, the background should not just dim; it should blur. This maintains the "Luminous" quality of the color palette while isolating the user's focus.

---

## 5. Components: Style & Execution

### Buttons
*   **Primary:** High-contrast `primary` gradient with `on-primary` text. Use `xl` (1.5rem) roundedness for a pill-shape that feels friendly yet premium.
*   **Secondary:** `surface-container-highest` (#dfe3e7) background with `on-primary-fixed-variant` (#0040a1) text. No border.
*   **Tertiary:** Text-only using `secondary` (#00696b) with a 2px bottom margin that expands on tap.

### Input Fields
*   **Styling:** Forgo the bottom line. Use a `surface-container-high` (#e4e9ed) fill with `md` (0.75rem) corner radius. 
*   **States:** On focus, the background transitions to `surface-container-lowest` (#ffffff) with a 1px "Ghost Border" of `primary`.

### Cards & Lists
*   **The Divider Ban:** Strictly forbid 1px horizontal lines between list items. Use **Spacing Scale 4** (1rem) to separate items, or use alternating tonal shifts between `surface-container-low` and `surface`.
*   **Overlays:** Mobile drawers must use `xl` (1.5rem) top-corner radius only, creating a "sheet" effect that slides over the UI.

### Selection Chips
*   Use `secondary-container` (#56f5f8) with `on-secondary-container` (#006e70) for selected states. The high-saturation teal against the soft blue background creates a focal point that is impossible to miss.

---

## 6. Do's and Don'ts

### Do
*   **Do** use asymmetrical padding (e.g., more padding on the bottom of a card than the top) to create an editorial, "weighted" feel.
*   **Do** use `primary-fixed` (#dae2ff) for subtle highlights in dark-themed sections.
*   **Do** maximize the use of the Spacing Scale `8` (2rem) for "breathable" margins around overlays.

### Don't
*   **Don't** use pure black (#000000) for shadows or text; always use `on-surface` (#171c1f) to maintain the sophisticated blue-tinted tonal range.
*   **Don't** use the `DEFAULT` (0.5rem) rounding for buttons; go `full` or `xl` to maintain the "Ethereal" softness.
*   **Don't** use high-contrast borders for checkboxes; use `outline` (#717786) at low opacity and fill with `secondary` when checked.

---
*Director's Final Note: Precision is the difference between "clean" and "premium." Stick to the Spacing Scale religiously. If an element feels "off," it's likely because you haven't given it enough room to breathe.*