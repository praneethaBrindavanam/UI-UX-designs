# Design System Document: Kinetic Luxury

## 1. Overview & Creative North Star: "The Digital Atelier"
This design system is not a mere utility; it is a high-performance stage. Our Creative North Star is **"The Digital Atelier"**—a space that blends the raw, high-octane energy of street culture with the precision of a luxury design studio. 

To move beyond the "template" look, we reject rigid, boxed-in layouts. We embrace **Intentional Asymmetry** and **Tonal Depth**. By utilizing overlapping elements (e.g., a high-resolution sneaker silhouette breaking the container bounds) and a drastic typography scale, we create a sense of forward motion. The interface should feel like a premium editorial magazine—spacious, authoritative, and fast.

---

## 2. Colors & Surface Philosophy
The palette is rooted in a high-contrast tension between `background (#0e0e11)` and `primary (#94aaff)`. 

### The "No-Line" Rule
**Prohibit 1px solid borders for sectioning.** Physical dividers feel static and "cheap." Boundaries must be defined solely through background color shifts. For instance, a `surface-container-low` section sitting on a `surface` background provides all the separation necessary.

### Surface Hierarchy & Nesting
Treat the UI as a series of physical layers. We use the surface-container tiers to create "nested" depth:
*   **Base:** `surface` (#0e0e11)
*   **Secondary Sections:** `surface-container-low` (#131316)
*   **Interactive Cards:** `surface-container-high` (#1f1f23)
*   **Elevated Overlays:** `surface-container-highest` (#25252a)

### The "Glass & Gradient" Rule
To inject "soul" into the digital experience, use **Glassmorphism** for floating navigation and customization menus. Apply `surface-variant` at 60% opacity with a `20px` backdrop blur. 
*   **Signature Gradient:** For primary CTAs, use a linear gradient from `primary (#94aaff)` to `primary-dim (#3467ff)` at a 135-degree angle. This mimics the sheen of technical fabrics.

---

## 3. Typography: Editorial Impact
We utilize a dual-typeface system to balance "Athletic Brutalism" with "Technical Precision."

*   **Display & Headlines (Epilogue):** This is our "voice." Use `display-lg` for product names and hero sections. The tight kerning and heavy weight of Epilogue convey power and premium status.
*   **Body & UI (Inter):** Inter handles the "data." It is optimized for readability during the customization process.
*   **The Scale of Authority:** Use extreme contrast. Pair a `display-lg` headline with a `label-md` uppercase caption to create an editorial, high-fashion aesthetic.

---

## 4. Elevation & Depth: Tonal Layering
We move away from the traditional "drop shadow" in favor of **Ambient Tonalism.**

*   **The Layering Principle:** Depth is achieved by stacking. Place a `surface-container-lowest` card on a `surface-container-low` section to create a soft, natural lift.
*   **Ambient Shadows:** If a floating effect is required (e.g., a floating "Add to Cart" bar), shadows must be extra-diffused. 
    *   *Shadow:* `0px 24px 48px rgba(0, 0, 0, 0.5)`. 
*   **The "Ghost Border" Fallback:** If a border is required for accessibility, use `outline-variant` at 15% opacity. Never use 100% opaque borders.
*   **Motion Depth:** When a user interacts with a sneaker component, the surrounding UI should recede using a slight `0.98x` scale down and an increase in backdrop blur on underlying layers.

---

## 5. Components

### Buttons (The Kinetic Trigger)
*   **Primary:** Uses the **Signature Gradient** (Primary to Primary-Dim). `borderRadius: md (0.375rem)`. Text is `on-primary-fixed` (Black) for maximum legibility.
*   **Secondary:** `surface-container-highest` background with `on-surface` text. No border.
*   **Tertiary:** Transparent background, `on-surface` text, underlined only on hover.

### Customization Chips
*   **Selection Chips:** Use `secondary-container` for the unselected state. Upon selection, animate to `primary` with a subtle `primary-dim` outer glow.
*   **Sizing:** All chips use `borderRadius: full` for a sleek, athletic feel.

### Input Fields (The Technical Spec)
*   **Styling:** Forbid traditional "box" inputs. Use a `surface-container-high` background with a `Ghost Border`. 
*   **Active State:** The bottom border transforms into a 2px `primary` line.

### Cards & Lists (The Gallery)
*   **Constraint:** Forbid divider lines.
*   **Execution:** Use `48px` of vertical whitespace (from the spacing scale) to separate list items. For product cards, use `surface-container-low` with `borderRadius: xl (0.75rem)`.
*   **Dynamic Component - "The Customizer Tray":** A bottom-anchored, glassmorphic container using `surface-variant` @ 70% opacity, allowing the sneaker photography to bleed through the UI controls.

---

## 6. Do’s and Don’ts

### Do:
*   **Do** use extreme whitespace (e.g., 80px+) between major sections to let product photography "breathe."
*   **Do** overlap elements. A sneaker image should partially cover a background `display-lg` title.
*   **Do** use `primary` sparingly. It is a high-energy "laser," not a background wash.

### Don’t:
*   **Don't** use 1px solid dividers or high-contrast borders. It breaks the premium "flow."
*   **Don't** use standard "Material Design" shadows. They are too muddy for this high-gloss aesthetic.
*   **Don't** crowd the interface. If the user is customizing a heel-tab, hide the lace-selector UI to maintain focus.

### Accessibility Note:
While we utilize deep blacks and vibrant blues, ensure all functional text (Labels, Body) maintains a contrast ratio of at least 4.5:1 against their respective `surface-container` tiers. Use `on-surface-variant` only for non-essential decorative metadata.