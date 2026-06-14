---
name: Momentum Growth System
colors:
  surface: '#f8f9ff'
  surface-dim: '#cbdbf5'
  surface-bright: '#f8f9ff'
  surface-container-lowest: '#ffffff'
  surface-container-low: '#eff4ff'
  surface-container: '#e5eeff'
  surface-container-high: '#dce9ff'
  surface-container-highest: '#d3e4fe'
  on-surface: '#0b1c30'
  on-surface-variant: '#3c4a42'
  inverse-surface: '#213145'
  inverse-on-surface: '#eaf1ff'
  outline: '#6c7a71'
  outline-variant: '#bbcabf'
  surface-tint: '#006c49'
  primary: '#006c49'
  on-primary: '#ffffff'
  primary-container: '#10b981'
  on-primary-container: '#00422b'
  inverse-primary: '#4edea3'
  secondary: '#0058be'
  on-secondary: '#ffffff'
  secondary-container: '#2170e4'
  on-secondary-container: '#fefcff'
  tertiary: '#855300'
  on-tertiary: '#ffffff'
  tertiary-container: '#e29100'
  on-tertiary-container: '#523200'
  error: '#ba1a1a'
  on-error: '#ffffff'
  error-container: '#ffdad6'
  on-error-container: '#93000a'
  primary-fixed: '#6ffbbe'
  primary-fixed-dim: '#4edea3'
  on-primary-fixed: '#002113'
  on-primary-fixed-variant: '#005236'
  secondary-fixed: '#d8e2ff'
  secondary-fixed-dim: '#adc6ff'
  on-secondary-fixed: '#001a42'
  on-secondary-fixed-variant: '#004395'
  tertiary-fixed: '#ffddb8'
  tertiary-fixed-dim: '#ffb95f'
  on-tertiary-fixed: '#2a1700'
  on-tertiary-fixed-variant: '#653e00'
  background: '#f8f9ff'
  on-background: '#0b1c30'
  surface-variant: '#d3e4fe'
typography:
  display-metrics:
    fontFamily: Hanken Grotesk
    fontSize: 48px
    fontWeight: '700'
    lineHeight: 56px
    letterSpacing: -0.02em
  headline-lg:
    fontFamily: Hanken Grotesk
    fontSize: 32px
    fontWeight: '600'
    lineHeight: 40px
    letterSpacing: -0.01em
  headline-lg-mobile:
    fontFamily: Hanken Grotesk
    fontSize: 24px
    fontWeight: '600'
    lineHeight: 32px
  headline-md:
    fontFamily: Hanken Grotesk
    fontSize: 20px
    fontWeight: '600'
    lineHeight: 28px
  body-lg:
    fontFamily: Inter
    fontSize: 18px
    fontWeight: '400'
    lineHeight: 28px
  body-md:
    fontFamily: Inter
    fontSize: 16px
    fontWeight: '400'
    lineHeight: 24px
  label-caps:
    fontFamily: JetBrains Mono
    fontSize: 12px
    fontWeight: '500'
    lineHeight: 16px
    letterSpacing: 0.05em
  label-sm:
    fontFamily: Inter
    fontSize: 12px
    fontWeight: '500'
    lineHeight: 16px
rounded:
  sm: 0.25rem
  DEFAULT: 0.5rem
  md: 0.75rem
  lg: 1rem
  xl: 1.5rem
  full: 9999px
spacing:
  unit: 8px
  container-max-width: 1200px
  gutter: 24px
  margin-mobile: 16px
  margin-desktop: 48px
  stack-sm: 8px
  stack-md: 16px
  stack-lg: 32px
---

## Brand & Style

This design system is built on the principles of **Modern Clarity** and **Positive Reinforcement**. The brand personality is encouraging, organized, and high-fidelity, designed to reduce cognitive load while providing a sense of forward motion. 

The aesthetic leans into **Minimalism** with a **Tactile** edge. It utilizes generous whitespace to prevent the "clutter anxiety" often found in productivity tools. Success is not just tracked; it is celebrated through vibrant color accents and refined micro-interactions. The interface should feel like a premium physical planner translated into a fluid digital experience—clean enough to focus, but structured enough to feel reliable.

## Colors

The color strategy centers on semantic clarity. 
- **Success Green (#10B981):** Used exclusively for progress completion, achievement states, and positive growth metrics.
- **Focus Blue (#3B82F6):** Used for active states, current goals, and primary navigation elements. It represents deep work and concentration.
- **Warm Amber (#F59E0B):** A tertiary accent for "at risk" goals or streaks that require attention, providing a non-alarming nudge.
- **Neutrals:** A palette of Slate grays (from #F8FAFC to #0F172A) provides a sophisticated, stable foundation that lets the success metrics "pop" without overwhelming the user.

## Typography

The typography system uses a tri-font approach to balance professional precision with readability.
- **Hanken Grotesk** is used for headlines and large progress metrics. Its sharp, contemporary geometry feels modern and highly legible at large scales.
- **Inter** serves as the workhorse for all body copy and descriptions, chosen for its neutral, systematic utility.
- **JetBrains Mono** is used sparingly for labels, timers, and data-driven metadata (like dates or streak counts) to give a technical, "measured" feel to the tracking aspect.

Scale headers down by one tier for mobile devices to maintain a comfortable reading rhythm.

## Layout & Spacing

This design system employs a **Fluid Grid** model with a strict 8px baseline power-of-two rhythm. 

- **Desktop:** 12-column grid with 24px gutters. Content is centered with a max-width of 1200px to maintain focus.
- **Mobile:** Single column with 16px side margins.
- **Rhythm:** Use "Stack" spacing for vertical relationships. Components are grouped using `stack-sm` (8px) for related items (label + input) and `stack-lg` (32px) for major sections.

The layout should feel "airy." If a screen feels crowded, increase the vertical padding rather than reducing the font size.

## Elevation & Depth

To maintain the high-fidelity and modern feel, depth is conveyed through **Tonal Layers** and **Ambient Shadows**.

- **Surfaces:** Use a layered approach. The base background is `#F8FAFC`. Secondary containers (cards, goal blocks) use pure white `#FFFFFF`.
- **Shadows:** Use extremely soft, low-opacity shadows with a slight Blue-Slate tint. Avoid harsh blacks. A "Floating" element should have a shadow like `0 10px 25px -5px rgba(51, 65, 85, 0.1)`.
- **Interactions:** Use a subtle "lift" effect on hover for goal cards—decreasing the shadow blur and slightly scaling the element (1.02x) to provide a tactile, encouraging response.

## Shapes

The shape language is **Rounded (Level 2)**. 

This level of corner radius (0.5rem / 8px for standard components) balances the professional "Focus Blue" aesthetic with the "Success Green" friendliness. It avoids the clinical feel of sharp corners while remaining more structured than a fully pill-shaped "playful" UI. 

- Standard Components (Buttons, Inputs): 8px
- Large Containers (Goal Cards, Progress Overviews): 16px (rounded-lg)
- Special Elements (Avatars, Tags): 24px+ (rounded-xl or full-round)

## Components

- **Buttons:** Primary buttons use a solid Focus Blue with white text. Success actions (e.g., "Complete Goal") use Success Green. Use 16px vertical padding for a substantial, high-fidelity feel.
- **Progress Bars:** Use a thick 8px track height. The background track is a very light gray-blue, and the progress fill is a vibrant Success Green gradient.
- **Goal Cards:** White background, 1px subtle border (#E2E8F0), and a `rounded-lg` corner. These should feature a prominent "Current Metric" in Hanken Grotesk.
- **Chips/Tags:** Use the Label-Caps typography. For status tags, use low-saturation background tints of the primary colors (e.g., Success Green at 10% opacity with 100% opacity text).
- **Inputs:** Clean, outline-style fields. On focus, the border transitions to Focus Blue with a 2px outer "glow" (soft shadow).
- **Checkboxes:** When checked, they should animate with a "pop" scale effect and fill with Success Green.
- **Streaks:** A specialized component using JetBrains Mono for the number count, paired with a small fire or star icon in Warm Amber.