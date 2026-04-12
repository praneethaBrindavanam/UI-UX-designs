# Design System Document: The Culinary Editorial

## 1. Overview & Creative North Star
**Creative North Star: "The Orchestrated Kitchen"**

In a high-pressure kitchen environment, digital interfaces must move beyond mere utility to become a silent, sophisticated partner. This design system rejects the cluttered, "app-like" aesthetic of traditional POS systems in favor of a **High-End Editorial** experience. We treat information as if it were laid out in a premium culinary monograph: spacious, authoritative, and impeccably legible.

To break the "template" look, this system utilizes **intentional asymmetry** and **tonal depth**. By using radical whitespace and oversized typography, we ensure readability from six feet away amidst the steam and speed of a professional kitchen. We move away from boxes and lines, defining the space through "The Layering Principle"—treating the screen as a series of physical, stacked surfaces that guide the eye naturally to what matters most.

---

### 2. Colors: Tonal Architecture
Our palette is rooted in "Professional Neutrals" with high-energy accents. We avoid the "flat" look by using subtle shifts in surface temperature.

#### The "No-Line" Rule
**Prohibit 1px solid borders for sectioning.** Boundaries must be defined solely through background color shifts. For example, a `surface-container-low` section sitting on a `surface` background creates a natural edge without visual noise.

#### Surface Hierarchy & Nesting
Use the surface tiers to create "nested" depth. Each inner container should shift one step in the hierarchy to define its importance:
- **Base Layer:** `surface` (#fcf9f8)
- **Secondary Zone:** `surface-container-low` (#f6f3f2)
- **Primary Content Card:** `surface-container-lowest` (#ffffff)
- **Deep Inset/Information Well:** `surface-dim` (#dcd9d9)

#### The "Glass & Gradient" Rule
For floating elements (like active order modals or system alerts), utilize **Glassmorphism**. Apply a semi-transparent `surface` color with a `backdrop-blur` of 20px. 
To add "soul" to primary actions, use subtle gradients:
- **Action Gradient:** Linear transition from `primary` (#006538) to `primary_container` (#13804b). This creates a tactile, "pressable" depth that flat green cannot achieve.

---

### 3. Typography: The High-Contrast Voice
We utilize **Inter** for its mathematical precision and exceptional legibility at high speeds. 

- **Display (Display-LG/MD):** Used for order numbers or critical timers. These are massive, bold, and authoritative. They demand attention in a busy room.
- **Headlines (Headline-LG/MD):** For dish names or section headers. Use high-contrast weights (Bold/Extra Bold) against the light surfaces.
- **Body (Body-LG/MD):** Reserved for modifications (e.g., "NO ONIONS"). These must be crisp and never smaller than `1rem` to ensure they aren't missed under harsh kitchen lighting.
- **Labels (Label-MD/SM):** Used for metadata (timestamps, server names). 

**Hierarchy Strategy:** Brand identity is conveyed through extreme scale contrast. A `display-lg` order number paired with a `label-md` timestamp creates an editorial rhythm that feels premium and intentional.

---

### 4. Elevation & Depth: Tonal Layering
Traditional shadows and borders are replaced by light-logic and surface-tier stacking.

- **The Layering Principle:** Place `surface-container-lowest` cards on a `surface-container-low` background. This creates a soft, natural lift that mimics fine paper on a stone countertop.
- **Ambient Shadows:** For floating elements only. Use a 24px blur with 6% opacity. The shadow color should be a tint of `on-surface` (#1b1c1c), ensuring it feels like an ambient occlusion shadow rather than a "drop shadow."
- **The "Ghost Border" Fallback:** If accessibility requires a border, use `outline-variant` (#becabe) at **20% opacity**. 100% opaque borders are strictly forbidden as they "trap" the content.
- **Glassmorphism:** Use semi-transparent layers for non-modal overlays. This allows the movement of the kitchen flow (orders moving in the background) to bleed through, keeping the user grounded in the environment.

---

### 5. Components: Functional Elegance

#### Large-Scale Touch Targets
Every interactive element must adhere to a minimum **48dp x 48dp** touch target. In kitchen environments, precision is a luxury; our UI must be "fat-finger friendly."

#### Buttons & CTAs
- **Primary:** Rounded (`xl`: 0.75rem), using the Action Gradient. High contrast text (`on_primary`).
- **Secondary/Tertiary:** `surface-container-highest` background with `on_surface` text. No borders.
- **States:** Hover/Active states should use a 10% brightness shift, never a color change.

#### Status Badges (The "Fresh" System)
Badges use high-chroma variants to communicate status instantly:
- **New:** `secondary` (#a83900) — Sunset orange demands immediate attention.
- **In Progress:** `tertiary` (#943942) — Deep berry/red for active focus.
- **Ready:** `primary` (#006538) — Herb green signifies completion.
*Note: Forbid small text in badges. Use `label-md` and generous horizontal padding.*

#### Cards & Lists
- **The Divider Rule:** Forbid 1px dividers. Separate order items using `1.5rem` of vertical whitespace or a subtle background shift to `surface-container-low`.
- **List Items:** Use "Leading Indicators"—a thick 4px vertical bar of `primary` or `secondary` color on the left edge of a card to denote priority, rather than a full border.

#### Specialized Culinary Components
- **The "Heat Map" Timer:** A progress bar component that transitions from `primary_fixed` to `secondary` as an order approaches its goal time.
- **Modification Callouts:** High-contrast `error_container` blocks for allergy alerts, using `headline-sm` to ensure zero-error tolerance.

---

### 6. Do's and Don'ts

#### Do
- **Do** use whitespace as a functional tool. If an order is complex, give it more room; don't cram it.
- **Do** use `surface-container-lowest` (#ffffff) for the most active, "interactable" elements.
- **Do** ensure all "Close" or "Back" actions are in the bottom corners, easily reachable by a thumb while holding a tablet.

#### Don't
- **Don't** use pure black (#000000). Use `on_surface` (#1b1c1c) for a softer, more premium high-contrast feel.
- **Don't** use standard Material Design "Outlined" text fields. Use "Filled" fields with `surface-variant` backgrounds for better visibility in high-glare environments.
- **Don't** use 100% opaque borders. They create "visual cages" that break the editorial flow.
- **Don't** settle for "good enough" typography. If the hierarchy feels flat, increase the size of the Display text. Extreme scale is our friend.