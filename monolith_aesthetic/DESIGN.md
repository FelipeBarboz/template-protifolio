---
name: Monolith Aesthetic
colors:
  surface: '#131313'
  surface-dim: '#131313'
  surface-bright: '#393939'
  surface-container-lowest: '#0e0e0e'
  surface-container-low: '#1b1b1b'
  surface-container: '#1f1f1f'
  surface-container-high: '#2a2a2a'
  surface-container-highest: '#353535'
  on-surface: '#e2e2e2'
  on-surface-variant: '#c4c7c8'
  inverse-surface: '#e2e2e2'
  inverse-on-surface: '#303030'
  outline: '#8e9192'
  outline-variant: '#444748'
  surface-tint: '#c6c6c7'
  primary: '#ffffff'
  on-primary: '#2f3131'
  primary-container: '#e2e2e2'
  on-primary-container: '#636565'
  inverse-primary: '#5d5f5f'
  secondary: '#c8c6c5'
  on-secondary: '#313030'
  secondary-container: '#4a4949'
  on-secondary-container: '#bab8b7'
  tertiary: '#ffffff'
  on-tertiary: '#303030'
  tertiary-container: '#e4e2e1'
  on-tertiary-container: '#656464'
  error: '#ffb4ab'
  on-error: '#690005'
  error-container: '#93000a'
  on-error-container: '#ffdad6'
  primary-fixed: '#e2e2e2'
  primary-fixed-dim: '#c6c6c7'
  on-primary-fixed: '#1a1c1c'
  on-primary-fixed-variant: '#454747'
  secondary-fixed: '#e5e2e1'
  secondary-fixed-dim: '#c8c6c5'
  on-secondary-fixed: '#1c1b1b'
  on-secondary-fixed-variant: '#474646'
  tertiary-fixed: '#e4e2e1'
  tertiary-fixed-dim: '#c8c6c5'
  on-tertiary-fixed: '#1b1c1c'
  on-tertiary-fixed-variant: '#474746'
  background: '#131313'
  on-background: '#e2e2e2'
  surface-variant: '#353535'
typography:
  display-xl:
    fontFamily: Epilogue
    fontSize: 160px
    fontWeight: '800'
    lineHeight: '0.9'
    letterSpacing: -0.04em
  display-lg:
    fontFamily: Epilogue
    fontSize: 120px
    fontWeight: '700'
    lineHeight: '0.95'
    letterSpacing: -0.03em
  headline-xl:
    fontFamily: Epilogue
    fontSize: 80px
    fontWeight: '700'
    lineHeight: '1.0'
    letterSpacing: -0.02em
  headline-md:
    fontFamily: Epilogue
    fontSize: 48px
    fontWeight: '600'
    lineHeight: '1.1'
    letterSpacing: -0.01em
  body-lg:
    fontFamily: Inter
    fontSize: 20px
    fontWeight: '400'
    lineHeight: '1.6'
    letterSpacing: '0'
  body-md:
    fontFamily: Inter
    fontSize: 16px
    fontWeight: '400'
    lineHeight: '1.5'
    letterSpacing: '0'
  label-sm:
    fontFamily: Inter
    fontSize: 12px
    fontWeight: '600'
    lineHeight: '1'
    letterSpacing: 0.1em
spacing:
  nav-padding: 10px
  footer-padding: 10px
  grid-margin: 40px
  section-gap: 160px
  element-gap: 20px
  base-unit: 10px
---

## Brand & Style

This design system is defined by an uncompromising, high-contrast editorial aesthetic. It draws inspiration from mid-century Swiss modernism and contemporary digital manifestos, where content is not just supported by the UI, but *is* the UI. The brand personality is authoritative, intellectual, and intentionally sparse, stripping away decorative elements to favor the raw power of scale and stark value transitions.

The target audience consists of high-end collaborators and patrons who value clarity over clutter. By utilizing a dark, minimalist approach, the design system evokes a sense of prestige and focus, positioning the portfolio as a definitive statement rather than a mere collection of work.

## Colors

The palette for this design system is strictly monochrome to ensure maximum visual impact through contrast rather than hue. The background is a deep, true black to create an infinite canvas, while the primary foreground is pure white for surgical legibility.

Secondary and tertiary grays are used sparingly to define structural boundaries or secondary information. The high-contrast relationship between #000000 and #FFFFFF is the core driver of the visual hierarchy, ensuring that the typography commands immediate attention.

## Typography

Typography is the foundational pillar of this design system. It utilizes **Epilogue** for all display and headline elements to provide a distinctive, geometric, and almost architectural character. The "Display XL" and "Display LG" sizes are intended to break standard layout conventions, often bleeding to the edges of the viewport or overlapping imagery.

**Inter** is employed for body text and labels to maintain functional clarity and an unobtrusive, systematic feel. High-scale text should be treated as a graphic element; use tight line heights and negative letter spacing for display levels to create "text-blocks" that feel solid and heavy.

## Layout & Spacing

The layout follows a strict 12-column modular grid with a heavy emphasis on verticality and whitespace. A unique constraint of this design system is the 10px padding logic applied to navigation bars and footers, creating a thin, precise frame around the massive internal content.

Large-scale sections are separated by significant gaps (160px+) to allow the bold typography breathing room. Content should be aligned to a rigid grid, but display text may occasionally break the grid to create a sense of dynamic energy. Avoid fluid stretching; instead, anchor elements to the grid columns with fixed-width behaviors for precise control over text wrapping.

## Elevation & Depth

This design system rejects the use of shadows, blurs, or gradients. Depth is conveyed exclusively through **Tonal Layering** and **Scale**.

1.  **Z-0 (Base):** True Black (#000000).
2.  **Z-1 (Overlays/Cards):** Deep Gray (#121212) or White (#FFFFFF) with no shadow.
3.  **Outlines:** Use 1px solid White or Gray borders to define boundaries where tonal contrast is insufficient. 

The visual "weight" comes from the mass of the typography rather than perceived physical height. Overlapping elements (text over images) should rely on blend modes or high-contrast background shifts to maintain legibility.

## Shapes

The shape language is strictly **Sharp (0px)**. Every element—including buttons, input fields, image containers, and cards—must utilize right angles. This reinforces the manifesto-style aesthetic, creating a sense of structural permanence and precision. Avoid any form of rounding or "softness" to maintain the aggressive, high-end minimalist tone.

## Components

### Buttons
Primary buttons are solid White with Black "Inter" text in all-caps. They feature 10px internal padding to align with the navigation logic. Hover states invert the colors (Black background with White border). Secondary buttons are ghost-style with a 1px white border.

### Navigation & Footer
Both components must adhere to the 10px padding rule. Use the `label-sm` typography style for menu items to create a delicate contrast against the massive headlines found in the main content area.

### Cards
Cards are defined by 1px white borders or simple tonal shifts to #121212. They should never have shadows. Headers within cards should use `headline-md` to maintain the design system's emphasis on bold text.

### Input Fields
Inputs are minimalist, consisting only of a 1px white bottom border. Focus states increase the border weight to 2px. Labels use the `label-sm` style and are positioned directly above the input line.

### Lists
Lists are high-contrast. Each item is separated by a 1px gray border. Large-scale numbers (using Epilogue) can be used as bullet points to turn simple lists into major visual features of the layout.