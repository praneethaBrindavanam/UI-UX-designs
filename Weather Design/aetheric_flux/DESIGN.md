# Design System Document: The Celestial Lens

## 1. Overview & Creative North Star
The "Creative North Star" for this design system is **The Celestial Lens**. 

Weather is not just data; it is an atmosphere that surrounds us. This design system moves away from the "utility grid" of traditional weather apps and moves toward a high-end editorial experience. We treat the screen as a window of layered, frosted glass where hyper-local data floats within an atmospheric void. 

To break the "template" look, designers must embrace **Intentional Asymmetry**. Large-scale typography (e.g., current temperature) should overlap container edges, and cards should vary in height to create a rhythmic, scanned flow rather than a rigid table. The interface doesn't just tell you the weather; it makes you *feel* the environment through tonal depth and light-refracting surfaces.

## 2. Colors
Our palette is rooted in the deep `background` (#0c0e17), but it is designed to be reactive. While the core tokens remain constant, the "visual soul" of the app shifts based on the forecast.

*   **The "No-Line" Rule:** Sectioning must never be achieved with 1px solid borders. Boundaries are defined strictly through background shifts. For example, a `surface-container-low` section sits on a `surface` background. If you need more definition, use a `surface-container-highest` element to pull a component forward.
*   **Surface Hierarchy & Nesting:** Use the tiers of surface containers to create physical layers.
    *   Base: `surface`
    *   Sectioning: `surface-container-low`
    *   Interactive Cards: `surface-container-high` or `surface-bright`
*   **The Glass & Gradient Rule:** High-end digital experiences require light play. Use `surface-variant` at 40-60% opacity with a `backdrop-blur` of 20px-40px to create glass containers. For primary actions, transition from `primary` (#b3a1ff) to `primary-container` (#a690ff) to provide a soft, velvet-like glow that flat colors cannot replicate.
*   **Dynamic Accentuation:** Use `secondary` (oranges) for sun-related data and `tertiary` (cyans) for wind and moisture to create immediate cognitive recognition of weather types.

## 3. Typography
We utilize a dual-font strategy to balance editorial authority with functional clarity.

*   **Display & Headlines (Manrope):** This is our "Editorial" voice. Manrope’s geometric but warm character should be used for large data points (Temperatures, City Names). Use `display-lg` for the current temperature, but set it with a slight negative letter-spacing (-2%) to give it a premium, "locked-in" feel.
*   **Body & Labels (Inter):** Inter provides the "Functional" voice. It is used for all technical data points, descriptions, and labels. Its high x-height ensures that even at `label-sm` (0.6875rem), the forecast remains legible under direct sunlight.
*   **Hierarchy Strategy:** Always pair a `display-md` temperature with a `label-md` uppercase descriptor (e.g., "FEELS LIKE") to create a sophisticated high-contrast scale.

## 4. Elevation & Depth
Depth in this design system is environmental, not structural. We simulate light passing through layers of atmosphere.

*   **The Layering Principle:** Instead of shadows, stack your containers. Place a `surface-container-lowest` card inside a `surface-container-low` section to create a "recessed" look. Place a `surface-bright` glass card on a `surface` background to create "lift."
*   **Ambient Shadows:** For floating elements like a search bar or a "High Alert" card, use a shadow that mimics natural light. The shadow should be 8% opacity of the `on-surface` color with a 40px blur and a 10px Y-offset. Never use pure black shadows.
*   **The "Ghost Border" Fallback:** If a layout feels too soft, you may use a "Ghost Border." This is a 1px stroke using `outline-variant` at 15% opacity. It should feel like a light catch on the edge of a piece of glass, not a box.
*   **Glassmorphism:** To achieve the "Atmospheric" feel, cards should use `surface-container-high` at 50% opacity with a heavy backdrop blur. This allows the dynamic background colors (blues, oranges, or grays) to bleed through, ensuring the UI feels integrated into the weather state.

## 5. Components

### Buttons
*   **Primary:** Uses a vertical gradient of `primary` to `primary-container`. Shape: `full` (pill). Text: `title-sm` (Inter, Semibold).
*   **Secondary:** Ghost-style. No fill, `outline-variant` border (at 20% opacity), text in `primary`.

### Cards (The Core Component)
*   **Rule:** Forbid the use of divider lines. Use vertical white space from the `xl` or `lg` roundedness scale to separate elements.
*   **Visual Style:** Use `xl` (1.5rem) corner radius. Use the Glassmorphism stack (blur + semi-transparent fill). Content within cards should use `title-sm` for headings and `display-sm` for primary data.

### Chips
*   **Action Chips:** Used for switching between "Hourly" and "Daily." Use `surface-container-highest` for the unselected state and `primary` with `on-primary` text for the active state. Shape: `md`.

### Input Fields (Search)
*   **Style:** A soft `surface-container-high` fill with no border. The placeholder text should be `on-surface-variant`. When focused, the container should transition to a slightly higher opacity of `surface-bright`.

### Atmospheric Pulse (Custom Component)
*   A specialized component for hyper-local rain alerts. Use a `tertiary` color pulse animation behind a glass card to signify live data processing.

## 6. Do's and Don'ts

### Do
*   **Do** use asymmetrical layouts where the weather icon might overlap the edge of a card.
*   **Do** use "surface-on-surface" layering to define hierarchy rather than lines.
*   **Do** ensure that the `on-surface` text maintains a 4.5:1 contrast ratio against the blurred background for accessibility.
*   **Do** use `manrope` for any numbers that need to feel "heroic."

### Don'ts
*   **Don't** use 100% opaque, high-contrast borders.
*   **Don't** use standard Material Design drop shadows (keep them diffused and tinted).
*   **Don't** use dividers or horizontal rules to separate list items; use 16px-24px of vertical breathing room instead.
*   **Don't** use generic weather icons; ensure icons are "illustrative"—using thin `outline` weights with subtle `primary` color fills.