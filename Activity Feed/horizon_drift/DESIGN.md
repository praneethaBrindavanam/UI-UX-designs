# Design System Strategy: The Digital Explorer

## 1. Overview & Creative North Star
The "Creative North Star" for this design system is **The Editorial Voyager**. 

We are moving away from the "utility-first" look of standard travel apps and toward the sophisticated feel of a high-end travel monograph. The objective is to make the user feel like they are flipping through a premium physical magazine, where the photography is the hero and the interface is the elegant curator. We break the template through **intentional asymmetry**: images may bleed off-canvas, while text elements are anchored to a generous, breathable margin. This system prioritizes tonal depth over structural lines, creating a fluid, immersive journey that feels as adventurous as the destinations it showcases.

---

## 2. Colors
Our palette balances the vastness of the ocean (`primary`) with the warmth of a Mediterranean sunset (`secondary`). 

### The "No-Line" Rule
To maintain a high-end, seamless aesthetic, **1px solid borders are strictly prohibited for sectioning content.** Boundaries must be defined through background color shifts. For example, a "Suggested Itineraries" section should transition from `surface` to `surface-container-low` to create a natural visual break without the "clutter" of a divider.

### Surface Hierarchy & Nesting
Treat the UI as a physical stack of luxury papers. 
*   **Base:** `surface` (#f9f9f9)
*   **Sectioning:** `surface-container-low` (#f3f3f3) for subtle grouping.
*   **Elevated Content:** `surface-container-lowest` (#ffffff) for high-impact cards.
*   **Interactive Overlays:** Use `surface-bright` to draw the eye to active search or filter states.

### The "Glass & Gradient" Rule
To elevate the "adventurous" spirit, use Glassmorphism for floating UI elements (like a navigation bar or a "Save Trip" button). Apply `surface` with 70% opacity and a 20px backdrop-blur. 

### Signature Textures
Main CTAs and Hero sections should utilize a subtle linear gradient transitioning from `primary` (#001e40) to `primary_container` (#003366) at a 135-degree angle. This adds a "soulful" depth that prevents the interface from feeling flat or clinical.

---

## 3. Typography
The typography system is a dialogue between the classic (`notoSerif`) and the modern (`manrope`).

*   **The Hero (Display & Headline):** We use `notoSerif` for all Display and Headline levels. This conveys authority and a sense of "timelessness." Display-lg (3.5rem) should be used for destination names, creating a bold, editorial impact.
*   **The Narrative (Body & Title):** `manrope` provides a clean, highly legible contrast. Title-lg (1.375rem) is used for storytelling sub-headers, while Body-md (0.875rem) handles the descriptive copy.
*   **The Utility (Label):** `manrope` labels at 0.75rem are used for technical data (e.g., flight times, price points), kept crisp and unobtrusive.

---

## 4. Elevation & Depth
In this system, depth is organic, not artificial.

*   **The Layering Principle:** Avoid shadows where color shifts can do the work. Place a `surface-container-lowest` card atop a `surface-container-low` background to create a "soft lift."
*   **Ambient Shadows:** If a floating element requires a shadow (e.g., a "Book Now" floating action button), use a 32px blur with 6% opacity. The shadow color must be a tinted version of `on-surface` (#1a1c1c) to ensure it looks like a natural environmental shadow rather than a digital drop shadow.
*   **The "Ghost Border" Fallback:** If a container requires a boundary (e.g., in high-density data views), use `outline-variant` (#c3c6d1) at **15% opacity**. This creates a "suggestion" of a container without breaking the editorial flow.

---

## 5. Components

### Primary Buttons
*   **Style:** `primary` background with `on_primary` text. 
*   **Radius:** `md` (0.375rem) for a refined, professional edge.
*   **Interaction:** On hover, transition to the signature gradient (Primary to Primary-Container).

### Imagery Cards (The Hero Component)
*   **Rule:** Forbid the use of divider lines. 
*   **Structure:** High-resolution imagery with a `secondary` (#ac3509) accent tag in the top-right corner using `label-md`. 
*   **Elevation:** Use `surface-container-lowest` for the card base and `xl` (0.75rem) roundedness to soften the adventurous visuals.

### Selection Chips
*   **Style:** `surface-container-high` background with `on_surface` text.
*   **Selected State:** `secondary_container` (#fe6f42) background with `on_secondary_container` (#631800) text. This provides a "sunset" pop of color.

### Input Fields
*   **Style:** Minimalist. No bottom border. Use `surface-container-highest` as a subtle fill.
*   **Focus:** Transition the background to `surface_bright` with a "Ghost Border" at 20% opacity.

### Featured Destination "Pull-Quotes"
*   **Context Specific:** A special component for travel tips. Use `notoSerif` Headline-sm, center-aligned, with a `secondary_fixed` (#ffdbd0) background "highlighter" effect behind key words.

---

## 6. Do's and Don'ts

### Do
*   **DO** use white space as a structural element. If a layout feels crowded, increase the margin rather than adding a line.
*   **DO** use `secondary` (Sunset Orange) sparingly. It is a "discovery" color—use it for CTAs, notifications, or to highlight a "Must See" destination.
*   **DO** lean into asymmetry. Off-set your `display-lg` text so it overlaps an image slightly to create a layered, 3D editorial effect.

### Don't
*   **DON'T** use 100% black text. Always use `on_surface` (#1a1c1c) to maintain a soft, premium feel.
*   **DON'T** use the `full` (9999px) roundedness for anything other than small notification badges or pill-shaped tags. Large buttons and cards must remain `md` or `xl` to keep the "clean and modern" look.
*   **DON'T** use standard grey shadows. Always ensure shadows have a minute hint of the `primary` blue to keep the palette cohesive.