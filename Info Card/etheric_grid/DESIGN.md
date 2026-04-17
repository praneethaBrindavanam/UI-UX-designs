```markdown
# Design System Document: The Editorial Information Architecture

## 1. Overview & Creative North Star: "The Modern Curator"
This design system moves beyond the generic "SaaS dashboard" aesthetic to embrace an **Editorial Minimalism** philosophy. Our Creative North Star is **"The Modern Curator"**—a system that treats information not as data points, but as curated content. 

To achieve a high-end, bespoke feel, we break the "template" look by using **intentional white space, tonal layering, and sophisticated typography scales.** Instead of rigid grids separated by lines, we use depth and atmospheric shifts to guide the eye. The experience should feel like a premium digital magazine: crisp, airy, and authoritative.

---

## 2. Colors & Atmospheric Tones
We utilize a neutral foundation punctuated by "Atmospheric Accents" to denote industry context (e.g., Blue for Real Estate, Purple/Green for Gaming) without overwhelming the content.

### The "No-Line" Rule
**Explicit Instruction:** Designers are prohibited from using 1px solid borders to section content. Boundaries must be defined through background color shifts. Use `surface-container-low` (#f0f4f7) sections sitting on a `surface` (#f7f9fb) background to create containment.

### Surface Hierarchy & Nesting
Treat the UI as a series of physical layers. Use the hierarchy below to define importance:
- **Base Layer:** `surface` (#f7f9fb)
- **Sectioning Layer:** `surface-container-low` (#f0f4f7)
- **Primary Content Cards:** `surface-container-lowest` (#ffffff)
- **Elevated Interstitials:** `surface-bright` (#f7f9fb)

### The Glass & Gradient Rule
To move beyond a flat feel, use **Glassmorphism** for floating overlays. Apply `surface-container-lowest` at 80% opacity with a `backdrop-blur` of 12px. For primary CTAs, do not use flat colors; use a subtle linear gradient from `primary` (#005ac2) to `primary-dim` (#004fab) at a 135-degree angle to provide "visual soul."

---

## 3. Typography: The Editorial Voice
Our typography pairing balances the structural precision of **Inter** with the character-rich geometry of **Manrope**.

*   **Display & Headlines (Manrope):** These are your "Editorial Anchors." Use `display-lg` (3.5rem) for hero moments and `headline-sm` (1.5rem) for card titles. The wider apertures of Manrope convey modernity and openness.
*   **Body & Labels (Inter):** Inter provides "Information Integrity." Use `body-md` (0.875rem) for general card descriptions to maintain high legibility even at smaller scales.
*   **Hierarchy as Identity:** Always maintain at least a 2-step jump in the type scale between titles and body text to ensure a high-contrast, premium look.

---

## 4. Elevation & Depth: Tonal Layering
We reject the heavy drop-shadows of the early web. Depth in this system is achieved through light and atmospheric layering.

*   **The Layering Principle:** Instead of a shadow, place a `surface-container-lowest` card (Pure White) on a `surface-container-low` background. The contrast in hex values creates a "soft lift" that feels architectural.
*   **Ambient Shadows:** For floating elements (like hover states), use a multi-layered shadow: `0px 10px 30px rgba(42, 52, 57, 0.06)`. Note the use of `on-surface` (#2a3439) as the shadow tint rather than pure black—this mimics natural light.
*   **The "Ghost Border" Fallback:** If accessibility requires a container boundary, use a "Ghost Border": `outline-variant` (#a9b4b9) at **15% opacity**.
*   **Glassmorphism:** For top-level navigation or modal cards, use semi-transparent `surface` colors with a blur. This allows the "Atmospheric Accents" (like the Real Estate blue) to bleed through the UI, integrating the content with the brand.

---

## 5. Components

### Information Cards (Primary Component)
*   **Structure:** No borders. Use `md` (0.75rem) or `lg` (1rem) corner radius.
*   **Contextual Accents:** For Real Estate, use a 4px left-accent bar of `primary` (#005ac2). For Gaming, use `secondary` (#6e3bd8).
*   **Content:** Forbid divider lines. Use 24px of vertical padding (`spacing-6`) to separate the title from the body.

### Buttons
*   **Primary:** Linear gradient (`primary` to `primary-dim`), `full` (pill) radius, `on-primary` text.
*   **Secondary:** `surface-container-high` background with `primary` text. No border.
*   **States:** On hover, increase the shadow diffusion; do not simply darken the color.

### Chips & Tags
*   **Action Chips:** Use `secondary-container` (#e9ddff) for Gaming-related tags to create a vibrant, high-energy feel.
*   **Information Chips:** Use `tertiary-container` (#69f6b8) for "New" or "Live" status indicators in Real Estate.

### Input Fields
*   **Soft Focus:** Background should be `surface-container-highest` (#d9e4ea). On focus, transition the background to `surface-container-lowest` (#ffffff) and apply a Ghost Border of `primary`.

### Navigation Rails
*   Instead of a sidebar with a line, use a subtle background shift to `surface-dim` (#cfdce3) to define the navigation area.

---

## 6. Do’s and Don’ts

### Do
*   **Do** use asymmetrical margins (e.g., more padding on the top than the bottom of a card) to create an editorial feel.
*   **Do** use `surface-container` tiers to nest content (e.g., a "Search" bar inside a "Header" section).
*   **Do** prioritize typography scale over color to show hierarchy.

### Don’t
*   **Don’t** use a 1px solid border, ever. It breaks the "Modern Curator" illusion.
*   **Don’t** use high-contrast drop shadows. If it looks like a "shadow," it’s too dark.
*   **Don’t** use pure black (#000000) for text. Always use `on-surface` (#2a3439) to maintain a soft, premium appearance.
*   **Don’t** crowd the cards. If in doubt, add 8px more padding. Space is a luxury.