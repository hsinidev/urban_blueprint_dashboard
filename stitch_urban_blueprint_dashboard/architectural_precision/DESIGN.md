---
name: Architectural Precision
colors:
  surface: '#f9f9f9'
  surface-dim: '#dadada'
  surface-bright: '#f9f9f9'
  surface-container-lowest: '#ffffff'
  surface-container-low: '#f3f3f3'
  surface-container: '#eeeeee'
  surface-container-high: '#e8e8e8'
  surface-container-highest: '#e2e2e2'
  on-surface: '#1a1c1c'
  on-surface-variant: '#434653'
  inverse-surface: '#2f3131'
  inverse-on-surface: '#f1f1f1'
  outline: '#737784'
  outline-variant: '#c3c6d5'
  surface-tint: '#2559bd'
  primary: '#00327d'
  on-primary: '#ffffff'
  primary-container: '#0047ab'
  on-primary-container: '#a5bdff'
  inverse-primary: '#b1c5ff'
  secondary: '#5f5e5e'
  on-secondary: '#ffffff'
  secondary-container: '#e4e2e1'
  on-secondary-container: '#656464'
  tertiary: '#353737'
  on-tertiary: '#ffffff'
  tertiary-container: '#4b4d4e'
  on-tertiary-container: '#bdbebe'
  error: '#ba1a1a'
  on-error: '#ffffff'
  error-container: '#ffdad6'
  on-error-container: '#93000a'
  primary-fixed: '#dae2ff'
  primary-fixed-dim: '#b1c5ff'
  on-primary-fixed: '#001946'
  on-primary-fixed-variant: '#00419e'
  secondary-fixed: '#e4e2e1'
  secondary-fixed-dim: '#c8c6c6'
  on-secondary-fixed: '#1b1c1c'
  on-secondary-fixed-variant: '#474747'
  tertiary-fixed: '#e2e2e2'
  tertiary-fixed-dim: '#c6c6c7'
  on-tertiary-fixed: '#1a1c1c'
  on-tertiary-fixed-variant: '#454747'
  background: '#f9f9f9'
  on-background: '#1a1c1c'
  surface-variant: '#e2e2e2'
typography:
  h1:
    fontFamily: Inter
    fontSize: 32px
    fontWeight: '700'
    lineHeight: '1.2'
    letterSpacing: -0.02em
  h2:
    fontFamily: Inter
    fontSize: 24px
    fontWeight: '600'
    lineHeight: '1.3'
    letterSpacing: -0.01em
  body-md:
    fontFamily: Inter
    fontSize: 16px
    fontWeight: '400'
    lineHeight: '1.6'
    letterSpacing: '0'
  data-lg:
    fontFamily: JetBrains Mono
    fontSize: 18px
    fontWeight: '500'
    lineHeight: '1.2'
    letterSpacing: -0.01em
  data-sm:
    fontFamily: JetBrains Mono
    fontSize: 12px
    fontWeight: '400'
    lineHeight: '1.0'
    letterSpacing: 0.02em
  label-caps:
    fontFamily: JetBrains Mono
    fontSize: 10px
    fontWeight: '700'
    lineHeight: '1.0'
    letterSpacing: 0.1em
spacing:
  base: 4px
  xs: 8px
  sm: 16px
  md: 24px
  lg: 40px
  xl: 64px
  border-hairline: 1px
  grid-gutter: 16px
---

## Brand & Style

The design system is engineered to evoke the meticulous precision of architectural drafting and high-end structural engineering. It targets institutional investors and property developers who demand clarity, speed, and technical depth. The aesthetic is "Structural Minimalism"—a blend of high-contrast data visualization and drafting-room utility.

The UI should feel like a premium BIM (Building Information Modeling) tool tailored for the boardroom. It prioritizes information density without clutter, using hairline strokes and mathematical alignment to convey a sense of structural integrity. Every element is intentional, removing decorative flourishes in favor of engineering-grade functionalism.

## Colors

The palette is derived from traditional architectural blueprints and modern construction materials. 

- **Blueprint Blue (#0047AB):** Used for primary actions, structural highlights, and active states. It represents the "ink" of the design.
- **Graphite (#333333):** The foundation for text, iconography, and heavy structural borders.
- **Pure White (#FFFFFF):** The primary canvas color, ensuring maximum legibility and a "clean site" feel.
- **Technical Accents:** Subtle gray washes are used for grid lines and blueprint-patterned backgrounds to provide depth without distracting from data.

Data visualizations should utilize high-contrast variations of the primary blue and graphite to ensure technical charts are legible at a glance, especially on mobile devices.

## Typography

This design system utilizes a dual-font approach to distinguish between narrative content and technical data. 

**Inter** handles all UI labels, headings, and instructional text. It provides a modern, neutral foundation that stays out of the way of the content.

**JetBrains Mono** is reserved exclusively for numerical data, timestamps, coordinates, and investor alerts. Its monospaced nature ensures that columns of numbers align perfectly in dashboards, echoing the look of an engineer’s site log. All technical labels use uppercase styling with increased letter spacing to mimic architectural titling blocks.

## Layout & Spacing

The layout is governed by a strict 8px square grid system. Every component, margin, and padding must be a multiple of this base unit to maintain mathematical consistency.

- **Mobile Architecture:** A 4-column fluid grid. The 'Live-Site-Cam' feed occupies the top quadrant of the screen, pinned for immediate access.
- **Desktop Architecture:** A 12-column fixed grid with a 280px sidebar modeled after a drafting "Legend" block.
- **Hairline Borders:** Elements are separated by 1px solid borders in Graphite (#333333) or Light Gray (#E0E0E0). These borders never use rounded corners.
- **Blueprint Pattern:** Large empty states or background sections feature a subtle 32px repeating dot or crosshair grid pattern in 5% opacity Blueprint Blue.

## Elevation & Depth

In keeping with the architectural theme, this design system avoids soft ambient shadows. Depth is instead communicated through **structural layering** and **line weight**.

- **Level 0 (Site):** The background canvas. Pure White or light gray blueprint pattern.
- **Level 1 (Foundation):** Components like cards and input fields. Defined by 1px Graphite outlines. No shadow.
- **Level 2 (Scaffolding):** Overlays and modals. These use a slightly thicker 2px border or a high-contrast Graphite fill with white text to "pop" from the layout.
- **Glassmorphism:** Reserved exclusively for mobile video overlays. Live-site cam controls use a 20px backdrop blur with a 60% opacity white fill to ensure controls remain visible over fluctuating site footage.

## Shapes

The shape language is strictly **Sharp (0px)**. All containers, buttons, and input fields feature 90-degree corners. 

This lack of rounding reinforces the "Engineering-grade" narrative and allows components to sit perfectly flush against one another, mimicking stacked building materials or floor plans. Circular shapes are permitted only for status indicators (e.g., a "Live" recording dot) or user avatars to provide a clear visual distinction from structural UI elements.

## Components

### Live-Site-Cams
Video containers feature a 1px Graphite border with a "viewfinder" overlay—four L-shaped corner brackets in Blueprint Blue. Metadata (timestamp, weather, site location) is overlaid using **JetBrains Mono** in a semi-transparent black bar at the bottom.

### Investor Alerts
High-priority notifications use a "Caution Tape" aesthetic: a 4px left-border in Status Alert Red, a White background, and Graphite text. The alert icon is always a geometric primitive (triangle or square).

### Buttons
Buttons are rectangular with 1px borders. Primary buttons use a solid Blueprint Blue fill. Secondary buttons use a white fill with a Graphite border. Ghost buttons are reserved for technical toggles and use JetBrains Mono text.

### Technical Data Viz
Charts must use thin stroke widths (1px - 1.5px). Data points are marked with small crosshairs rather than solid dots. Grids within charts must align with the global 8px spacing system.

### Input Fields
Fields are represented as simple underline strokes (1px Graphite) or full-bordered boxes. Labels sit above the field in **label-caps** style. Focus states are indicated by the border color shifting to Blueprint Blue.