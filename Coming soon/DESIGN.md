# Design System Documentation: The Obsidian Edge

## 1. Overview & Creative North Star
**Creative North Star: "The Obsidian Edge"**

This design system is built to evoke the feeling of a high-end, classified technological breakthrough. It moves away from the "friendly SaaS" aesthetic toward something more evocative, mysterious, and elite. We are not just building a webpage; we are building a digital artifact.

To achieve this, the system leverages **"Digital Redaction"**—using deep blacks (`#131313`) and tonal shifts to hide and reveal information—and **"Atmospheric Luminosity,"** where light doesn't just sit on a button but glows from within the interface. We break the standard grid with intentional asymmetry, allowing large-scale typography to overlap containers, creating a sense of motion and cinematic scale.

---

## 2. Colors & Surface Logic
The palette is rooted in deep-space neutrals, punctuated by high-energy cyans.

### The Palette
*   **Surface:** `#131313` (The foundation of the abyss)
*   **Primary:** `#c3f5ff` (The core light source)
*   **Primary Container:** `#00e5ff` (Used for high-intensity glow and "active" states)
*   **Secondary:** `#a7ccda` (Muted technical details)
*   **Outline Variant:** `#3b494c` (The "Ghost Border" token)

### The "No-Line" Rule
Standard 1px borders are strictly prohibited for sectioning. They feel "cheap" and "templated." Instead:
*   **Tonal Transitions:** Define sections by moving from `surface` to `surface_container_low` (`#1c1b1b`).
*   **Optical Separation:** Use negative space (referencing our Typography scale) to let the eye distinguish between content blocks.

### Surface Hierarchy & Nesting
Treat the UI as layers of dark glass.
1.  **Base:** `surface_dim` (`#131313`)
2.  **Sectioning:** `surface_container_low` (`#1c1b1b`)
3.  **Floating Elements/Cards:** `surface_container_high` (`#2a2a2a`)
4.  **Interactive Overlays:** `surface_bright` (`#3a3939`) with a 40% opacity and 20px backdrop-blur.

### Signature Textures
Main CTAs should never be flat. Use a linear gradient: `primary` (`#c3f5ff`) to `primary_fixed_dim` (`#00daf3`) at a 135-degree angle. This creates a "metallic" sheen that mimics high-end hardware.

---

## 3. Typography
We utilize a high-contrast scale to create an editorial, futuristic feel.

*   **Display (Space Grotesk):** Use `display-lg` (3.5rem) for hero statements. Tighten the letter-spacing to `-0.04em` to create a dense, modern "tech-heavy" look.
*   **Technical Details (Space Grotesk - Label):** Even though we use Space Grotesk for headlines, use `label-md` (0.75rem) in **ALL CAPS** with a letter-spacing of `0.15em` for technical specs, dates, and metadata. This mimics a clean, mono-spaced "HUD" (Heads-Up Display) aesthetic.
*   **Body (Manrope):** Use `body-lg` (1rem) for descriptions. Manrope provides a human, legible counterpoint to the sharp, geometric Display font. Keep line heights generous (1.6) to ensure the dark theme remains breathable.

---

## 4. Elevation & Depth
In this system, depth is a function of light and tone, not physical shadows.

### The Layering Principle
To lift a "Coming Soon" card off the background:
*   Place a `surface_container_highest` (`#353534`) element onto the `surface` (`#131313`) background.
*   The contrast alone provides the "lift."

### Ambient Shadows
If an element must float (like a modal or a floating sign-up bar), use an **Ambient Glow** instead of a shadow.
*   **Shadow Color:** `surface_tint` (`#00daf3`) at 5% opacity.
*   **Blur:** 40px to 60px.
*   **Spread:** -10px.
*   This makes the component appear to be back-lit by the neon primary color.

### The "Ghost Border" Fallback
When structural containment is vital for accessibility:
*   Use `outline_variant` (`#3b494c`) at **15% opacity**. It should be felt, not seen.

---

## 5. Components

### Buttons (The "Power Cell" Variant)
*   **Primary:** No border. Background: `primary_container`. Text: `on_primary_container`. Add a subtle outer glow using the Ambient Shadow rule above.
*   **Secondary:** Background: `none`. Border: 1px Ghost Border (`outline_variant` at 20%). On hover, increase the opacity to 100%.
*   **Shape:** Use `md` (0.375rem) for a precise, "machined" look. Avoid `full` (pill) shapes as they feel too soft for this tech aesthetic.

### Input Fields (The "Terminal" Input)
*   **Background:** `surface_container_lowest` (`#0e0e0e`).
*   **Bottom Border Only:** Instead of a full box, use a 1px `outline` (`#849396`) only on the bottom. 
*   **Focus State:** The bottom border transforms into a `primary` color glow.

### Cards & Lists
*   **Rule:** **Zero Dividers.** 
*   Use `surface_container_high` for the card background. 
*   For list items within the card, use a subtle hover state shift to `surface_bright`.
*   **Asymmetry:** Try offsetting the card title by -24px horizontally to break the container's edge—this is the "Editorial" touch.

### Additional Component: The "Progress Pulse"
For the teaser page, use a thin 2px horizontal bar (using the `tertiary` color `#ffeac0`) to indicate "System Loading" or "Time Remaining." The warmth of the tertiary color against the cold cyans creates a focal point of extreme importance.

---

## 6. Do’s and Don'ts

### Do:
*   **Embrace the Void:** Leave large areas of `surface` (`#131313`) empty. It builds tension and mystery.
*   **Use Kinetic Type:** Have your headlines overlap sections. A `display-lg` headline should feel like it's too big for its container.
*   **Layer with Glass:** Use `backdrop-blur` on navigation bars to let the background neon accents "bleed" through as the user scrolls.

### Don't:
*   **Don't use Pure White:** Use `on_surface` (`#e5e2e1`) for text. Pure `#FFFFFF` is too harsh against the deep blacks and ruins the premium "Obsidian" feel.
*   **Don't use Rounded Corners `xl` or `full`:** This isn't a consumer app for kids. Stick to `sm` and `md` to maintain a sharp, professional edge.
*   **Don't use standard Drop Shadows:** If it looks like a shadow from a 2010 interface, delete it. Use tonal shifts or glows.