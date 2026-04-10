# Design System Specification: Editorial Trust

## 1. Overview & Creative North Star
The Creative North Star for this design system is **"The Architectural Concierge."** 

Standard scheduling apps often feel like spreadsheets—rigid, cold, and anxiety-inducing. This system rejects that "utility-first" template in favor of an editorial, high-end experience. We move beyond "Trust Blue" as a mere accent color and treat it as an anchor for a sophisticated, layered environment. By utilizing intentional asymmetry, expansive whitespace, and a "No-Line" philosophy, we create a sense of calm authority. This is not just a booking tool; it is a premium space where time feels managed and spacious.

## 2. Colors & Surface Philosophy
We utilize a sophisticated palette that moves away from the "flat" web. Depth is our primary tool for organization.

### The "No-Line" Rule
**Explicit Instruction:** Designers are prohibited from using 1px solid borders to section content. Boundaries must be defined solely through background color shifts or subtle tonal transitions.
*   **Implementation:** To separate a sidebar from a main view, use `surface-container-low` (#f2f4f6) against a `surface` (#f7f9fb) background.

### Surface Hierarchy & Nesting
Treat the UI as physical layers of fine stationery or frosted glass. Use the `surface-container` tiers to define importance:
*   **Primary Canvas:** `surface` (#f7f9fb)
*   **Sub-Sectioning:** `surface-container-low` (#f2f4f6)
*   **High-Priority Cards:** `surface-container-lowest` (#ffffff) for maximum "pop."
*   **Nested Modals/Overlays:** `surface-container-high` (#e6e8ea) to create a sense of recess.

### Signature Textures & Glassmorphism
*   **The "Glass" Rule:** For floating navigation bars or quick-action panels, use `surface-container-lowest` at 80% opacity with a `24px` backdrop blur. This ensures the app feels "light" and integrated.
*   **The Signature Gradient:** Primary actions should not be flat. Apply a subtle linear gradient from `primary-container` (#2563eb) to `primary` (#004ac6) at a 135-degree angle to give CTAs a "jewel" quality.

## 3. Typography
We use a dual-typeface system to balance editorial personality with functional clarity.

*   **Display & Headlines (Manrope):** Use Manrope for all `display` and `headline` roles. Its geometric yet warm curves provide a modern, "custom" feel that Inter lacks in large formats. Use `display-lg` for hero booking stats or welcome messages to establish an authoritative voice.
*   **Functional Text (Inter):** Use Inter for `title`, `body`, and `label` roles. Inter’s high x-height ensures that complex scheduling data (times, dates, durations) remains legible at small scales.
*   **Hierarchy Note:** Always pair a `headline-md` in Manrope with a `body-md` in Inter. The contrast between the two typefaces signals the difference between "Story/Brand" and "Data/Action."

## 4. Elevation & Depth
In this system, shadows are "felt, not seen." We achieve hierarchy through **Tonal Layering.**

*   **The Layering Principle:** To lift a card, do not reach for a shadow first. Place a `surface-container-lowest` card on a `surface-container-low` background. This creates a "soft lift" that is cleaner and more professional than a drop shadow.
*   **Ambient Shadows:** When an element must float (e.g., a date picker popover), use a shadow with a `32px` blur and `4%` opacity, using a tinted version of `on-surface` (#191c1e).
*   **The "Ghost Border" Fallback:** If a border is required for accessibility, use the `outline-variant` (#c3c6d7) at **15% opacity**. High-contrast, 100% opaque borders are strictly forbidden.

## 5. Components

### Buttons
*   **Primary:** Uses the Signature Gradient (`primary-container` to `primary`). `12px` (xl) corner radius. Typography: `title-sm` (Inter, Semibold).
*   **Secondary:** No background, no border. Use `primary` text with a subtle `surface-container-high` background on hover.
*   **Ghost:** `outline-variant` at 20% opacity.

### Cards & Scheduling Slots
*   **Rule:** Forbid divider lines. Use `16px` of vertical whitespace (`spacing-lg`) or a shift from `surface-lowest` to `surface-low` to separate appointments.
*   **Interaction:** On hover, a card should shift from `surface-container-lowest` to `surface-bright`, coupled with a subtle scale-up (1.02x).

### Input Fields
*   **Style:** Minimalist. No bottom line or full box. Use a `surface-container-low` background with an `8px` (DEFAULT) radius. 
*   **Focus State:** The background shifts to `surface-container-lowest` and a "Ghost Border" of `primary` at 30% appears.

### Signature Component: The Time-Blocker
Instead of a standard list, use an asymmetrical "Time-Blocker." The hour label uses `display-sm` (Manrope) in a light `on-surface-variant`, while the appointment card "overlaps" the grid line slightly to break the rigid structure.

## 6. Do’s and Don’ts

### Do:
*   **Do** use asymmetrical layouts. Place primary content 2/3rds wide and secondary "meta" data 1/3rd wide without using a vertical divider.
*   **Do** use `tertiary` (#943700) sparingly for "Urgent" or "New" notifications—it provides a sophisticated contrast to the Trust Blue.
*   **Do** leverage `surface-bright` for the main background of the booking flow to reduce eye strain.

### Don’t:
*   **Don’t** use pure black (#000000) for text. Use `on-surface` (#191c1e) for high contrast and `on-surface-variant` (#434655) for secondary information.
*   **Don’t** use the `full` (9999px) radius on buttons—it feels too "consumer/social." Stick to `xl` (1.5rem/24px) for a professional, pill-like feel that maintains its architectural integrity.
*   **Don’t** use standard "drop shadows." If the tonal shift isn't enough, rethink the surface nesting.