# Design System Overview: The Editorial Ledger

### 1. Overview & Creative North Star
**Creative North Star: "The Human Auditor"**
Financial software often feels cold, rigid, and clinical. This design system rejects the "spreadsheet" aesthetic in favor of a **High-End Editorial** experience. We treat financial data with the same reverence a luxury magazine treats typography. By blending the authoritative precision of deep teals with the warmth of organic accents, we create an environment that feels both bank-level secure and boutique-level personal.

This system breaks the "template" look through **intentional asymmetry** and **tonal layering**. We avoid a sea of identical boxes; instead, we use high-contrast typography scales and varying surface elevations to guide the eye toward what matters most: the bottom line and the call to action.

### 2. Colors & Surface Philosophy
The palette is rooted in trust (`primary`: deep teal) and punctuated by human warmth (`tertiary`: terracotta/warm orange). 

*   **The "No-Line" Rule:** To achieve a premium feel, **1px solid borders are strictly prohibited for sectioning.** Do not use lines to separate the sidebar from the main content or to divide invoice line items. Boundaries must be defined solely through background color shifts.
*   **Surface Hierarchy & Nesting:** Treat the UI as a physical stack of papers. 
    *   **Base:** `surface` (#f6fafe) is your canvas.
    *   **Sections:** Use `surface-container-low` (#f0f4f8) for secondary panels.
    *   **Active Focus:** Use `surface-container-lowest` (#ffffff) for the "active" invoice or focal card to make it appear to lift off the page.
*   **The "Glass & Gradient" Rule:** To avoid a flat, "out-of-the-box" look:
    *   **CTAs:** Use a subtle linear gradient transitioning from `primary` (#004f56) to `primary-container` (#006972) at a 135-degree angle.
    *   **Floating Elements:** Modals and tooltips should utilize Glassmorphism—using `surface_container_lowest` at 85% opacity with a 12px backdrop blur.

### 3. Typography: Authoritative Clarity
We pair the geometric sophistication of **Manrope** for high-level data with the functional neutrality of **Inter** for utility.

*   **Display & Headlines (Manrope):** Use `display-lg` and `headline-md` for invoice totals and branding. Manrope’s modern curves make large financial figures feel like a design statement rather than a chore.
*   **Body & Titles (Inter):** All tabular data, descriptions, and line items must use Inter. `title-sm` (1rem) is the workhorse for invoice items, providing a clean, "pro" feel that ensures legibility even at small sizes.
*   **Editorial Emphasis:** Use `label-md` in all-caps with 0.05em tracking for metadata (e.g., "INVOICE DATE" or "CLIENT ID") to mimic a high-end financial report.

### 4. Elevation & Depth
Depth is the primary driver of hierarchy in this system.

*   **Tonal Layering:** Instead of a shadow, place a `surface_container_highest` element inside a `surface_container_low` parent. This "inner depth" feels more modern and sophisticated than external shadows.
*   **Ambient Shadows:** If a card must "float" (e.g., a payment modal), use a shadow with a 32px blur, 0px offset-y, and 6% opacity. The shadow color must be a tinted version of `on_surface` (#171c1f) to ensure it feels like natural light, not digital soot.
*   **The Ghost Border:** For input fields or cards that require a boundary for accessibility, use a "Ghost Border": the `outline_variant` (#bec8ca) at **20% opacity**. It should be barely felt, only perceived.

### 5. Components

#### Buttons (The Core Action)
*   **Primary:** Features the signature Teal-to-Teal-Container gradient. Corner radius: `md` (0.375rem). Labels: `title-sm` (Inter, Semibold).
*   **Secondary:** No fill. Use a `surface-container-high` background on hover. No border.
*   **Tertiary (Warm Accent):** Used exclusively for "Pay Now" or "Urgent" actions. Fill: `tertiary` (#6e3900). It acts as a visual firefly, drawing the eye immediately.

#### Input Fields (The Data Entry)
*   **Style:** Abandon the four-sided box. Use a tonal background (`surface-container-highest`) with a `none` border and a 2px `primary` bottom-stroke that appears only on focus.
*   **Typography:** User input should be `body-lg` to ensure the user feels confident in the data they are entering.

#### Invoice Cards & Lists
*   **Rule:** Forbid the use of divider lines. 
*   **Separation:** Use vertical white space (at least 24px) or alternating background tints (`surface` to `surface-container-low`) to distinguish between line items.
*   **Status Chips:** Use `full` (9999px) roundedness. "Paid" status uses `primary_fixed_dim` with `on_primary_fixed` text. "Overdue" uses `error_container` with `on_error_container` text.

#### Progress & Charts
*   Use `primary` for growth/positive data and `tertiary` for pending/outstanding funds. This maintains the "warm vs. cold" balance of the system.

### 6. Do’s and Don’ts

**Do:**
*   **Do** use asymmetrical layouts. A sidebar that doesn't reach the bottom of the screen creates a more "editorial" feel.
*   **Do** lean into white space. If a page feels crowded, increase the padding—never add a border to "fix" it.
*   **Do** use the `tertiary` color sparingly. It is a "personal touch" intended for moments of human interaction or urgent action.

**Don’t:**
*   **Don’t** use pure black (#000000) for text. Always use `on_surface` (#171c1f) to maintain the soft, premium feel.
*   **Don’t** use standard Material 1px outlines. It breaks the "Physical Layers" metaphor.
*   **Don’t** use `xl` or `full` roundedness on primary cards. Stick to `lg` (0.5rem) to maintain a professional, slightly architectural edge.