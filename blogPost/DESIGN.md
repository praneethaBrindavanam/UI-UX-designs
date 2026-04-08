```markdown
# Design System Specification: The Electric Editorial

## 1. Overview & Creative North Star
**Creative North Star: "Kinetic Elegance"**

This design system is engineered to break the monotony of the standard SaaS grid. It translates "vibrant and modern" not through chaotic color, but through **intentional asymmetry, high-energy typography scales, and sophisticated tonal layering.** 

We move beyond the "template" look by treating the screen as a high-end digital editorial. This means aggressive whitespace, overlapping elements that create a sense of forward motion, and a refusal to use traditional containment lines. The goal is a "premium-promotional" feel—one that captures immediate attention while maintaining the poise of a luxury brand.

---

## 2. Colors: Tonal Depth & "The No-Line Rule"
The palette centers on an electric blue (`primary`) paired with a sophisticated lavender (`secondary`). We do not use these colors merely for decoration; we use them to direct the eye through a high-energy narrative.

### The "No-Line" Rule
**Explicit Instruction:** Do not use 1px solid borders to define sections. All boundaries must be achieved through:
*   **Background Shifts:** Transitioning from `surface` to `surface-container-low`.
*   **Tonal Transitions:** Utilizing `surface-container-highest` to anchor a content block against a `surface` background.

### Surface Hierarchy & Nesting
Treat the UI as a series of physical layers. We use the surface-container tiers to define importance:
*   **Hero/Base:** `surface` (#f6f6f9)
*   **Primary Content Containers:** `surface-container-lowest` (#ffffff) to provide "pop."
*   **Secondary Context:** `surface-container-high` (#e1e2e6) to recede.

### The "Glass & Gradient" Rule
To elevate the system from "flat" to "premium," floating elements (modals, navigation bars) should utilize **Glassmorphism**:
*   **Token:** `surface-container-lowest` at 80% opacity.
*   **Effect:** 20px - 40px Backdrop Blur.
*   **Signature Texture:** Use a subtle linear gradient on main CTAs from `primary` (#0846ed) to `primary_container` (#859aff) at a 135-degree angle. This adds a "soul" to the color that flat hex codes cannot replicate.

---

## 3. Typography: The Power of Scale
We utilize a pairing of **Plus Jakarta Sans** for high-impact displays and **Inter** for functional readability.

*   **Display (Plus Jakarta Sans):** These are your "vibe" setters. Use `display-lg` (3.5rem) with tight letter-spacing (-0.02em) to create a bold, high-energy headline that feels like a magazine cover.
*   **Headlines (Plus Jakarta Sans):** Use `headline-lg` for section headers. Ensure they have ample `margin-bottom` to let the "Kinetic Elegance" breathe.
*   **Body & Titles (Inter):** These tokens (`body-lg`, `title-md`) are the workhorses. Inter’s neutral character balances the aggressive energy of the displays, ensuring the "premium" aspect of the brand personality is maintained.
*   **Labels (Inter):** Use `label-md` in all-caps with +0.05em tracking for overlines to signal high-end categorization.

---

## 4. Elevation & Depth: Tonal Layering
Traditional shadows are often a crutch for poor layout. In this system, depth is earned.

*   **The Layering Principle:** Instead of a shadow, place a `surface-container-lowest` card on top of a `surface-container-low` section. The subtle delta in hex value creates a "soft lift" that feels architectural rather than digital.
*   **Ambient Shadows:** For floating CTAs or high-priority cards, use a "Double-Diffusion" shadow:
    *   **Layer 1:** 0px 4px 20px rgba(8, 70, 237, 0.04) (Tinted with `primary`)
    *   **Layer 2:** 0px 10px 40px rgba(12, 14, 16, 0.06) (Tinted with `inverse_surface`)
*   **The "Ghost Border" Fallback:** If a container sits on a background of the same color, use a `outline-variant` token at **15% opacity**. Never use 100% opaque borders.
*   **Roundedness:** Stick to `xl` (1.5rem) for main containers and `md` (0.75rem) for smaller interactive elements. This creates a friendly, modern "vibe" that offsets the sharp typography.

---

## 5. Components: Precision & Interaction

### Buttons (The Energy Drivers)
*   **Primary:** Gradient of `primary` to `primary_container`. Roundedness: `full`. Text: `label-md` (Bold).
*   **Secondary:** `secondary_container` background with `on_secondary_container` text. This soft lavender provides a sophisticated "rest" for the eyes.
*   **Tertiary:** No background. Underline using 2px `primary` at 30% opacity, shifting to 100% on hover.

### Cards & Lists
*   **Forbid Dividers:** Use `surface-container` shifts or `2rem` vertical spacing to separate items. 
*   **The "Floating Chip":** Use `secondary_fixed` for category chips. They should feel like soft accents against the high-energy blue.

### Input Fields
*   **Style:** `surface-container-lowest` background with a `Ghost Border` (15% `outline-variant`). 
*   **Focus State:** Transition the border to 100% `primary` and add a 4px soft outer glow using the `primary_fixed` token.

---

## 6. Do’s and Don’ts

### Do:
*   **Do** lean into white space. If you think there is enough space, add 16px more.
*   **Do** overlap elements. Let a `display-lg` headline partially hang over a `surface-container-lowest` card to create depth.
*   **Do** use the `primary` electric blue sparingly but purposefully to drive the "vibrant" energy.

### Don’t:
*   **Don’t** use black (#000000) for text. Always use `on_surface` (#2d2f31) to maintain the premium, soft-touch feel.
*   **Don’t** use "Drop Shadows" from a standard UI kit. If it looks like a default shadow, it is wrong.
*   **Don’t** use lines to separate content. If you feel the need for a line, try a background color shift first.
*   **Don't** use standard "Rounded" corners (4px). Go big (`xl`) or go home (`none`).

---

## 7. Signature Editorial Component: The "Feature Break"
When transitioning between high-energy promotional sections, use a "Feature Break":
*   A full-width `primary` section using `on_primary` typography.
*   Use a `display-lg` headline centered with 15% opacity `primary_container` decorative shapes (large, `full` roundedness circles) floating in the background. 
*   This resets the user's visual palette and reinforces the "Bold/High-Energy" brand pillar.```