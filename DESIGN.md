---
name: Kinetic Redline
colors:
  surface: '#131313'
  surface-dim: '#131313'
  surface-bright: '#3a3939'
  surface-container-lowest: '#0e0e0e'
  surface-container-low: '#1c1b1b'
  surface-container: '#201f1f'
  surface-container-high: '#2a2a2a'
  surface-container-highest: '#353534'
  on-surface: '#e5e2e1'
  on-surface-variant: '#e9bcb9'
  inverse-surface: '#e5e2e1'
  inverse-on-surface: '#313030'
  outline: '#b08784'
  outline-variant: '#5f3e3d'
  surface-tint: '#ffb3af'
  primary: '#ffb3af'
  on-primary: '#68000e'
  primary-container: '#ff5357'
  on-primary-container: '#5c000b'
  inverse-primary: '#bf0024'
  secondary: '#c8c6c5'
  on-secondary: '#313030'
  secondary-container: '#474746'
  on-secondary-container: '#b7b5b4'
  tertiary: '#c8c6c6'
  on-tertiary: '#303030'
  tertiary-container: '#919090'
  on-tertiary-container: '#292a2a'
  error: '#ffb4ab'
  on-error: '#690005'
  error-container: '#93000a'
  on-error-container: '#ffdad6'
  primary-fixed: '#ffdad8'
  primary-fixed-dim: '#ffb3af'
  on-primary-fixed: '#410006'
  on-primary-fixed-variant: '#930019'
  secondary-fixed: '#e5e2e1'
  secondary-fixed-dim: '#c8c6c5'
  on-secondary-fixed: '#1c1b1b'
  on-secondary-fixed-variant: '#474746'
  tertiary-fixed: '#e4e2e2'
  tertiary-fixed-dim: '#c8c6c6'
  on-tertiary-fixed: '#1b1c1c'
  on-tertiary-fixed-variant: '#474747'
  background: '#131313'
  on-background: '#e5e2e1'
  surface-variant: '#353534'
typography:
  headline-xl:
    fontFamily: Space Grotesk
    fontSize: 48px
    fontWeight: '700'
    lineHeight: '1.1'
    letterSpacing: -0.02em
  headline-lg:
    fontFamily: Space Grotesk
    fontSize: 32px
    fontWeight: '700'
    lineHeight: '1.2'
    letterSpacing: -0.01em
  headline-lg-mobile:
    fontFamily: Space Grotesk
    fontSize: 24px
    fontWeight: '700'
    lineHeight: '1.2'
  body-md:
    fontFamily: Hanken Grotesk
    fontSize: 16px
    fontWeight: '400'
    lineHeight: '1.6'
  label-sm:
    fontFamily: JetBrains Mono
    fontSize: 12px
    fontWeight: '500'
    lineHeight: '1.0'
    letterSpacing: 0.1em
  button-text:
    fontFamily: Space Grotesk
    fontSize: 14px
    fontWeight: '600'
    lineHeight: '1.0'
    letterSpacing: 0.05em
spacing:
  unit: 4px
  gutter: 24px
  margin-mobile: 16px
  margin-desktop: 64px
  container-max: 1280px
---

## Brand & Style

The design system is engineered for high-performance gaming configurations, targeting competitive players who demand precision and speed. The visual identity is aggressive, technical, and high-contrast, drawing heavily from **Modern Cyber-Brutalism** and **Tactile Glassmorphism**. 

The interface should feel like a high-end military or racing telemetry dashboard. It utilizes "Carbon Black" depth to create a focused environment where "Neon Red" serves as the primary signal for action and data importance. The emotional response is one of intensity, urgency, and technical superiority. 

Key stylistic pillars include:
- **Luminous Hierarchy:** Using neon glows to denote active states and primary calls to action.
- **Technical Rigor:** Sharp edges mixed with precise, thin-stroke borders.
- **Dynamic Energy:** Subtle pulse animations on critical status indicators to simulate a living machine.

## Colors

The palette is strictly limited to maintain an aggressive, focused aesthetic. 

- **Primary (Neon Red):** Used for primary buttons, active toggles, and critical alerts. It must always carry a subtle outer glow when used against dark backgrounds to simulate a neon light source.
- **Neutral (Carbon Black):** The base layer of the application. It provides the deep contrast necessary for the red elements to pop.
- **Surface (Dark Gray):** Used for secondary containers and cards to create depth without breaking the dark-mode immersion.
- **Functional Colors:** Success states use a sharp Cyan to contrast the Red, while warnings remain in high-saturation Orange.

## Typography

This design system utilizes a trio of fonts to balance futuristic flair with technical readability. 

- **Display & Headings:** Space Grotesk provides a modern, geometric tech feel with wide apertures. Headlines should use tight tracking to feel dense and impactful.
- **Body Text:** Hanken Grotesk is used for long-form content and descriptions, offering high legibility in low-light (dark mode) environments.
- **Data & Labels:** JetBrains Mono is utilized for technical specs, XIM configuration codes, and metadata, evoking a "developer" or "hacker" aesthetic.

All labels should be uppercase with increased letter spacing to enhance the "UI dashboard" feel.

## Layout & Spacing

The layout follows a **Rigid Grid** philosophy. Elements are aligned to a 4px baseline grid to ensure mathematical precision.

- **Grid:** A 12-column grid for desktop with 24px gutters. On mobile, this collapses to a 4-column grid.
- **Sectioning:** Content sections should be separated by heavy 2px horizontal rules in #1A1A1A to maintain a "structured" look.
- **Density:** High information density is preferred. Padding should be sufficient for touch targets but compact enough to show multiple configuration parameters at once.

## Elevation & Depth

Depth is achieved through **Tonal Layering** and **Glassmorphism**, rather than traditional soft shadows.

- **Base Level:** #0A0A0A (Pure dark background).
- **Surface Level (Cards):** #121212 with a 1px solid border (#4D4D4D). 
- **Glass Effect:** For floating menus or modals, use a backdrop-blur (12px) with a semi-transparent dark fill (rgba(18, 18, 18, 0.8)).
- **Interactivity:** Elements "lift" by increasing the intensity of their border-color or adding the Neon Red outer glow (`box-shadow: 0 0 15px rgba(255, 0, 51, 0.5)`).

## Shapes

The shape language is **Sharp and Aggressive**. 

- **Radii:** All primary UI components (buttons, inputs, cards) must have 0px border radius. 
- **Accents:** Use "clipped corners" (45-degree chamfers) on decorative elements or primary section headers to reinforce the high-tech, military hardware aesthetic.
- **Borders:** Constant 1px or 2px borders are preferred over shadows to define shapes.

## Components

- **Buttons:** 
  - *Primary:* Solid Neon Red background, black text, no radius. On hover, apply a strong red outer glow.
  - *Secondary:* Transparent background, 2px Neon Red border, red text.
- **Config Cards:** Use the "Glassmorphism" style. A dark semi-transparent fill, 1px border, and a subtle "scanline" pattern overlay (low opacity) to give it a CRT/Terminal feel.
- **Accordions (FAQ):** Sharp headers with a red vertical accent bar on the left. The chevron icon should be a minimalist "plus/minus" in JetBrains Mono.
- **Input Fields:** Bottom-border only, or a full 1px #4D4D4D border. Focus state changes border to Neon Red with a faint glow.
- **Status Indicators:** Use a pulsing animation on a small 8px square for "Live" or "Active" configuration states.
- **Data Tables:** Use striped rows with alternating shades of Carbon Black and Dark Gray. No vertical grid lines.