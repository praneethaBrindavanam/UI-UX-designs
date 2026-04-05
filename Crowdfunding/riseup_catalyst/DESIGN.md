# Design System Specification: The Architectural Bridge

## 1. Overview & Creative North Star
**The Creative North Star: "The Visionary Steward"**

This design system is built to inhabit the space between institutional gravity and communal optimism. We are moving away from the "template" look of standard crowdfunding sites. Instead of a flat grid of boxes, we are creating a **high-end editorial experience** that treats every investment opportunity like a featured story in a premium financial journal.

The system breaks the traditional "crowdfunding" mold by using **intentional asymmetry, overlapping depth, and high-contrast typography scales.** By pairing the authoritative weight of `Manrope` with the utilitarian precision of `Inter`, we signal to the user that while the mission is community-driven, the execution is professional-grade.

---

## 2. Colors & Surface Philosophy
The palette is anchored in a deep, "Midnight Navy" (`primary`) to establish immediate trust, punctuated by a "Vibrant Menthol" (`secondary`) that pulses with optimism.

### The "No-Line" Rule
**Explicit Instruction:** Designers are prohibited from using 1px solid borders for sectioning. Structural boundaries must be defined solely through background shifts. For instance, a `surface-container-low` section should sit against a `surface` background to denote a change in context. Lines are a sign of structural weakness; color shifts are a sign of intentional architecture.

### Surface Hierarchy & Nesting
Treat the UI as a series of physical layers—like stacked sheets of fine vellum.
*   **Level 0 (Base):** `surface` (#f7f9fb) – The canvas.
*   **Level 1 (Sectioning):** `surface-container-low` (#f2f4f6) – For large background blocks.
*   **Level 2 (Interaction):** `surface-container-lowest` (#ffffff) – For primary cards and elevated content.

### Signature Textures: The "Glass & Gradient" Rule
To escape the "out-of-the-box" feel:
*   **The Glass Overlay:** Use `surface-container-lowest` with a 70% opacity and a `24px` backdrop-blur for floating navigation or sticky headers. This allows the richness of the `primary` navy or the `secondary` emerald to bleed through, softening the interface.
*   **The Tonal Gradient:** For main CTAs or Hero backgrounds, use a subtle linear gradient from `primary` (#041627) to `primary-container` (#1a2b3c) at a 135-degree angle. This adds "soul" and depth that a flat hex code cannot achieve.

---

## 3. Typography: Editorial Authority
We utilize a dual-typeface system to balance "Serious Investment" with "Modern Clarity."

*   **Display & Headlines (Manrope):** Chosen for its geometric confidence. Use `display-lg` and `headline-lg` to lead the eye. These should be set with tight letter-spacing (-0.02em) to feel like a premium masthead.
*   **Body & UI (Inter):** The workhorse. Inter provides maximum legibility for financial data and campaign descriptions.
*   **The Hierarchy of Trust:** Use `label-md` in all-caps with `+0.05em` tracking for metadata (e.g., "CAMPAIGN ENDS IN 4 DAYS") to create a sense of professional urgency without shouting.

---

## 4. Elevation & Depth: Tonal Layering
Traditional drop shadows are often a crutch for poor layout. In this system, depth is achieved through **Tonal Layering.**

*   **The Layering Principle:** Place a `surface-container-lowest` card on a `surface-container-low` section. The subtle contrast creates a "natural lift" that feels architectural rather than digital.
*   **Ambient Shadows:** When a float is required (e.g., a "Donate" modal), use an ultra-diffused shadow: `0px 24px 48px rgba(25, 28, 30, 0.06)`. Notice the shadow is tinted with the `on-surface` color, not pure black, to mimic natural light.
*   **The "Ghost Border" Fallback:** If a border is essential for accessibility, use the `outline-variant` token at **15% opacity**. High-contrast borders are strictly forbidden.

---

## 5. Component Guidelines

### Buttons: The Action Drivers
*   **Primary (The "Invest" Button):** Uses `secondary` (#006b59) background with `on-secondary` text. Shape: `md` (0.75rem) roundedness. Use a subtle inner-glow (top-down) to make it feel tactile.
*   **Secondary:** `primary` background with `on-primary` text. Used for "Learn More" or secondary navigations.
*   **Tertiary:** No background, `primary` text. Used for "Cancel" or "View All" actions.

### Cards: The Investment Units
*   **Layout:** No dividers. Use `2.5rem` (40px) of vertical padding to separate header, body, and footer.
*   **Progress Bars:** A custom implementation. The track uses `surface-variant`, while the indicator uses a gradient of `secondary` to `secondary_fixed_dim`. This visualizes growth and "filling up" with energy.

### Input Fields
*   **Style:** Minimalist. Use `surface-container-highest` as a subtle background fill with a bottom-only "Ghost Border" that transitions to a full `primary` outline on focus. This keeps the form feeling light and editorial.

### Signature Component: The "Impact Score" Chip
*   A specialized chip using `tertiary_container` with `on_tertiary_container` text to highlight social impact or ESG scores. It should feel like a seal of approval, not just a tag.

---

## 6. Do's & Don'ts

### Do
*   **Do** use asymmetrical layouts (e.g., an image overlapping a text container) to create a premium, custom feel.
*   **Do** allow for "Breathing Room." If you think there's enough whitespace, add 20% more.
*   **Do** use `primary_fixed` for background washes behind dark text to create a sophisticated, low-contrast reading environment.

### Don't
*   **Don't** use 1px dividers to separate list items. Use vertical spacing and subtle background shifts.
*   **Don't** use pure black (#000000) for text. Always use `on-surface` or `on-background` to maintain the navy-charcoal depth.
*   **Don't** use the `full` roundedness (pills) for primary cards; keep them at `lg` (1rem) or `xl` (1.5rem) to maintain a "serious" architectural profile.

---

**Director's Note:** Every pixel must feel like it was placed by a curator, not a framework. If the layout feels "expected," break the grid. If it feels "noisy," remove a line and add a shadow. This is about building trust through superior craftsmanship.