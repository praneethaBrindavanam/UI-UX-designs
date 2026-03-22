# Design System Specification: High-Octane Competitive Interface

## 1. Overview & Creative North Star
The Creative North Star for this design system is **"Kinetic Precision."** 

In the world of high-stakes gaming, interfaces must feel as fast as the players themselves. This system rejects the static, boxy layouts of traditional web design in favor of a fluid, editorial approach. We move beyond the "template" look by utilizing intentional asymmetry—placing the top-ranked players in oversized, overlapping "Glass Hero" cards that break the standard container grid. By leveraging high-contrast typography scales and deep, layered surfaces, we create a sense of atmospheric depth that feels less like a spreadsheet and more like a high-end broadcast HUD.

## 2. Colors & Surface Architecture
The palette is rooted in the deep `background` (#0e0e13), providing a void-like canvas where vibrant accents provide "energy pulses."

*   **Primary Pulse:** The `primary` (#9cff93) "Neon Green" is reserved for the #1 rank and critical success actions.
*   **Secondary Velocity:** The `secondary` (#00d2fd) "Electric Blue" drives the narrative for secondary ranks and interactive navigation elements.
*   **The "No-Line" Rule:** We do not use 1px solid borders to define sections. Period. Structure is achieved through "Tonal Carving." A section of content should be distinguished from the `background` by shifting to `surface-container-low` or `surface-container-high`.
*   **Surface Hierarchy & Nesting:** Treat the UI as physical layers. 
    *   Main Page: `surface`
    *   Sub-sections: `surface-container-low`
    *   Leaderboard Rows: `surface-container`
    *   Highlighted Player: `surface-container-highest`
*   **The "Glass & Gradient" Rule:** To achieve a premium feel, top-tier leaderboard cards must use Glassmorphism. Use semi-transparent versions of `surface-variant` with a 20px backdrop-blur. For main CTAs, apply a linear gradient from `primary` to `primary-container` at a 135-degree angle to simulate light-speed motion.

## 3. Typography: The Editorial Voice
We use two distinct voices to create a hierarchy that demands attention.

*   **Display & Headlines (Space Grotesk):** This is our "Machinery" font. It is bold, technical, and wide. Use `display-lg` for the "01" rank indicator to make it feel like an architectural element rather than just a number.
*   **Title & Body (Manrope):** This is our "Human" font. It is highly legible and grounded. Use `title-lg` for player names and `body-md` for secondary stats like "K/D Ratio" or "Win Rate."
*   **The Hierarchy Strategy:** High-energy design requires drastic scale shifts. Don't be afraid to pair a `display-lg` rank number directly next to a `label-sm` timestamp. This contrast creates the "Signature Editorial" look.

## 4. Elevation & Depth
Depth in this design system is "Atmospheric," not structural.

*   **Tonal Layering:** Avoid shadows for static elements. Instead, place a `surface-container-lowest` card on a `surface-container-low` background. The subtle 2-3% value shift is enough to create "Soft Lift."
*   **Ambient Shadows:** For floating modals or "Winner Pop-ups," use a shadow with a 40px-60px blur at 8% opacity. The shadow color should be a tinted `secondary` (Electric Blue) to simulate the neon glow of the UI onto the surface below.
*   **The "Ghost Border" Fallback:** If a player’s avatar needs more definition, use the `outline-variant` token at 15% opacity. It should be felt, not seen.
*   **Glassmorphism Depth:** When nesting glass elements, increase the `surface-container` tier slightly for each inner layer to simulate thicker, more refractive glass.

## 5. Components & Primitive Styles

### Buttons
*   **Primary:** Rounded `full`. Gradient fill (`primary` to `primary_container`). Text color `on_primary_fixed`. No border.
*   **Secondary:** Rounded `md`. `surface_container_highest` background with a `secondary` "Ghost Border" at 20% opacity.
*   **Interaction:** On hover, the `surface_tint` should create a subtle outer glow (0px 0px 15px).

### Leaderboard Rows (Cards)
*   **Style:** No dividers. Use `surface_container` for the row background. 
*   **Spacing:** Use `spacing-4` (0.9rem) for vertical padding to give the data room to breathe.
*   **The "Active" State:** The current user's row should use `surface_bright` and a `secondary` left-accent bar (4px width, rounded `full`).

### Chips (Stat Tags)
*   **Style:** Use `surface_container_high` with `label-md` text. 
*   **Rounding:** Always `xl` (1.5rem) to contrast with the more angular `md` row corners.

### Gaming-Specific Components
*   **Rank Medals:** Use `tertiary` (#ac89ff) for "Elite" or "Pro" tiers to separate them from the standard blue/green color flow.
*   **Performance Trend Micro-charts:** Use `secondary` for positive trends and `error` (#ff7351) for negative, rendered as 2px thick lines with no fill.

## 6. Do's and Don'ts

### Do:
*   **Use Asymmetry:** Place the "Top 3" players in a non-linear layout (e.g., #1 in the center, larger and higher than #2 and #3).
*   **Embrace Negative Space:** Use `spacing-16` (3.5rem) between major sections to let the "High-Energy" accents pop without cluttering the view.
*   **Layer with Purpose:** Use `primary` gradients only for the absolute highest point of interest on the screen.

### Don't:
*   **No Grid-Lock:** Avoid making every column the same width. Let player names have more room than numeric stats.
*   **No High-Contrast Borders:** Never use a 100% opaque `outline` for a container. It kills the "Glass" illusion.
*   **No Pure Greys:** Ensure all neutral surfaces have a slight blue/purple tint inherited from the `surface` tokens to maintain the dark-mode atmosphere.
*   **No Default Shadows:** Never use the standard (0,0,0) black drop shadow; it looks "dirty" on a neon theme. Always tint your shadows with the accent color.