---
name: Aetheric Flux
colors:
  surface: '#001330'
  surface-dim: '#001330'
  surface-bright: '#283958'
  surface-container-lowest: '#000d26'
  surface-container-low: '#071b39'
  surface-container: '#0c1f3d'
  surface-container-high: '#182a48'
  surface-container-highest: '#233554'
  on-surface: '#d7e2ff'
  on-surface-variant: '#c3c6d7'
  inverse-surface: '#d7e2ff'
  inverse-on-surface: '#1f304f'
  outline: '#8d90a0'
  outline-variant: '#434655'
  surface-tint: '#b4c5ff'
  primary: '#b4c5ff'
  on-primary: '#002a78'
  primary-container: '#2563eb'
  on-primary-container: '#eeefff'
  inverse-primary: '#0053db'
  secondary: '#7bd0ff'
  on-secondary: '#00354a'
  secondary-container: '#00a6e0'
  on-secondary-container: '#00374d'
  tertiary: '#d2bbff'
  on-tertiary: '#3f008e'
  tertiary-container: '#8343f4'
  on-tertiary-container: '#f7edff'
  error: '#ffb4ab'
  on-error: '#690005'
  error-container: '#93000a'
  on-error-container: '#ffdad6'
  primary-fixed: '#dbe1ff'
  primary-fixed-dim: '#b4c5ff'
  on-primary-fixed: '#00174b'
  on-primary-fixed-variant: '#003ea8'
  secondary-fixed: '#c4e7ff'
  secondary-fixed-dim: '#7bd0ff'
  on-secondary-fixed: '#001e2c'
  on-secondary-fixed-variant: '#004c69'
  tertiary-fixed: '#eaddff'
  tertiary-fixed-dim: '#d2bbff'
  on-tertiary-fixed: '#25005a'
  on-tertiary-fixed-variant: '#5a00c6'
  background: '#001330'
  on-background: '#d7e2ff'
  surface-variant: '#233554'
typography:
  display-hero:
    fontFamily: Sora
    fontSize: 72px
    fontWeight: '700'
    lineHeight: 80px
    letterSpacing: -0.02em
  display-hero-mobile:
    fontFamily: Sora
    fontSize: 40px
    fontWeight: '700'
    lineHeight: 48px
    letterSpacing: -0.01em
  headline-lg:
    fontFamily: Sora
    fontSize: 40px
    fontWeight: '600'
    lineHeight: 48px
    letterSpacing: -0.01em
  headline-md:
    fontFamily: Sora
    fontSize: 32px
    fontWeight: '600'
    lineHeight: 40px
  headline-sm:
    fontFamily: Sora
    fontSize: 24px
    fontWeight: '600'
    lineHeight: 32px
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
  body-sm:
    fontFamily: Inter
    fontSize: 14px
    fontWeight: '400'
    lineHeight: 20px
  label-md:
    fontFamily: Inter
    fontSize: 12px
    fontWeight: '600'
    lineHeight: 16px
    letterSpacing: 0.05em
rounded:
  sm: 0.25rem
  DEFAULT: 0.5rem
  md: 0.75rem
  lg: 1rem
  xl: 1.5rem
  full: 9999px
spacing:
  unit: 4px
  xs: 4px
  sm: 8px
  md: 16px
  lg: 24px
  xl: 32px
  xxl: 48px
  section: 80px
  gutter: 24px
  margin-mobile: 16px
  margin-desktop: 64px
---

## Brand & Style
The design system embodies a premium, futuristic SaaS aesthetic that prioritizes clarity, depth, and technological sophistication. It targets a high-end enterprise and developer audience, evoking feelings of reliability, cutting-edge innovation, and "quiet luxury" within a digital space. 

The visual style is a hybrid of **Glassmorphism** and **Minimalism**. It utilizes frosted surfaces and subtle background blurs to create a sense of multi-dimensional depth. The interface feels "atmospheric," as if elements are floating in a deep-space environment. High whitespace is used intentionally to separate complex data sets, ensuring that the premium nature of the brand is reflected through generous breathing room and editorial-grade composition.

## Colors
The palette is rooted in a **Deep Navy (#081C3A)** foundation to establish authority and depth. **Electric Blue (#2563EB)** serves as the primary action color, providing a vibrant high-contrast point against the dark backgrounds.

*   **Primary & Secondary:** Used for high-priority actions, active states, and brand-critical iconography.
*   **Accents:** Cyan and Purple are reserved for data visualization, subtle gradients, and status indicators to maintain a "technological" feel.
*   **Surface Strategy:** Instead of solid fills, use semi-transparent hex codes with backdrop filters. Surfaces should feel like "sheets of light" layered over the background mesh gradients. 
*   **Gradients:** Use linear gradients (e.g., `#2563EB` to `#7C3AED`) sparingly for primary buttons and hero typography to signify high-value interactions.

## Typography
The typographic hierarchy relies on the geometric precision of **Sora** for headlines to emphasize the futuristic aesthetic. **Inter** is utilized for body text to ensure maximum legibility and a systematic, clean look across dense data layouts.

*   **Hero Headlines:** Use -2% letter spacing on large display text to create a more compact, high-end editorial feel.
*   **Labels:** All-caps styling with 5% letter spacing is the default for overlines and small metadata to provide a distinct structural rhythm.
*   **Hierarchy:** Maintain a clear vertical rhythm by ensuring line heights are consistently 1.2x to 1.5x the font size.

## Layout & Spacing
The layout uses a **Fluid Grid** model with a 12-column structure for desktop. To maintain the premium feel, the system utilizes a high-whitespace philosophy where section vertical spacing starts at 80px.

*   **Desktop (1440px+):** 12 columns, 24px gutters, 64px side margins.
*   **Tablet (768px - 1439px):** 8 columns, 20px gutters, 32px side margins.
*   **Mobile (0px - 767px):** 4 columns, 16px gutters, 16px side margins.
*   **Rhythm:** All spacing must be multiples of the 4px base unit. Component internal padding should default to `md` (16px) for standard elements and `lg` (24px) for cards.

## Elevation & Depth
Hierarchy is established through **Glassmorphism** and **Tonal Layering** rather than traditional heavy shadows.

*   **Level 0 (Background):** Deep navy gradients or mesh blurs.
*   **Level 1 (Sub-surface):** `surface-container` color with 1px solid `border-glass`. No shadow.
*   **Level 2 (Floating Cards):** `surface` color with `backdrop-filter: blur(12px)`. Subtle 1px gradient border (Top-left: white 20% to Bottom-right: white 0%).
*   **Level 3 (Popovers/Modals):** Same as Level 2 but with a "Global Glow" shadow: `0px 20px 40px rgba(0, 0, 0, 0.4)` and a secondary outer glow of `0px 0px 20px rgba(37, 99, 235, 0.15)`.

## Shapes
The design system uses a generous roundedness to soften the "technical" feel and make the UI more approachable and modern.

*   **Base Radius:** 8px (0.5rem) for inputs and small buttons.
*   **Container Radius:** 20px (1.25rem) for cards and main UI containers.
*   **Pill Radius:** Used exclusively for tags, chips, and specific "Call to Action" buttons to distinguish them from structural elements.

## Components
Consistent styling across components ensures the premium "Vernexify" feel is maintained.

*   **Premium Buttons:** Primary buttons feature a subtle linear gradient background (`Electric Blue` to `Royal Blue`). On hover, they emit a soft outer glow (`accent-glow`) and scale slightly (1.02x).
*   **Glassmorphic Cards:** Use a semi-transparent fill with a 12px backdrop blur. The "Border Gradient" effect is mandatory: a 1px stroke that is brighter on the top-left to simulate a light source.
*   **Input Fields:** Ghost-style inputs with `surface-container` backgrounds. The border should transition from `border-glass` to `primary_color` on focus, accompanied by a subtle inner glow.
*   **Chips/Tags:** Small, high-contrast pills with a light tint of the accent color (e.g., 10% opacity Purple background with 100% opacity Purple text).
*   **Interactive Lists:** Items should have a transparent background that transitions to `surface-container` on hover, with a "left-edge" accent bar appearing in `primary_color`.