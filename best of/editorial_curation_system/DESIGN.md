---
name: Editorial Curation System
colors:
  surface: '#fbf9f9'
  surface-dim: '#dbdad9'
  surface-bright: '#fbf9f9'
  surface-container-lowest: '#ffffff'
  surface-container-low: '#f5f3f3'
  surface-container: '#efeded'
  surface-container-high: '#e9e8e7'
  surface-container-highest: '#e4e2e2'
  on-surface: '#1b1c1c'
  on-surface-variant: '#444748'
  inverse-surface: '#303031'
  inverse-on-surface: '#f2f0f0'
  outline: '#747878'
  outline-variant: '#c4c7c7'
  surface-tint: '#5f5e5e'
  primary: '#000000'
  on-primary: '#ffffff'
  primary-container: '#1c1b1b'
  on-primary-container: '#858383'
  inverse-primary: '#c8c6c5'
  secondary: '#5d5f5d'
  on-secondary: '#ffffff'
  secondary-container: '#e2e3e1'
  on-secondary-container: '#636563'
  tertiary: '#000000'
  on-tertiary: '#ffffff'
  tertiary-container: '#09006b'
  on-tertiary-container: '#7273ff'
  error: '#ba1a1a'
  on-error: '#ffffff'
  error-container: '#ffdad6'
  on-error-container: '#93000a'
  primary-fixed: '#e5e2e1'
  primary-fixed-dim: '#c8c6c5'
  on-primary-fixed: '#1c1b1b'
  on-primary-fixed-variant: '#474746'
  secondary-fixed: '#e2e3e1'
  secondary-fixed-dim: '#c6c7c5'
  on-secondary-fixed: '#1a1c1b'
  on-secondary-fixed-variant: '#454746'
  tertiary-fixed: '#e1dfff'
  tertiary-fixed-dim: '#c1c1ff'
  on-tertiary-fixed: '#09006b'
  on-tertiary-fixed-variant: '#2b20d2'
  background: '#fbf9f9'
  on-background: '#1b1c1c'
  surface-variant: '#e4e2e2'
typography:
  display-lg:
    fontFamily: Newsreader
    fontSize: 72px
    fontWeight: '600'
    lineHeight: '1.1'
    letterSpacing: -0.02em
  display-md:
    fontFamily: Newsreader
    fontSize: 48px
    fontWeight: '600'
    lineHeight: '1.15'
    letterSpacing: -0.01em
  headline-lg:
    fontFamily: Newsreader
    fontSize: 32px
    fontWeight: '500'
    lineHeight: '1.2'
  headline-md:
    fontFamily: Newsreader
    fontSize: 24px
    fontWeight: '500'
    lineHeight: '1.3'
  body-lg:
    fontFamily: Inter
    fontSize: 18px
    fontWeight: '400'
    lineHeight: '1.6'
  body-md:
    fontFamily: Inter
    fontSize: 16px
    fontWeight: '400'
    lineHeight: '1.6'
  label-caps:
    fontFamily: Inter
    fontSize: 12px
    fontWeight: '600'
    lineHeight: '1.4'
    letterSpacing: 0.1em
  caption:
    fontFamily: Inter
    fontSize: 13px
    fontWeight: '400'
    lineHeight: '1.4'
spacing:
  unit: 4px
  xs: 4px
  sm: 8px
  md: 16px
  lg: 24px
  xl: 48px
  xxl: 80px
  gutter: 24px
  margin: 40px
---

## Brand & Style

The design system is anchored in the tradition of high-end editorial print, adapted for a modern digital experience. It targets a discerning audience that values depth, curation, and a quiet sense of luxury. The emotional response is intended to be one of "focused immersion"—where the interface recedes to let photography and long-form thought take center stage.

The design style is a sophisticated blend of **Minimalism** and **High-Contrast Editorial**. It leverages the tension between expansive whitespace and razor-sharp typography. Every element is intentional; there is no decoration for the sake of decoration. Subtle borders and a restricted color palette create a structured, gallery-like environment for content curation.

## Colors

The palette is architectural, relying on a high-contrast foundation to establish hierarchy.

*   **Primary (Charcoal):** Used for typography, iconography, and structural borders. It provides a grounded, authoritative weight.
*   **Secondary (Off-White):** The primary canvas color. It is softer than pure white, reducing eye strain and evoking the feel of premium paper stock.
*   **Tertiary (Electric Indigo):** A high-energy accent used sparingly for interaction cues, active states, and specific curated highlights.
*   **Neutral:** A range of mid-tone greys used for secondary metadata and subtle UI borders to maintain the premium feel without introducing visual noise.

## Typography

Typography is the primary driver of this design system. We utilize a dual-font strategy to create clear editorial distinction.

The **Headline Font (Newsreader)** brings a literary, traditional soul to the system. It should be used for article titles, section headers, and pulled quotes. Tighten letter-spacing on larger display sizes to maintain a bespoke, typeset appearance.

The **Body Font (Inter)** provides a clean, functional counterpoint. Its neutrality ensures legibility in long-form reading and utility in interface elements. Use generous line heights for body copy to facilitate a comfortable reading rhythm. The **Label-Caps** style is essential for categorization and metadata, providing a "tag" feel without requiring heavy containers.

## Layout & Spacing

The layout philosophy follows a **Fixed Grid** approach for desktop to mirror the structured columns of a magazine, transitioning to a fluid model for mobile. 

A 12-column grid provides the framework. However, the system encourages "breaking" the grid with asymmetrical placements or oversized margins to create visual interest. Use the `xxl` spacing unit for vertical padding between major content sections to allow the design to breathe. Gutters are kept wide (24px) to ensure that even dense information feels organized and airy.

## Elevation & Depth

This design system avoids traditional drop shadows in favor of **Low-contrast outlines** and **Tonal layers**. Depth is communicated through structural layering rather than artificial lighting effects.

*   **Borders:** Use 1px borders in a light neutral tone to define content areas. This creates a "boxed" editorial aesthetic.
*   **Z-Index:** Content is layered using flat planes. When a modal or overlay is required, use a solid Off-White background with a subtle, sharp 1px Charcoal border rather than a soft shadow.
*   **Image Treatments:** High-quality imagery should be treated as part of the architecture, often sitting flush against borders or filling entire columns to create a sense of scale.

## Shapes

The design system utilizes a **Sharp (0px)** roundedness level. Square corners reinforce the architectural and print-inspired nature of the brand. This sharpness applies to buttons, input fields, image containers, and cards. The lack of border-radius demands precision in alignment, as every line contributes to the overall structural integrity of the layout.

## Components

Components in this design system are characterized by their skeletal and typographic nature.

*   **Buttons:** Primary buttons are solid Charcoal with White text, using the `label-caps` typography style. Secondary buttons use a 1px border with no fill. Interaction is shown through a color shift to Electric Indigo or a slight opacity change.
*   **Cards:** Content cards should be minimalist. A card consists of a high-resolution image, followed by a `label-caps` category, and a `headline-md` title. Avoid "container" backgrounds for cards; let the image and text sit directly on the page background.
*   **Input Fields:** Use simple bottom-border-only styling or a full 1px border. Focus states are indicated by the border color changing to Electric Indigo.
*   **Chips/Tags:** Small, rectangular boxes with 1px borders. Typography is strictly `label-caps`. 
*   **Curation Grid:** A specific component for the magazine feel—this is a mix of small and large cards that span varying column widths (e.g., one card spanning 8 columns next to one spanning 4) to create an asymmetrical, curated rhythm.
*   **Navigation:** A minimalist top-bar with thin 1px horizontal borders separating it from the content. Use the `label-caps` style for navigation links.