# Design System: Midnight Gold Editorial

## 1. Overview & Creative North Star
**Creative North Star: "The Nocturnal Curator"**

This design system is engineered to evoke the tactile, sensory experience of a high-end lounge at midnight. We are moving away from the "app-like" utility of standard digital interfaces and toward a "high-end editorial" experience. The design breaks the traditional grid through **intentional asymmetry**, where high-resolution cocktail photography bleeds off-canvas, and typography scales are pushed to extremes to create a rhythmic, musical flow.

To avoid a "template" look, we utilize **layered depth**. Imagine the UI as sheets of dark smoked glass and polished brass stacked atop one another. Elements should never feel "pasted on"; they should feel emerged from the shadows.

---

## 2. Colors: The Midnight Palette
The color strategy relies on a "Midnight Gold" contrast—low-light backgrounds meeting glowing, amber-infused highlights.

### The "No-Line" Rule
**Explicit Instruction:** Designers are prohibited from using 1px solid borders for sectioning or containment. Boundaries must be defined solely through background color shifts or subtle tonal transitions. For example, a `surface-container-low` section sitting on a `surface` background provides all the definition needed.

### Surface Hierarchy & Nesting
Use the surface tiers to create physical depth without lines:
- **Base Layer:** `surface` (#0b1326) – The deep navy foundation.
- **Sunken Elements:** `surface-container-lowest` (#060e20) – For recessed areas like search bars or footer foundations.
- **Elevated Layers:** `surface-container-high` (#222a3d) – For cards that should feel closer to the user.

### The "Glass & Gradient" Rule
Standard flat colors lack the "soul" of a luxury lounge. 
- **CTAs:** Use a subtle linear gradient from `primary` (#f2ca50) to `primary-container` (#d4af37) to mimic the shimmer of liquid gold.
- **Overlays:** Use `surface-bright` (#31394d) at 60% opacity with a `20px` backdrop blur for navigation bars and floating modals.

---

## 3. Typography: Editorial Authority
We pair the authority of a classic serif with the modern precision of a sans-serif.

- **Display & Headlines (Noto Serif):** These are your "hero" moments. Use `display-lg` for signature cocktails and `headline-md` for section titles. The serif should feel expensive, spaced with a slightly tighter letter-spacing for a custom-kerned look.
- **Body & Labels (Manrope):** Use this for descriptions and utility. Manrope’s geometric clarity ensures menu items remain legible even on mobile devices in low-light environments.
- **The Contrast Gap:** Always pair a large Serif heading with a much smaller Sans-Serif label. The dramatic difference in scale is what creates the "Editorial" feel.

---

## 4. Elevation & Depth: Tonal Layering
Traditional shadows are too "digital." We achieve lift through light and translucency.

- **The Layering Principle:** Depth is achieved by "stacking." Place a `surface-container-highest` card on a `surface-container` background. The slight shift in navy tones creates a soft, natural lift.
- **Ambient Shadows:** When an element must float (e.g., a reservation modal), use a shadow with a `40px` blur and `8%` opacity. The shadow color must be a tinted version of `surface-container-lowest`, never pure black.
- **The "Ghost Border" Fallback:** If a divider is essential for accessibility, use the `outline-variant` (#4d4635) at **15% opacity**. This creates a "suggestion" of a line rather than a hard break.
- **Glassmorphism:** Apply to any element that sits over photography. Combine `surface-container` (at 70% opacity) with a heavy `backdrop-filter: blur(12px)`.

---

## 5. Components

### Buttons
- **Primary:** Gold gradient (`primary` to `primary-container`), black text (`on-primary`), `md` (0.75rem) rounded corners.
- **Secondary:** Transparent background with a "Ghost Border" (15% opacity `outline`).
- **Tertiary:** Text-only in `secondary` (#ffb875) with an arrow icon.

### Cards & Menu Items
- **Rule:** Forbid divider lines between menu items.
- **Implementation:** Use `1.5rem` (xl) vertical spacing and a subtle background shift on hover using `surface-container-high`.
- **Photography:** Containers must use `lg` (1rem) rounded corners and a subtle inner glow (1px inset shadow with 10% `primary` color) to simulate a glass frame.

### Inputs & Fields
- **Styling:** Use `surface-container-low` with a `none` border. On focus, transition the background to `surface-container-highest` and add a `primary` bottom-border (2px) only.

### Chips (Dietary Tags/Filters)
- **Selection Chips:** Use `secondary-container` (#a96000) with `on-secondary-container` text.
- **Action Chips:** Low-profile `surface-container-high` with `md` roundedness.

### Reservation Tooltips
- High-contrast: `surface-variant` background with `on-surface` text. Ensure a `12px` backdrop blur to separate the tooltip from the busy cocktail imagery behind it.

---

## 6. Do's and Don'ts

### Do:
- **Embrace Negative Space:** Allow headlines to breathe. Large margins are the hallmark of luxury.
- **Layer Elements:** Overlap a gold-accented button slightly over a photography container to break the "box" feel.
- **Use "Amber" for Interaction:** Use the `secondary` (#ffb875) and `secondary-fixed` tokens for hover states and interactive icons.

### Don't:
- **Don't use 100% white:** Use `on-surface` (#dae2fd) or `on-surface-variant` (#d0c5af) for text. Pure white (#FFFFFF) is too harsh against the Midnight backgrounds.
- **Don't use sharp corners:** This design system relies on the `DEFAULT` (0.5rem) to `xl` (1.5rem) scale to feel "velvet" and approachable.
- **Don't use standard Dividers:** If you feel the need to separate content, use a `surface-container-low` full-width block or increased whitespace.