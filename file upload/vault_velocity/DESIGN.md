# Design System Specification: The Architectural Flow

## 1. Overview & Creative North Star
**Creative North Star: "The Digital Atrium"**

This design system rejects the cluttered, industrial look of traditional file management. Instead, it adopts the philosophy of an "Architectural Atrium"—a space characterized by light, expansive volume, and structural clarity. We move beyond "standard" utility by treating file management as an editorial experience. 

To break the "template" look, we employ **Intentional Asymmetry**. Large `display-lg` headings are often offset against right-aligned utility bars, and the grid is broken by overlapping "floating" upload zones. We prioritize breathing room over information density, ensuring that every interaction feels premium, secure, and deliberate.

---

## 2. Colors & Tonal Depth
Our palette is anchored in a deep, authoritative blue and a lush, organic green, supported by a sophisticated range of architectural grays.

### The "No-Line" Rule
**Strict Mandate:** Designers are prohibited from using 1px solid borders for sectioning. Boundaries must be defined solely through background color shifts or tonal transitions. 
*   *Implementation:* Place a `surface-container-low` section directly against a `surface` background to define a sidebar or header. The human eye perceives the change in luminosity as a boundary, creating a cleaner, more high-end aesthetic.

### Surface Hierarchy & Nesting
Treat the UI as a series of stacked, semi-transparent layers. 
*   **Base:** `surface` (#f8f9fb)
*   **Low Importance:** `surface-container-low` (#f3f4f6)
*   **Interactive Containers:** `surface-container-lowest` (#ffffff) for primary content cards to create a "lifted" effect.
*   **Deep Utility:** `surface-container-highest` (#e1e2e4) for persistent navigation or footer elements.

### The "Glass & Gradient" Rule
To inject "soul" into the utility, use **Glassmorphism** for floating elements (e.g., file preview modals). Apply `surface-container-lowest` at 80% opacity with a 20px `backdrop-blur`. 
For primary CTAs (like "Start Upload"), apply a subtle linear gradient from `primary` (#003d9b) to `primary_container` (#0052cc) at a 135-degree angle. This prevents the "flat" look and adds a tactile, metallic sheen.

---

## 3. Typography: Editorial Authority
We utilize a dual-font strategy to balance character with utility. **Manrope** provides a modern, geometric voice for headers, while **Inter** ensures relentless legibility for data.

*   **Display & Headlines (Manrope):** High-contrast scales. Use `display-lg` (3.5rem) for empty states and welcome screens to create an editorial, "poster" feel.
*   **Body & Labels (Inter):** Tight tracking and generous line height. `body-md` (0.875rem) is our workhorse for file metadata.
*   **Hierarchy Note:** Use `title-lg` in `on_surface_variant` (#434654) for secondary information to create a clear visual separation from primary `headline-sm` titles.

---

## 4. Elevation & Depth
In this system, depth is a functional tool, not a stylistic flourish.

*   **Tonal Layering:** Avoid shadows for static elements. Instead, place a `surface-container-lowest` card on a `surface-container-low` background. This creates a "soft lift."
*   **Ambient Shadows:** When an element must float (e.g., a dragged file or a dropdown), use an "Extra-Diffused Ambient Shadow":
    *   `box-shadow: 0 24px 48px -12px rgba(0, 61, 155, 0.08);`
    *   The shadow is tinted with our `primary` color at very low opacity to mimic natural light refraction.
*   **The "Ghost Border" Fallback:** If a border is required for accessibility in input fields, use `outline_variant` at 20% opacity. Never use 100% opaque lines.

---

## 5. Components

### Primary Upload Zone (Drag & Drop)
The centerpiece of the experience. 
*   **Style:** A large `surface-container-low` area with a `xl` (1.5rem) corner radius. 
*   **Interaction:** On hover, the background transitions to `primary_fixed` with a "Ghost Border" of `primary`. Use a subtle micro-interaction where the icon "bounces" slightly to invite the drop.

### Buttons
*   **Primary:** Gradient fill (`primary` to `primary_container`), `full` roundedness, and `title-sm` typography. 
*   **Tertiary:** No background or border. Use `primary` text. On hover, apply a `primary_fixed` background at 50% opacity.

### Progress Bars
*   **Track:** `surface-container-highest`.
*   **Indicator:** A gradient of `tertiary` (#004e32) to `tertiary_fixed_dim` (#65dca4). 
*   **Animation:** A "shimmer" effect moving across the indicator to signal active processing.

### Input Fields
*   **Style:** `surface-container-lowest` background with a `md` (0.75rem) radius.
*   **States:** On focus, the container shouldn't just change border color; it should subtly scale by 1.01% while the `primary` "Ghost Border" fades in.

### Cards & Lists
*   **Rule:** Forbid divider lines. Use 24px of vertical whitespace (`Spacing Scale`) to separate file rows. 
*   **Selection:** Instead of a checkbox, use a background shift to `secondary_fixed` (#dae2ff) for selected rows.

---

## 6. Do’s and Don’ts

### Do
*   **DO** use whitespace as a structural element. If a layout feels crowded, increase the padding rather than adding a line.
*   **DO** use `tertiary` (#004e32) for all "Success" and "Secure" states. It feels more "Atmospheric" and professional than a standard neon green.
*   **DO** ensure all interactive elements have a minimum 44px hit zone, even if the visual asset is smaller.

### Don’t
*   **DON'T** use pure black (#000000) for text. Always use `on_surface` (#191c1e) to maintain the soft, premium feel.
*   **DON'T** use "Standard" easing. Use `cubic-bezier(0.34, 1.56, 0.64, 1)` for a playful, "springy" feel that makes the system feel responsive and alive.
*   **DON'T** ever use a 1px border to separate the sidebar from the main content. Use a background color shift.