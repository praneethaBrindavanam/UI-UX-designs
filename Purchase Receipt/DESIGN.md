# High-End Editorial: Digital Receipt Design System

## 1. Overview & Creative North Star: "The Bespoke Ledger"
The goal of this design system is to transform the mundane mobile receipt into a high-end editorial experience. We are moving away from the "utilitarian spreadsheet" look and toward the "Digital Ledger"—an experience that feels as much like a premium magazine spread as it does a transaction record.

**Creative North Star: The Bespoke Ledger**
This system relies on **Intentional Asymmetry** and **Tonal Depth**. By utilizing a high-contrast typographic scale (the elegance of *Newsreader* paired with the precision of *Inter*) and replacing harsh lines with soft color shifts, we create a layout that breathes. Elements should feel "placed" rather than "slotted," using generous white space to guide the eye through the transaction story.

---

## 2. Colors & Surface Logic
The palette is rooted in a "Paper & Ink" philosophy. We use a sophisticated range of neutrals to define structure, reserved for a single, commanding stroke of `primary` indigo to signify brand authority.

### The "No-Line" Rule
**Strict Mandate:** Designers are prohibited from using 1px solid borders to separate sections.
Boundaries must be defined exclusively through background shifts. For example, a itemized list sitting in `surface-container-low` should transition to a `surface-container-highest` footer to denote the total amount. This creates a seamless, modern flow.

### Surface Hierarchy & Nesting
Treat the UI as a physical stack of fine stationery:
- **Base Layer:** `surface` (#f9f9f9) — The desk.
- **Content Block:** `surface-container-lowest` (#ffffff) — The main receipt paper.
- **Nested Detail:** `surface-container` (#ebeeef) — Inset areas for shipping maps or promo codes.

### The "Glass & Gradient" Rule
To prevent the design from feeling "flat," use Glassmorphism for floating action buttons or sticky headers. Use `surface` colors at 80% opacity with a `16px` backdrop-blur. 
- **Signature Texture:** For the "Pay" button or "View Invoice" CTA, use a subtle linear gradient from `primary` (#4c56af) to `primary_dim` (#4049a2) at a 135-degree angle. This adds "soul" and weight to the action.

---

## 3. Typography: The Editorial Mix
We use typography to establish a clear narrative hierarchy. 

*   **The Voice (Serif):** `newsreader` is used for `display` and `headline` levels. It provides a formal, trustworthy, and "boutique" feel. Use `headline-sm` for vendor names to make them feel like a masthead.
*   **The Data (Sans-Serif):** `inter` is used for `title`, `body`, and `labels`. Its high x-height ensures legibility for SKU numbers, prices, and dates.

**Hierarchy Strategy:**
- **Order Total:** `display-sm` (Newsreader) — This is the hero of the screen.
- **Section Headers:** `title-sm` (Inter, All Caps, tracking +5%) — Use for "Order Details" or "Shipping Address."
- **Item Names:** `title-md` (Inter, Medium weight) — High legibility for product titles.

---

## 4. Elevation & Depth: Tonal Layering
Traditional drop shadows are too aggressive for this aesthetic. We achieve lift through "Ambient Presence."

*   **The Layering Principle:** Place a `surface-container-lowest` card on top of a `surface-container-low` background. The contrast in hex codes provides enough "edge" without visual clutter.
*   **Ambient Shadows:** If an element must float (like a "Support" FAB), use a shadow with a `24px` blur, `0px` spread, and `4%` opacity of the `on-surface` (#2d3435) color.
*   **The "Ghost Border" Fallback:** For accessibility in input fields, use `outline-variant` (#adb3b4) at **15% opacity**. It should be felt, not seen.

---

## 5. Components & Layout Styles

### The Itemized List (The Ledger)
**Forbid dividers.** Instead, use the **Spacing Scale**.
- Use `spacing-6` (1.5rem) between items.
- Use `surface-container-lowest` for the item row background and `surface-container-high` for a "Quantity" badge.
- Lead with the product image (rounded `md`: 0.75rem), followed by the `title-md` product name.

### Status Badges
Badges should not be "bubbles" but subtle highlights.
- **Paid:** `primary-container` background with `on-primary-container` text.
- **Shipped/In Transit:** `secondary-container` background with `on-secondary-container` text.
- **Shape:** Use `rounded-full` (9999px) for a soft, pebble-like feel.

### Buttons (Key Actions)
- **Primary (Download/Share):** Background `primary`, Text `on-primary`. Shape: `rounded-lg` (1rem). 
- **Secondary (Return Item):** Background `surface-container-high`, Text `on-surface`. No border.

### Input Fields (Promo Codes)
- Use `surface-container-low` as the fill. 
- Avoid a bottom line. Use a `label-md` floating above the field in `on-surface-variant`.

---

## 6. Do’s and Don’ts

### Do:
- **Use Asymmetric Margins:** Try a wider left margin (`spacing-8`) and a tighter right margin (`spacing-5`) for "Order Total" sections to create an editorial look.
- **Embrace White Space:** If a section feels crowded, double the spacing token (e.g., move from `spacing-4` to `spacing-8`).
- **Nesting Surfaces:** Use `surface-container-lowest` for the main receipt body to make it "pop" against the `background` gray.

### Don’t:
- **Don't use 100% Black:** Never use #000000. Use `on-surface` (#2d3435) for text to maintain a premium, ink-on-paper feel.
- **Don't use 1px Dividers:** If you feel the need to separate content, use a `2px` tall gap of the `background` color instead.
- **Don't Overuse the Accent:** The `primary` indigo is a spice, not the main ingredient. Reserve it for the final "Balance Paid" or the main "Track Package" button.