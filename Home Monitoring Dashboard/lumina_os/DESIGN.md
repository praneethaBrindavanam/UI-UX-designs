# Design System: Premium Smart Home OS

## 1. Overview & Creative North Star
**Creative North Star: "The Ethereal Guardian"**

The objective of this design system is to move away from the "industrial utility" of traditional home monitoring and toward a "living digital environment." By blending the high-tech precision of glassmorphism with the warmth of organic movement, we create a dashboard that feels less like a tool and more like a sophisticated companion. 

We break the "template" look by rejecting rigid borders and standard grids. Instead, we use **Intentional Asymmetry**—where a hero climate card might be larger and more deeply blurred than a row of energy toggles—and **Layered Translucency** to suggest depth. This isn't just a flat UI; it is a stack of optical layers that respond to the user's touch.

---

## 2. Colors & Surface Philosophy
The palette is rooted in deep obsidian tones (`surface: #0e0e10`) to provide a high-contrast canvas for our vibrant tech accents.

### The "No-Line" Rule
**Explicit Instruction:** Traditional 1px solid borders are strictly prohibited for sectioning. Boundaries must be defined solely through:
- **Background Shifts:** Placing a `surface-container-low` component on a `surface` background.
- **Tonal Transitions:** Using the delta between `surface-container` and `surface-bright` to imply an edge.

### Surface Hierarchy & Nesting
Think of the UI as physical sheets of frosted glass. 
- **Base Layer:** `surface` (#0e0e10).
- **Secondary Sections:** `surface-container-low` (#131315).
- **Actionable Cards:** `surface-container` (#19191c) or `surface-container-high` (#1f1f22).
- **Active/Floating States:** `surface-bright` (#2c2c2f).

### The "Glass & Gradient" Rule
To achieve the signature "Smart Home OS" feel, all floating cards must use **Glassmorphism**:
- **Background:** Semi-transparent versions of `surface-variant` (approx 60% opacity).
- **Backdrop-Blur:** Minimum 20px to 40px blur.
- **Signature Textures:** For high-impact areas (like Energy Savings), use a subtle linear gradient from `secondary` (#6ffb85) to `secondary-container` (#006e28) at a 15-degree angle to add "soul" to the data.

---

## 3. Typography
We use a dual-font strategy to balance technical precision with editorial elegance.

*   **Display & Headlines (Manrope):** Used for large data points and room names. Manrope’s geometric nature feels architectural and premium. Use `display-lg` (3.5rem) for critical home metrics (e.g., Temperature numbers).
*   **Body & Labels (Inter):** The workhorse for readability. Inter's tall x-height ensures that even at `body-sm` (0.75rem), status updates remain legible under heavy blur effects.

**Hierarchy as Identity:** 
High-contrast scale is key. Pair a `display-md` temperature value with a `label-md` "Target 72°" text to create a clear, sophisticated information hierarchy that feels like a high-end magazine layout.

---

## 4. Elevation & Depth
Depth is achieved through physics-based layering rather than artificial structure.

*   **The Layering Principle:** Stack `surface-container-lowest` cards on a `surface-container-low` section. The change in hex value provides a soft, natural lift.
*   **Ambient Shadows:** For "floating" elements like modals or active light controls, use a shadow with a 32px blur, 0% spread, and 6% opacity. The shadow color must be a tinted version of `on-surface`, never pure black.
*   **The "Ghost Border" Fallback:** If a container requires further definition (e.g., in high-glare environments), use the `outline-variant` token at **15% opacity**. A 100% opaque border is a failure of the system.
*   **Glass Interaction:** When a card is pressed, increase the backdrop-blur and shift the color from `surface-container` to `surface-bright` to mimic the glass physically moving closer to the user.

---

## 5. Components

### Buttons & Interaction
*   **Primary (Tech Blue):** Uses `primary` (#84adff) with `on-primary` (#002d64) text. 
*   **Secondary (Energy Green):** Uses `secondary` (#6ffb85) for sustainability actions.
*   **Tertiary (Climate Orange):** Uses `tertiary` (#ffa84f) for environmental alerts.
*   **Style:** Buttons should use the `full` (9999px) roundedness for a friendly, approachable feel.

### Input Fields & Controls
*   **Text Inputs:** No bottom line or box. Use a `surface-container-high` background with `xl` (1.5rem) corner radius.
*   **Checkboxes/Radios:** Use `primary` for active states. The "fun" element comes from a subtle bounce animation (0.3s cubic-bezier) when toggled.

### Cards & Data Lists
*   **Strict Rule:** No dividers. Use `spacing-4` (1.4rem) or `spacing-6` (2rem) of vertical white space to separate list items.
*   **Nesting:** Group related devices (e.g., all Bedroom lights) inside a `surface-container-low` wrapper to visually unify them without using a border.

### Smart Home Contextual Components
*   **Glance-Bars:** Ultra-thin horizontal progress bars for energy usage using `secondary_dim` on a `surface-variant` track.
*   **Status Orbs:** Pulsing glows using `primary_container` (blue) or `tertiary_container` (orange) to indicate active monitoring.

---

## 6. Do’s and Don’ts

### Do:
*   **Embrace Space:** Use `spacing-10` and `spacing-12` between major functional blocks to let the "Glass" breathe.
*   **Use Tonal Shifts:** Define zones by moving from `surface-container-lowest` to `surface-container-highest`.
*   **Color as Meaning:** Reserve `tertiary` (orange) strictly for climate/warmth and `secondary` (green) for energy efficiency.

### Don’t:
*   **Don’t use 1px Borders:** Never use a solid line to separate content. It breaks the "Ethereal" illusion.
*   **Don’t Over-Shadow:** If three elements are on the same plane, they should not have shadows. Only "floating" interactive layers get shadows.
*   **Don’t Use Pure Black/White:** Use the designated `surface` (#0e0e10) and `on-surface` (#fefbfe) to maintain the sophisticated, high-end tech aesthetic.