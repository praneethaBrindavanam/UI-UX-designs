# Design System Strategy: The Kinetic Horizon

## 1. Overview & Creative North Star
The Creative North Star for this design system is **"The Kinetic Horizon."** 

In the high-stakes environment of automotive design, interfaces must transcend "digital dashboards" and become seamless extensions of the vehicle’s soul. This system rejects the static, boxy layouts of traditional web design in favor of a fluid, high-velocity aesthetic. We achieve this through **Intentional Asymmetry**—placing data-heavy visualizations off-center to mimic the driver’s peripheral focus—and **Tonal Depth**, where the UI feels like a single, machined block of obsidian rather than a collection of separate components. By utilizing overlapping glass surfaces and sharp neon accents, we create a sense of forward motion even when the vehicle is stationary.

## 2. Colors: Obsidian & Electric Pulse
The color palette is rooted in an ultra-dark spectrum to preserve night vision and provide a premium "cockpit" feel.

- **The Primary Axis (`#81ecff`):** This is your pulse. Use the `primary` and `primary_container` tokens exclusively for active data, critical alerts, and primary interactions.
- **Surface Hierarchy & Nesting:** Avoid a flat UI by stacking layers. 
    - Base Layer: `surface` (`#0b0e11`).
    - Sectional Lifts: Use `surface_container_low` for large background areas.
    - Component Lifts: Use `surface_container_high` or `highest` for interactive cards.
- **The "No-Line" Rule:** 1px solid borders are strictly prohibited for sectioning. Define boundaries through shifts in surface tokens. For example, a `surface_container_low` widget should sit directly on a `surface` background. The change in hex value is the boundary.
- **The "Glass & Gradient" Rule:** To achieve a "high-tech" look, use semi-transparent `surface_bright` with a `backdrop-filter: blur(20px)`. Main CTAs should utilize a subtle linear gradient from `primary` (`#81ecff`) to `primary_dim` (`#00d4ec`) at a 135-degree angle to provide a sense of metallic sheen.

## 3. Typography: Precision Engineering
Typography must feel machined and purposeful. We use a dual-font approach to balance futuristic character with extreme legibility.

- **Display & Headlines (`Space Grotesk`):** This is our "Machined" face. The slight quirks in Space Grotesk provide the futuristic tone. Use `display-lg` for speedometers or critical hero metrics.
- **Title & Body (`Manrope`):** This is our "Functional" face. Manrope’s geometric clarity ensures that even at high speeds or in low-light conditions, data remains legible.
- **Editorial Contrast:** Create impact by pairing a `display-sm` value in `primary` color with a `label-sm` value in `on_surface_variant`. The extreme scale shift (2.25rem vs 0.6875rem) removes the "template" feel and creates an authoritative hierarchy.

## 4. Elevation & Depth
Depth in this system is not about "shadows"—it is about **Refraction and Light.**

- **The Layering Principle:** Use the "Ambient Lift" method. If a module needs to feel closer to the driver, move it from `surface_container` up to `surface_bright`. 
- **Ambient Shadows:** Standard drop shadows are too "web-like." If a floating element (like a modal or pop-over) requires a shadow, use a 40px blur at 8% opacity using the `primary` color. This creates a "glow" rather than a shadow, suggesting the screen is emitting light onto the dashboard.
- **The "Ghost Border" Fallback:** For input fields or areas requiring strict containment, use a 1px border with `outline_variant` at **15% opacity**. It should be felt, not seen.
- **Glassmorphism:** All floating cards must use `surface_container_high` at 60% opacity with a `20px` backdrop blur. This allows the background map or data visualizations to bleed through, maintaining the "integrated" automotive feel.

## 5. Components

### Buttons & Interaction
- **Primary Action:** Rounded (`9999px`), using the Primary-to-Primary-Dim gradient. No border. Text is `on_primary_fixed` for maximum contrast.
- **Secondary Action:** Transparent background with a "Ghost Border" and `primary` text.
- **Active States:** When a button is pressed, use a subtle outer glow (0px 0px 12px) using the `primary` token.

### Data Visualization (The Pulse)
- **Gauges:** Use `primary` for current values and `outline_variant` for the "empty" track.
- **Trends:** Use `tertiary` (`#70aaff`) for secondary data streams to provide a sophisticated, multi-tonal blue aesthetic without clashing with the primary action color.

### Cards & Lists
- **No Dividers:** Lists must never use horizontal lines. Use `1.5rem` (xl) vertical spacing to separate items, or alternate background colors between `surface_container_low` and `surface_container`.
- **Rounding:** Use the `lg` (1rem) token for standard cards. Use `xl` (1.5rem) for main dashboard modules to emphasize the "integrated" feel.

### Input Fields
- **States:** Inactive fields should be `surface_container_highest` with no border. Upon focus, the field should transition to a 1px "Ghost Border" of `primary` and a subtle inner glow.

## 6. Do’s and Don’ts

### Do:
- **Do** use `primary` sparingly. It is a "signal" color. If everything is neon, nothing is important.
- **Do** lean into asymmetry. A map that takes up 65% of the screen with data controls tucked into the remaining 35% feels more custom than a 50/50 split.
- **Do** use `spaceGrotesk` for all numerical data to give it a technical, high-end feel.

### Don’t:
- **Don’t** use pure white (`#FFFFFF`). Use `secondary` (`#e2e2e5`) or `on_surface` (`#f8f9fe`) to prevent eye strain in dark car interiors.
- **Don’t** use hard 90-degree corners. The automotive world is fluid; every edge should have at least a `sm` (0.25rem) radius.
- **Don’t** use standard "Material Design" shadows. They look "dirty" on deep black backgrounds. Use light-based glows instead.