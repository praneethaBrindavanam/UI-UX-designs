# Design System Strategy: Editorial Precision

## 1. Overview & Creative North Star
**Creative North Star: "The Luminescent Authority"**

This design system moves beyond the standard "SaaS template" by blending the rigid authority of high-end editorial layouts with a fluid, digital-first vibrancy. We reject the "boxed-in" web; instead, we treat the subscription page as a singular, cohesive canvas where importance is defined by scale, light, and depth rather than lines and borders. 

By utilizing intentional asymmetry—such as offset headline placements and overlapping surface layers—we create a sense of forward motion. This system is designed to evoke a "Premium Digital Service" through high-contrast typography and a sophisticated use of luminescence, where colors don't just sit on the page—they glow from within.

---

## 2. Colors & The "No-Line" Rule
The color palette is anchored in a deep, midnight foundation (`surface: #0a082f`) contrasted against hyper-modern accents (`secondary: #00f4fe` and `tertiary: #ff7350`).

### The "No-Line" Rule
**Strict Mandate:** Designers are prohibited from using 1px solid borders for sectioning or containment. 
*   **Definition through Shift:** Separate the Hero from the Pricing Grid using a background shift from `surface` to `surface-container-low`.
*   **The Signature Glow:** Use `surface-bright` (#26245f) as a subtle radial gradient behind primary value propositions to create a "halo" effect, guiding the eye without structural clutter.

### Surface Hierarchy & Nesting
Treat the UI as physical layers. 
1.  **Base:** `surface` (#0a082f)
2.  **Sectioning:** `surface-container-low` (#0e0d38)
3.  **Interactive Elements (Cards):** `surface-container` (#141341)
4.  **Floating Modals/Popovers:** `surface-container-highest` (#201e55)

### The "Glass & Gradient" Rule
To achieve a "High-Impact" feel, primary CTAs should not be flat. Use a linear gradient from `primary` (#97a9ff) to `primary-dim` (#3e65ff) at a 135-degree angle. For floating navigation or secondary pricing tiers, use Glassmorphism: `surface-container-high` at 60% opacity with a `20px` backdrop-blur.

---

## 3. Typography
We use a dual-font strategy to balance "Modern" with "Trust."

*   **Display & Headlines (Manrope):** This geometric sans-serif provides the "Impact." Use `display-lg` for subscription totals or hero hooks. The tight tracking and bold weights convey authority.
*   **Body & Labels (Inter):** The "Clarity" engine. Inter’s tall x-height ensures readability even at `body-sm`. Use `on-surface-variant` (#a8a7d5) for secondary body text to maintain a sophisticated hierarchy.

**Editorial Tip:** Use `headline-lg` for pricing tier names, but set them in all-caps with `0.1rem` letter spacing to create a premium, "magazine-header" feel.

---

## 4. Elevation & Depth
Depth is a psychological tool for trust. If an element feels "grounded," it feels secure.

*   **The Layering Principle:** Instead of shadows, nest a `surface-container-lowest` card inside a `surface-container-high` wrapper. This "inverted depth" creates a sleek, recessed look that feels integrated into the interface.
*   **Ambient Shadows:** If a pricing card must "float" to indicate a "Recommended" status, use a shadow color derived from `on-surface` at 6% opacity with a `48px` blur and `12px` Y-offset. It should feel like a soft glow, not a hard drop-shadow.
*   **The "Ghost Border":** For accessibility on inputs, use `outline-variant` (#45446c) at **15% opacity**. It provides a "hint" of a container without breaking the "No-Line" rule.

---

## 5. Components

### Buttons
*   **Primary:** Gradient of `primary` to `primary-dim`. Text: `on-primary`. Shape: `xl` (0.75rem). Use `16` (5.5rem) horizontal padding for a wide, cinematic stance.
*   **Tertiary:** No background. Text: `secondary` (#00f4fe). Use `label-md` in all-caps.

### Subscription Cards
*   **Layout:** Forbid dividers. Use `spacing-8` (2.75rem) to separate the price from the feature list.
*   **Featured State:** Scale the card by 1.05x and apply a `2px` "inner glow" using a semi-transparent `secondary` color.

### Input Fields
*   **Styling:** Use `surface-container-highest` backgrounds. 
*   **Focus State:** Transition the background to `surface-bright` and change the label color to `secondary`. No heavy focus rings; use a subtle `secondary` under-glow (2px bottom border only).

### Progress Indicators (Step-based Checkout)
*   **Visuals:** Use the `tertiary` (#ff7350) color for active steps. It provides a "vibrant" high-contrast signal against the deep blue background, ensuring the user never feels lost.

---

## 6. Do's and Don'ts

### Do:
*   **DO** use whitespace as a separator. Use `spacing-20` (7rem) between major sections to let the typography "breathe."
*   **DO** use `secondary` (#00f4fe) for small, high-impact functional elements like checkmarks in a feature list.
*   **DO** align text-heavy sections to a 12-column grid but allow imagery or "background glass" elements to break the grid and bleed to the edge of the viewport.

### Don't:
*   **DON'T** use pure black (#000000) for backgrounds. It kills the "luminescent" quality of the `surface` tokens.
*   **DON'T** use `error` (#ff6e84) for anything other than critical destructive actions. For "High-Impact" alerts, use `tertiary`.
*   **DON'T** stack more than three levels of surface nesting. If you need more depth, use a backdrop-blur instead of a fourth color shift.