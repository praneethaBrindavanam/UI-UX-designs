```markdown
# Design System Strategy: Kinetic Vitality

## 1. Overview & Creative North Star
**Creative North Star: "The High-Velocity Editorial"**

This design system is built to destroy the "standard fitness app" aesthetic. We are moving away from generic grids and flat boxes toward a high-end editorial experience that feels like a premium motion-graphics piece frozen in time. The objective is to capture the raw energy of a workout—the sweat, the movement, and the focus—through **intentional asymmetry**, **aggressive typography scales**, and **kinetic layering**. 

By overlapping elements (e.g., a "Display" heading bleeding over a "Primary" card) and utilizing a high-contrast palette, we create a sense of forward momentum. We don't just display data; we give it an athletic pulse.

---

## 2. Colors & Atmospheric Depth
Our palette is a high-octane dialogue between the void (`background: #0e0e0e`) and the spark (`primary: #f3ffca`). 

### The "No-Line" Rule
To maintain a premium, seamless feel, **1px solid borders are strictly prohibited for sectioning.** 
*   **Separation through Tonal Shifts:** Define boundaries by placing a `surface-container-low` section against the `surface` background. 
*   **Depth through Nesting:** Use the surface-container tiers (Lowest to Highest) to create a physical sense of stacking. A workout card (`surface-container-highest`) should sit atop a category tray (`surface-container-low`), creating natural hierarchy without visual clutter.

### Glass & Signature Textures
*   **Kinetic Glass:** For floating navigation or modal overlays, use semi-transparent `surface-variant` with a 24px backdrop blur. This allows the vibrant "Electric Lime" of the content to bleed through, softening the interface.
*   **Soulful Gradients:** For high-impact CTAs, do not use flat fills. Transition from `primary` (#f3ffca) to `primary-container` (#cafd00) at a 135-degree angle to simulate the sheen of high-performance athletic gear.

---

## 3. Typography
The typography is the engine of this system. We use two sans-serif powerhouses: **Lexend** for rhythmic impact and **Manrope** for technical clarity.

*   **Display (Lexend):** Massive, bold, and unapologetic. Use `display-lg` (3.5rem) for hero stats and motivational headlines. The tight tracking conveys urgency.
*   **Headlines & Labels (Lexend):** These are the "call-outs." Use `headline-sm` for card titles to maintain the brand’s aggressive personality.
*   **Body & Titles (Manrope):** This is your functional workhorse. `body-lg` provides a sophisticated, readable contrast to the heavy headers, ensuring that complex workout instructions remain accessible.

---

## 4. Elevation & Depth
In a "Kinetic" system, depth is not about shadows; it’s about **Tonal Layering.**

*   **The Layering Principle:** Stack `surface-container-lowest` cards on `surface-container-low` backgrounds. This "recessed" look feels more integrated into the "Deep Charcoal" environment than a floating shadow.
*   **Ambient Shadows:** If an element must float (e.g., a FAB), use a shadow tinted with `surface-tint`. Settings: `Blur: 40px, Opacity: 6%, Offset-Y: 12px`. It should feel like a soft glow, not a dark smudge.
*   **The "Ghost Border" Fallback:** If accessibility requires a stroke, use `outline-variant` at **15% opacity**. It should be felt, not seen.
*   **Glassmorphism:** Use for "Quick Action" menus. The background blur creates a "frosted lens" effect that keeps the focus on the movement happening behind the UI.

---

## 5. Components

### Buttons (The High-Contrast Engine)
*   **Primary:** Solid `primary-container` (#cafd00) with `on-primary-container` (#4a5e00) text. Shape: `xl` (3rem) roundedness. 
*   **Secondary:** Glassmorphic fill (`surface-variant` at 40% opacity) with a `primary` ghost border. 
*   **Tertiary:** No background. Bold `lexend` uppercase text with a playful icon.

### Cards & Progress
*   **Forbid Dividers:** Never use a line to separate "Sets" or "Reps." Use 24px of vertical whitespace or a shift from `surface-container-high` to `surface-container-lowest`.
*   **Progress Rings:** Use `primary` for active progress and `surface-container-highest` for the track. The high contrast against the `#0e0e0e` background makes the data pop like a neon sign.

### Input Fields
*   **State:** Default inputs use `surface-container-low`. On focus, the container shifts to `surface-container-highest` with a 2px `primary_dim` glow. No harsh boxes—use `md` (1.5rem) corners.

### Playful Interaction Components
*   **Achievement Chips:** Use `secondary_container` with `primary` icons. These should feel like physical "badges" collected during a session.

---

## 6. Do’s and Don’ts

### Do
*   **Do Use Overlapping Elements:** Let a high-resolution athlete image bleed under the `display-lg` typography.
*   **Do Embrace Whitespace:** Fitness is about breathing. Give your elements room to move.
*   **Do Use "Electric Lime" Sparingly:** It is a highlighter, not a background. Use it to pull the eye to the most critical action.

### Don’t
*   **Don’t Use Pure Black:** Always use our `background` (#0e0e0e) to maintain a soft, premium "Charcoal" depth.
*   **Don’t Use Sharp Corners:** Anything under 16px feels "corporate" and "stiff." Keep it `md` to `xl` to stay friendly and accessible.
*   **Don’t Use Default System Icons:** Use heavy-weight, rounded icons that match the `lexend` stroke width to maintain visual harmony.

---
*Director's Final Note: Every screen should feel like it's in motion. If a layout feels static, break the grid. Lean into the asymmetry of the human body.*```