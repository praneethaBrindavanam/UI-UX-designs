# Design System Specification: Editorial Softness & Layered Trust

## 1. Overview & Creative North Star: "The Fluid Concierge"
This design system moves away from the rigid, boxy constraints of traditional mobile onboarding. The Creative North Star is **"The Fluid Concierge"**—an experience that feels less like a technical setup and more like a high-end hospitality greeting. 

We break the "template" look through **Intentional Asymmetry** and **Tonal Depth**. By leaning into the `plusJakartaSans` display scale and generous white space, we create an editorial rhythm. Screens should never feel "filled"; they should feel "composed." We use overlapping elements and varying surface heights to guide the user’s eye naturally through the onboarding flow, favoring soft transitions over jarring step-changes.

---

## 2. Colors & Surface Architecture
Our palette uses a sophisticated Indigo (`primary: #4a40e0`) paired with a soft, tinted background (`background: #faf4ff`). This isn't just "white and blue"—it's a calculated hierarchy of warmth and authority.

### The "No-Line" Rule
**Strict Mandate:** Designers are prohibited from using 1px solid borders to define sections. Layout boundaries must be achieved through background shifts. 
*   *Example:* A `surface-container-low` section sitting directly on a `surface` background creates a sophisticated, "pressed" look without the visual clutter of lines.

### Surface Hierarchy & Nesting
Treat the UI as physical layers of fine paper. 
*   **Base:** `surface` (#faf4ff)
*   **Secondary Content:** `surface-container-low` (#f5eeff)
*   **Interactive Cards:** `surface-container-lowest` (#ffffff) to create a "lifted" feel.
*   **High-Priority Modals:** `surface-container-highest` (#e2d7ff) for maximum contrast against the base.

### The "Glass & Gradient" Rule
To avoid a flat, "out-of-the-box" appearance:
*   **Main CTAs:** Use a subtle linear gradient from `primary` (#4a40e0) to `primary_dim` (#3d30d4) at a 135° angle.
*   **Floating Elements:** Use `surface_container_lowest` with an 80% opacity and a `20px` backdrop-blur to create a "frosted glass" effect for navigation bars or floating action buttons.

---

## 3. Typography: Editorial Authority
The interplay between **Plus Jakarta Sans** (Display) and **Manrope** (Body) is the system’s heartbeat.

*   **Display & Headlines (Plus Jakarta Sans):** Used for "The Hook." These should be set with tight letter-spacing (-2%) to feel premium and authoritative. Use `display-md` for welcome screens to create an immediate impact.
*   **Body & Labels (Manrope):** Chosen for its exceptional legibility at small sizes. Use `body-lg` for onboarding instructions to ensure the "Friendly" vibe is maintained through readability.
*   **Tonal Contrast:** Always pair a `headline-lg` in `on_surface` (#32294f) with a `body-md` in `on_surface_variant` (#5f557f). This 20% drop in contrast for body text creates a natural visual hierarchy that signals "Headlines first, details second."

---

## 4. Elevation & Depth: Tonal Layering
We reject traditional heavy drop shadows. Depth is an atmosphere, not a decoration.

*   **The Layering Principle:** Achieve depth by "stacking." Place a `surface_container_lowest` card on a `surface_container` background. The slight shift in hex value creates a soft, natural lift.
*   **Ambient Shadows:** If a shadow is required for a floating CTA, use: `Y: 8px, Blur: 24px, Color: rgba(74, 64, 224, 0.08)`. This tints the shadow with our `primary` color, making it feel like light is passing through the element rather than a grey "dirt" mark.
*   **The Ghost Border Fallback:** For high-density inputs, use a 1px border with `outline_variant` at **15% opacity**. It should be felt, not seen.

---

## 5. Components

### Buttons (The "Pill" Signature)
*   **Primary:** Full rounded (`9999px`), `primary` background, `on_primary` text. Use `spacing-4` (1.4rem) horizontal padding.
*   **Secondary:** `surface_container_high` background with `on_secondary_container` text. No border.
*   **States:** On press, shift from `primary` to `primary_dim`.

### Input Fields (The "Soft Nest")
*   **Structure:** Use `surface_container_low` as the field background. 
*   **Corners:** `md` (0.75rem).
*   **Interaction:** On focus, the background shifts to `surface_container_lowest` and a "Ghost Border" of `primary` at 20% opacity appears.

### Cards & Lists
*   **No Dividers:** Forbid the use of horizontal lines. Use `spacing-3` (1rem) or `spacing-4` (1.4rem) of vertical white space to separate items.
*   **Progress Indicators:** Use the `tertiary` (#983772) color for progress dots to provide a "spark" of unexpected color that keeps the onboarding feeling modern and vibrant.

### Selection Chips
*   **Unselected:** `surface_container_highest` with `on_surface_variant`.
*   **Selected:** `primary` background with `on_primary` text. Apply a `xl` (1.5rem) corner radius for a friendly, organic feel.

---

## 6. Do’s and Don’ts

### Do:
*   **Do** use asymmetrical margins. For example, a headline might have a `spacing-8` left margin while the body text below it has `spacing-10` to create an editorial "staircase" effect.
*   **Do** use `primary_container` (#9795ff) for low-priority background accents to keep the "vibrant" brand promise without overwhelming the user.
*   **Do** lean into the `lg` (1rem) and `xl` (1.5rem) corner radii for a welcoming, approachable UI.

### Don’t:
*   **Don’t** use pure black (#000000) for text. Always use `on_surface` (#32294f) to maintain the "Soft Indigo" tonal warmth.
*   **Don’t** stack more than three layers of surfaces. It breaks the "Fluid Concierge" simplicity.
*   **Don’t** use standard Material Design "Drop Shadows." If it looks like a default setting, it’s wrong for this system. Use Tonal Layering first.