# Design System Strategy: The Serene Pulse

## 1. Overview & Creative North Star
This design system is built upon the Creative North Star of **"The Serene Pulse."** In the context of health and reminders, notifications should never feel like "alerts" or "interruptions." Instead, they are rhythmic, gentle nudges that integrate seamlessly into the user’s life. 

We move away from the rigid, boxed-in nature of standard mobile UI. By leveraging intentional asymmetry, high-contrast editorial typography, and a "layer-first" spatial philosophy, we create a digital environment that feels premium, breathable, and authoritative. This is not a utility; it is a high-end health companion.

## 2. Colors: Tonal Depth over Structural Lines
The palette is anchored in calming teals (`primary`) and sophisticated slate-greys (`secondary`), set against a clinical yet warm background (`surface`).

### The "No-Line" Rule
To maintain a high-end editorial feel, **1px solid borders are strictly prohibited** for sectioning or containment. Boundaries must be defined through:
*   **Background Shifts:** Use `surface-container-low` elements placed on a `surface` background.
*   **Tonal Transitions:** Use `surface-container-highest` to emphasize critical notification cards without the "boxed" aesthetic of a stroke.

### Surface Hierarchy & Nesting
Treat the UI as a series of physical layers of fine paper. 
*   **Level 0 (Background):** `surface` (#f7fafc) – The canvas.
*   **Level 1 (Sections):** `surface-container-low` (#eff4f7) – Large grouped content areas.
*   **Level 2 (Cards/Prompts):** `surface-container-lowest` (#ffffff) – Individual notifications or interactive elements. This creates a "lifted" look through pure color contrast.

### The "Glass & Gradient" Rule
For floating action buttons or high-priority reminders, use a subtle gradient transitioning from `primary` (#23677a) to `primary-dim` (#105b6d). For persistent overlays, apply Glassmorphism: use `surface-container-lowest` at 80% opacity with a `20px` backdrop blur to allow health data visualizations to bleed through softly.

## 3. Typography: The Editorial Voice
This system utilizes a dual-font strategy to balance character with utility.

*   **Manrope (Display & Headlines):** This is our "Editorial Voice." Use `display-lg` and `headline-md` for daily goals or health summaries. The geometric nature of Manrope provides a modern, confident tone.
*   **Inter (Body & Labels):** This is our "Functional Voice." Use `body-md` for notification descriptions and `label-sm` for timestamps. Inter’s high x-height ensures maximum readability even in low-light environments (e.g., late-night medication reminders).

**Hierarchy Principle:** Always pair a `headline-sm` title with a `body-sm` description to create a dramatic, intentional contrast in scale, moving away from "standard" mid-sized text blocks.

## 4. Elevation & Depth
We reject the heavy, muddy shadows of generic UI. Depth in this design system is achieved through **Tonal Layering**.

*   **The Layering Principle:** Place a `surface-container-lowest` card on top of a `surface-container` background to create natural separation.
*   **Ambient Shadows:** When a notification must "float" (e.g., a modal or top-level snackbar), use a shadow with a 24px blur, 0px offset, and 6% opacity. The shadow color must be a tinted version of `on-surface` (#2b3437) rather than pure black, ensuring the depth feels like natural ambient light.
*   **The "Ghost Border" Fallback:** If accessibility requirements demand a container edge, use a "Ghost Border." This is an `outline-variant` (#aab3b8) set to **15% opacity**. It should be felt, not seen.
*   **Roundedness:** Use the `xl` (1.5rem) scale for all primary notification cards to evoke a friendly, organic feel. Reserve `sm` (0.25rem) for minor utility elements like checkboxes.

## 5. Components

### Notification Cards
*   **Style:** No borders. Background: `surface-container-lowest`. 
*   **Layout:** Use asymmetrical internal padding (e.g., 24px top/left, 16px bottom/right) to create a custom, high-end feel. 
*   **Interaction:** On press, transition the background color to `surface-container-high`.

### Buttons
*   **Primary:** Filled with `primary`. Use `label-md` for text, converted to uppercase with 0.05em letter spacing for an authoritative look.
*   **Tertiary (Ghost):** No background or border. Use `primary` text. Ensure the hit target remains 48x48dp.

### Health Progress Chips
*   **Style:** Roundedness `full`. 
*   **Color:** `secondary-container` with `on-secondary-container` text.
*   **Usage:** For categorizing notifications (e.g., "Vitals," "Activity," "Sleep").

### Input Fields
*   **Style:** A simple underline using `outline-variant` at 40% opacity. 
*   **Focus State:** The underline transforms into a 2px weight using the `primary` color. No "box" around the input.

### Signature Component: The "Soft Pulse" Indicator
For active reminders, use a small dot (8px) of `primary` color. Apply a CSS animation that scales a `primary-container` ring from 100% to 200% size with 0% opacity to mimic a calming, rhythmic pulse.

## 6. Do's and Don'ts

### Do:
*   **Do** use `surface-container-low` to group related notifications instead of using a divider line.
*   **Do** prioritize whitespace. If a notification feels crowded, increase the `xl` corner radius and add 8px of padding.
*   **Do** use `tertiary` (#4a6084) for "informational" states that don't require immediate action.

### Don't:
*   **Don't** use 100% opaque `outline` colors for borders. It breaks the "Serene Pulse" atmosphere.
*   **Don't** use `error` (#a83836) for non-critical health alerts. Use `secondary` for missed reminders to avoid inducing user anxiety.
*   **Don't** use standard "Drop Shadows." If the element doesn't look like it's naturally lifting via color shift, use the Ambient Shadow specification.