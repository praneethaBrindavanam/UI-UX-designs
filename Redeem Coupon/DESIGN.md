---
name: Kinetic Clarity
colors:
  surface: '#faf8ff'
  surface-dim: '#d2d9f4'
  surface-bright: '#faf8ff'
  surface-container-lowest: '#ffffff'
  surface-container-low: '#f2f3ff'
  surface-container: '#eaedff'
  surface-container-high: '#e2e7ff'
  surface-container-highest: '#dae2fd'
  on-surface: '#131b2e'
  on-surface-variant: '#424656'
  inverse-surface: '#283044'
  inverse-on-surface: '#eef0ff'
  outline: '#727687'
  outline-variant: '#c2c6d8'
  surface-tint: '#0054d6'
  primary: '#0050cb'
  on-primary: '#ffffff'
  primary-container: '#0066ff'
  on-primary-container: '#f8f7ff'
  inverse-primary: '#b3c5ff'
  secondary: '#006c49'
  on-secondary: '#ffffff'
  secondary-container: '#6cf8bb'
  on-secondary-container: '#00714d'
  tertiary: '#a33200'
  on-tertiary: '#ffffff'
  tertiary-container: '#cc4204'
  on-tertiary-container: '#fff6f4'
  error: '#ba1a1a'
  on-error: '#ffffff'
  error-container: '#ffdad6'
  on-error-container: '#93000a'
  primary-fixed: '#dae1ff'
  primary-fixed-dim: '#b3c5ff'
  on-primary-fixed: '#001849'
  on-primary-fixed-variant: '#003fa4'
  secondary-fixed: '#6ffbbe'
  secondary-fixed-dim: '#4edea3'
  on-secondary-fixed: '#002113'
  on-secondary-fixed-variant: '#005236'
  tertiary-fixed: '#ffdbd0'
  tertiary-fixed-dim: '#ffb59d'
  on-tertiary-fixed: '#390c00'
  on-tertiary-fixed-variant: '#832600'
  background: '#faf8ff'
  on-background: '#131b2e'
  surface-variant: '#dae2fd'
typography:
  display-lg:
    fontFamily: manrope
    fontSize: 32px
    fontWeight: '700'
    lineHeight: 40px
    letterSpacing: -0.02em
  headline-md:
    fontFamily: manrope
    fontSize: 24px
    fontWeight: '600'
    lineHeight: 32px
    letterSpacing: -0.01em
  body-lg:
    fontFamily: inter
    fontSize: 18px
    fontWeight: '400'
    lineHeight: 28px
  body-md:
    fontFamily: inter
    fontSize: 16px
    fontWeight: '400'
    lineHeight: 24px
  label-caps:
    fontFamily: inter
    fontSize: 12px
    fontWeight: '600'
    lineHeight: 16px
    letterSpacing: 0.05em
  numeric-md:
    fontFamily: manrope
    fontSize: 16px
    fontWeight: '600'
    lineHeight: 24px
rounded:
  sm: 0.25rem
  DEFAULT: 0.5rem
  md: 0.75rem
  lg: 1rem
  xl: 1.5rem
  full: 9999px
spacing:
  unit: 8px
  container-max: 1120px
  gutter: 24px
  margin-mobile: 16px
  section-gap: 48px
---

## Brand & Style

The design system is engineered to transform the high-friction moment of checkout into a seamless, reassuring transition. The brand personality is grounded yet forward-leaning—balancing the institutional reliability of a bank with the modern efficiency of a premium digital service. 

The aesthetic follows a **Corporate / Modern** direction with a focus on high-clarity minimalism. It utilizes generous whitespace to isolate tasks, preventing the "information overload" typically associated with financial transactions. The emotional response should be one of confidence, security, and momentum.

## Colors

The palette is anchored by a vibrant **Electric Blue** (#0066FF) primary color, selected specifically for its high-action "Proceed" energy. A **Success Green** (#10B981) is utilized for confirmation states and security indicators to reinforce trust.

The neutral scale favors a deep **Slate** (#0F172A) for high-readability typography, set against a very soft **Ice Blue** (#F8FAFC) background. This subtle tinting reduces the harshness of pure white while maintaining a clean, medical-grade level of professionalism.

## Typography

This design system employs a dual-font strategy. **Manrope** is used for headlines and financial figures; its refined, modern geometric structure conveys stability and makes currency values feel premium. **Inter** is used for body copy and UI labels due to its exceptional legibility and systematic, utilitarian nature.

Special attention is paid to financial details. All price-related data must use **tabular-nums** (tnum) OpenType features to ensure that columns of numbers align vertically for easy comparison during the checkout summary.

## Layout & Spacing

The layout utilizes a **Fixed Grid** model for the desktop checkout experience to maintain a focused, narrow reading path that minimizes eye travel. The main content area is capped at 1120px, typically divided into a 2/3 column for form entry and a 1/3 sidebar for the order summary.

A strict 8px spatial system governs all margins and padding. Large "Section Gaps" (48px) are used to clearly separate logical steps (e.g., Shipping vs. Payment) to reduce the perceived complexity of the form.

## Elevation & Depth

Visual hierarchy is established through **Tonal Layers** and **Ambient Shadows**. The design avoids heavy, dark shadows in favor of light, diffused blurs (e.g., `box-shadow: 0 4px 20px rgba(15, 23, 42, 0.05)`). 

Surfaces that require user input are elevated onto "Level 1" white cards against the off-white background. Critical summary information—like the "Final Total"—should be highlighted using a subtle primary-tinted background (2% opacity) rather than a shadow, keeping the interface feeling "light" and airy.

## Shapes

The design system adopts a **Rounded** (Level 2) language. This 8px base radius (0.5rem) strikes a balance between the technical precision of a financial tool and the approachability of a consumer brand. Form inputs and primary buttons use this consistent radius, while large container cards may scale up to 1rem (rounded-lg) to soften the overall appearance of the page.

## Components

- **Buttons:** Primary buttons are high-contrast Electric Blue with white text. They should include a subtle "micro-bounce" on hover to feel responsive.
- **Input Fields:** Use a floating label pattern to keep the footprint small. Active states must use a 2px Electric Blue border to guide focus.
- **Order Summary Card:** Use a "sticky" behavior on desktop. It features a dashed separator line above the total to evoke a physical receipt metaphor.
- **Checkboxes/Radios:** These are custom-styled with the primary blue. Selection states should be reinforced by a light blue background fill across the entire selection row.
- **Progress Stepper:** A horizontal, non-interactive visual indicator at the top of the page. Completed steps use the Success Green with a checkmark icon.
- **Trust Badges:** Minimalist, monochromatic icons for "Secure SSL" and "Money Back Guarantee" placed near the final call-to-action to provide terminal reassurance.