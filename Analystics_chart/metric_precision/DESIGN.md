# Design System Strategy: The Precision Curator

## 1. Overview & Creative North Star
The "Precision Curator" is a design system built to transform cold data into a high-end editorial experience. Moving beyond the "dashboard-in-a-box" aesthetic, this system treats analytics as a premium narrative. 

**Creative North Star: The Informed Whisper.** 
The design system emphasizes quiet authority through expansive white space, intentional asymmetry, and a rejection of traditional structural lines. Instead of "boxing in" data, we allow it to breathe within a sophisticated hierarchy of light and depth. By utilizing overlapping layers and a highly disciplined typographic scale, we move from "reporting" to "curating," ensuring that the most vital insights command the user's attention through visual gravity rather than visual noise.

---

## 2. Colors & Tonal Depth
The palette is a curated spectrum of professional depth. We utilize a "Primary" core of deep midnight blues (`primary: #00478d`), "Secondary" teals for stability (`secondary: #006a6a`), and "Tertiary" corals for high-impact alerts or divergent data series (`tertiary: #8d1620`).

### The "No-Line" Rule
Standard 1px borders are strictly prohibited for sectioning. Boundaries must be defined solely through background color shifts. For instance, a data visualization area using `surface_container_low` should sit directly against a `surface` background. This creates a "soft edge" that feels integrated into the interface rather than cordoned off.

### Surface Hierarchy & Nesting
Treat the UI as a physical stack of semi-translucent materials.
*   **Base Layer:** `surface` (#f8f9fa) – The canvas.
*   **Secondary Content:** `surface_container_low` (#f3f4f5) – For sidebar backgrounds or grouping secondary widgets.
*   **Primary Focus:** `surface_container_lowest` (#ffffff) – Reserved for the "Hero" charts and cards to provide maximum contrast.
*   **The Glass & Gradient Rule:** For floating headers or navigational elements, use `surface_container_lowest` at 85% opacity with a `backdrop-blur: 20px`. Main action buttons should utilize a subtle linear gradient from `primary` (#00478d) to `primary_container` (#005eb8) to add a three-dimensional "soul" to the touchpoint.

---

## 3. Typography
Our typography creates a clear dialogue between high-level brand storytelling and granular data density.

*   **Editorial Authority (Display & Headline):** We use **Manrope**. Its geometric yet slightly condensed nature feels modern and architectural. Use `display-lg` (3.5rem) for high-level total metrics and `headline-sm` (1.5rem) for section titles.
*   **Functional Clarity (Title, Body, Label):** We use **Inter**. Its neutral, high-legibility x-height is perfect for dense data. Use `label-md` (0.75rem) with `on_surface_variant` (#424752) for axis labels and chart legends.
*   **The Contrast Rule:** Pair `headline-md` (Manrope) for card titles with `body-sm` (Inter) for metadata descriptions to create a professional, editorial rhythm.

---

## 4. Elevation & Depth
In this design system, depth is a function of light, not lines.

*   **The Layering Principle:** To "lift" a component, move up the surface scale. A `surface_container_lowest` card placed on a `surface_container` background creates an organic lift.
*   **Ambient Shadows:** For floating modals or "active" states, use an extra-diffused shadow: `box-shadow: 0 24px 48px -12px rgba(25, 28, 29, 0.06)`. Note the use of `on_surface` (#191c1d) as the shadow tint rather than pure black.
*   **The Ghost Border:** If containment is required for high-density charts, use the "Ghost Border": `outline_variant` (#c2c6d4) at 20% opacity. This provides a whisper of a boundary without interrupting the flow of white space.

---

## 5. Components & Data Visualization

### Data Cards
*   **Structure:** No borders. Use `surface_container_lowest` and `xl` (0.75rem) roundedness.
*   **Spacing:** Use `spacing-6` (2rem) internal padding to ensure the data doesn't feel "cramped."
*   **Content:** Lead with a `display-sm` metric, followed by a `label-sm` trend indicator.

### Line & Bar Charts
*   **Data Series:** Use `primary` (Blue) for the main series, `secondary` (Teal) for comparisons, and `tertiary_fixed_dim` (Soft Coral) for target lines or anomalies.
*   **Grid Lines:** Prohibit vertical grid lines. Horizontal lines must use `outline_variant` at 10% opacity.
*   **Line Styling:** Use a 2.5px stroke width for line charts with a subtle `primary_container` glow (glow radius: 8px) to emphasize the current data path.

### Interactive Elements
*   **Buttons:** `primary` buttons use the `lg` (0.5rem) roundedness. Text should be `label-md` in semi-bold.
*   **Chips:** Use `surface_container_high` backgrounds with no border. When selected, transition to `secondary_container` with `on_secondary_container` text.
*   **Input Fields:** Use `surface_container_low` for the field fill. On focus, transition to a `primary` "Ghost Border" (20% opacity) rather than a solid heavy line.

### Segmented Controls (Custom Component)
For toggling timeframes (1D, 1W, 1M), use a pill-shaped (`full` roundedness) container in `surface_container`. The active state should be a `surface_container_lowest` "floating" card with an ambient shadow, creating a tactile, high-end feel.

---

## 6. Do’s and Don’ts

### Do
*   **Do** use `spacing-12` (4rem) or `spacing-16` (5.5rem) between major sections to emphasize a premium, "un-crowded" feel.
*   **Do** use `tertiary` (#8d1620) sparingly—only for data points that require immediate cognitive intervention.
*   **Do** favor asymmetric layouts. For example, a large chart on the left (spanning 8 columns) balanced by a vertical stack of key insights on the right (4 columns).

### Don't
*   **Don't** use 100% black (#000000) for text. Always use `on_surface` (#191c1d) to maintain a soft, sophisticated contrast.
*   **Don't** use dividers or lines to separate list items. Use `spacing-3` (1rem) and subtle `surface` background shifts on hover.
*   **Don't** use "Standard" shadows. If a shadow feels visible at first glance, it is too heavy. It should be felt, not seen.