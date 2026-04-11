# Design System Document: The Editorial Trust System

## 1. Overview & Creative North Star
**Creative North Star: "The Curated Perspective"**

This design system moves away from the sterile, "template" feel of traditional SaaS reviews. Instead, it adopts a high-end editorial approach. We treat every testimonial not as a data point, but as a feature story. By utilizing intentional white space, sophisticated tonal layering, and an authoritative typographic scale, we transform "social proof" into a premium brand asset. 

The goal is to break the rigid grid. We achieve this through **Asymmetric Balance**—placing elements like star ratings or author avatars in unexpected but intentional positions—to guide the eye through a narrative rather than a list.

---

## 2. Colors: Tonal Depth & The "No-Line" Rule
The palette is built on a foundation of sophisticated neutrals (`surface` to `surface-dim`) to establish trust, punctuated by a commanding blue (`primary`) and a warm, golden accent (`tertiary`) reserved exclusively for validation and ratings.

### The "No-Line" Rule
**Explicit Instruction:** Prohibit the use of 1px solid borders for sectioning. 
Structure must be defined solely through background color shifts. For example, a testimonial card (`surface-container-lowest`) should sit on a `surface-container-low` section. Boundaries are felt, not seen.

### Surface Hierarchy & Nesting
Treat the UI as physical layers of fine paper. 
- **Base Layer:** `surface` (#f7f9fb)
- **Content Blocks:** `surface-container` (#eceef0)
- **High-Priority Cards:** `surface-container-lowest` (#ffffff) for maximum "lift" and perceived cleanliness.

### The "Glass & Gradient" Rule
To add "soul" to the professional palette, use subtle gradients for primary actions. A linear transition from `primary` (#2b4bb9) to `primary_container` (#4865d3) creates a soft, convex volume that feels tactile and premium. For floating overlays, apply a backdrop-blur (12px–20px) with a semi-transparent `surface_variant` to achieve a frosted glass effect.

---

### 3. Typography: The Friendly Authority
We use a dual-typeface system to balance professional rigor with approachable warmth.

*   **Display & Headlines (Manrope):** A geometric sans-serif that feels modern and structured. Use `display-md` for hero quotes to command attention.
*   **Body & Labels (Be Vietnam Pro):** A highly legible typeface with a friendly, open aperture. 

**Hierarchy as Identity:**
- **The Quote:** `headline-sm` in `on_surface`. High contrast, tight tracking (-0.02em).
- **The Attribution:** `title-sm` for names, `label-md` for job titles in `secondary`.
- **The Validation:** Ratings use `tertiary` (#784b00) to stand out against the cool grays without the "danger" associated with reds or oranges.

---

## 4. Elevation & Depth: Tonal Layering
Traditional drop shadows are often a crutch for poor layout. In this system, we prioritize **Tonal Layering**.

*   **The Layering Principle:** Depth is achieved by stacking. A `surface-container-lowest` card placed on a `surface-container-high` background creates a natural, crisp edge that communicates hierarchy without visual noise.
*   **Ambient Shadows:** If a card must "float" (e.g., a hover state), use a shadow color tinted with the `on_surface` value at 4% opacity with a 32px blur. It should feel like natural light, not a digital effect.
*   **The "Ghost Border" Fallback:** If accessibility requires a container boundary, use `outline_variant` (#c3c6d7) at **15% opacity**. 100% opaque borders are strictly forbidden.

---

## 5. Components

### Testimonial Cards
*   **Structure:** No dividers. Use `md` (0.75rem) or `lg` (1rem) corner radius. 
*   **Asymmetry:** Position the rating `tertiary` stars in the top-right "margin" of the card, breaking the standard left-aligned text block.
*   **Background:** Use `surface-container-lowest` to make the testimonial pop against the `background` (#f7f9fb).

### Buttons
*   **Primary:** Gradient of `primary` to `primary_container`. White text (`on_primary`). `full` (pill) roundedness for a friendly, modern touch.
*   **Secondary:** `surface-container-high` background with `primary` text. No border.

### Ratings & Chips
*   **Rating Stars:** Always `tertiary`. For "empty" stars, use `tertiary_fixed_dim` at 30% opacity.
*   **Category Chips:** Use `secondary_container` with `on_secondary_container` text. Keep these small (`label-sm`) to ensure they don't compete with the testimonial text.

### Input Fields (Review Submission)
*   **Field Style:** Use `surface-container-low` as the fill. On focus, transition the background to `surface_container_lowest` and add a 1px "Ghost Border" using `primary`.
*   **Labeling:** `label-md` in `secondary` placed 8px above the field.

---

## 6. Do's and Don'ts

### Do
*   **DO** use whitespace as a structural element. A 64px gap is often better than a line.
*   **DO** use `surface-dim` for secondary footer areas to "ground" the page.
*   **DO** overlap elements slightly (e.g., an avatar overlapping the edge of a card) to create a custom, editorial feel.

### Don't
*   **DON'T** use pure black (#000000) for text. Always use `on_surface` (#191c1e) to maintain a premium, soft-contrast look.
*   **DON'T** use default 1px borders. If you feel the need for a line, try a background color shift first.
*   **DON'T** use high-saturation yellows for ratings. Stick to the sophisticated `tertiary` gold-brown tones provided.

---

## 7. Signature Interaction: The "Soft Lift"
When a user hovers over a testimonial card, do not move the card or change the border. Instead, subtly shift the background from `surface-container-lowest` to `surface-bright`. This "glow" effect feels more sophisticated and less "bouncy" than traditional UI animations.