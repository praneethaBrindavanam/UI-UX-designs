# Design System Strategy: The Stratospheric Editorial

This design system is engineered to move the airline experience away from the cluttered "utility-first" approach of legacy carriers toward a high-end, editorial-inspired digital concierge. We are replacing rigid grids and heavy borders with **The Stratospheric Editorial**—a philosophy defined by vast "sky-like" whitespace, tonal layering, and sophisticated typography that mirrors the precision of flight.

## 1. Creative North Star: The Precision Horizon
The "Precision Horizon" dictates that every interface should feel like looking out of a cockpit window at dawn: clear, layered, and deep. We break the "template" look by using **intentional asymmetry**—offsetting flight details to create a visual rhythm—and **layered surfaces** that mimic the atmospheric tiers of the sky. 

To achieve this, we avoid "flat" design. Instead, we use a sophisticated hierarchy of light and depth where the most critical information (like a Gate Number or a Boarding QR Code) sits on the "highest" visual plane.

## 2. Color & Atmosphere
The palette is rooted in the authority of deep space and the clarity of the upper atmosphere.

### The "No-Line" Rule
**Explicit Instruction:** You are prohibited from using 1px solid borders to section content. Boundaries must be defined solely through background color shifts or subtle tonal transitions.
*   **Surface Hierarchy:** Use the `surface-container` tiers to define "zones." For example, a flight itinerary should sit on `surface-container-low`, while the individual flight cards within it use `surface-container-lowest` (pure white) to create a soft, natural lift.
*   **The Glass & Gradient Rule:** For floating elements like "Check-in" prompts or "Live Flight Status" overlays, use **Glassmorphism**. Apply a `surface-container-lowest` background with 80% opacity and a `backdrop-filter: blur(20px)`.
*   **Signature Textures:** For primary actions, do not use flat navy. Use a subtle linear gradient from `primary` (#001a48) to `primary_container` (#002d72) at a 135-degree angle to give the UI a "metallic" aviation finish.

| Token | Hex | Role |
| :--- | :--- | :--- |
| `primary` | #001a48 | Brand Authority, Primary CTAs |
| `secondary` | #00658d | Action Accents, Flight Path Indicators |
| `surface` | #faf8ff | The Canvas (Atmospheric White) |
| `on_surface_variant` | #444651 | Secondary Editorial Content |

## 3. Typography: The Editorial Scale
We use a high-contrast pairing: **Manrope** for its technical, geometric precision and **Inter** for its unparalleled legibility at high altitudes/low light.

*   **Display (Manrope):** Use `display-lg` for destination codes (e.g., LHR, JFK). The large scale creates an "editorial hero" moment.
*   **Headlines (Manrope):** Used for "Status" or "Welcome" messages. Intentional tracking (letter-spacing: -0.02em) adds a premium feel.
*   **Body & Labels (Inter):** All flight data, seat numbers, and fine print. We use `label-md` for technical data to maintain a "manifest" aesthetic.

## 4. Elevation & Depth: Tonal Layering
Traditional shadows are too "web-standard." In this system, we use **Ambient Depth**.

*   **The Layering Principle:** Stack `surface-container-lowest` on top of `surface-container-high`. This creates a "sheet of paper" effect without a single line of CSS border.
*   **Ambient Shadows:** If an element must "float" (like a boarding pass card), use a shadow with a 40px blur, 0% spread, and 6% opacity of `on-surface`. This mimics natural light scattering through a cabin.
*   **The Ghost Border:** If accessibility requires a container edge, use the `outline-variant` token at **15% opacity**. It should be felt, not seen.

## 5. Components & Signature Elements

### The Modern Boarding Pass
*   **Structure:** A single, continuous surface using `surface-container-lowest`. 
*   **The "Tear-Off" Detail:** Instead of a dashed line, use a change in surface color from `surface-container-lowest` to `surface-container-low` to indicate the "stub" section.
*   **Barcodes:** Must be housed in a `surface-container-highest` rounded box (`xl` radius) with high contrast to ensure 100% scanner reliability.
*   **Seat Numbers:** Treat these as "Display" elements. Use `headline-lg` in `primary` to make the seat the most prominent item on the screen.

### Buttons & Interaction
*   **Primary Button:** `primary` gradient background, `on-primary` text, `xl` (0.75rem) roundedness. 
*   **Secondary/Ghost:** Use `secondary_fixed` background with no border. When hovered, transition to `secondary_fixed_dim`.
*   **Input Fields:** Use `surface-container-highest` with a `label-sm` floating above. No bottom line; the background fill defines the interaction area.

### Lists & Flight Results
*   **Rule:** Forbid the use of divider lines. 
*   **Implementation:** Use `spacing-8` (2rem) of vertical white space between flight cards. Inside a card, use a subtle 1px vertical "shim" using `secondary_container` to separate Departure and Arrival times—this is the only exception to the "No-Line" rule, used to represent a flight path.

## 6. Do’s and Don’ts

### Do
*   **Do** use `display-lg` for airport codes to create a "Signature Moment."
*   **Do** use asymmetrical padding (e.g., more padding on the left than the right) for editorial layouts.
*   **Do** use `surface-tint` at low opacities to "cool down" white surfaces.

### Don't
*   **Don't** use pure black (#000000). Always use `tertiary` (#171d21) for the deepest blacks.
*   **Don't** use 1px solid borders to separate "Departure" from "Arrival." Use whitespace and typography weight.
*   **Don't** use standard "drop shadows." If it looks like a default plugin setting, it is wrong.