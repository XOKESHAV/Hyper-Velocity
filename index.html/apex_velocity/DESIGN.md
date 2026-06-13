---
name: Apex Velocity
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
  on-surface-variant: '#ebbbb4'
  inverse-surface: '#e2e2e2'
  inverse-on-surface: '#303030'
  outline: '#b18780'
  outline-variant: '#603e39'
  surface-tint: '#ffb4a8'
  primary: '#ffb4a8'
  on-primary: '#690100'
  primary-container: '#ff5540'
  on-primary-container: '#5c0000'
  inverse-primary: '#c00100'
  secondary: '#ffb596'
  on-secondary: '#581e00'
  secondary-container: '#fe6500'
  on-secondary-container: '#541d00'
  tertiary: '#3cd7ff'
  on-tertiary: '#003642'
  tertiary-container: '#009ebe'
  on-tertiary-container: '#002e3a'
  error: '#ffb4ab'
  on-error: '#690005'
  error-container: '#93000a'
  on-error-container: '#ffdad6'
  primary-fixed: '#ffdad4'
  primary-fixed-dim: '#ffb4a8'
  on-primary-fixed: '#410000'
  on-primary-fixed-variant: '#930100'
  secondary-fixed: '#ffdbcd'
  secondary-fixed-dim: '#ffb596'
  on-secondary-fixed: '#360f00'
  on-secondary-fixed-variant: '#7c2e00'
  tertiary-fixed: '#b4ebff'
  tertiary-fixed-dim: '#3cd7ff'
  on-tertiary-fixed: '#001f27'
  on-tertiary-fixed-variant: '#004e5f'
  background: '#131313'
  on-background: '#e2e2e2'
  surface-variant: '#353535'
typography:
  display-hero:
    fontFamily: anybody
    fontSize: 80px
    fontWeight: '900'
    lineHeight: '1.0'
    letterSpacing: -0.04em
  headline-lg:
    fontFamily: anybody
    fontSize: 48px
    fontWeight: '800'
    lineHeight: '1.1'
    letterSpacing: -0.02em
  headline-lg-mobile:
    fontFamily: anybody
    fontSize: 32px
    fontWeight: '800'
    lineHeight: '1.1'
  stats-data:
    fontFamily: jetbrainsMono
    fontSize: 24px
    fontWeight: '700'
    lineHeight: '1.2'
    letterSpacing: 0.05em
  body-md:
    fontFamily: spaceGrotesk
    fontSize: 16px
    fontWeight: '400'
    lineHeight: '1.6'
  label-caps:
    fontFamily: spaceGrotesk
    fontSize: 12px
    fontWeight: '700'
    lineHeight: '1.0'
    letterSpacing: 0.15em
spacing:
  base: 8px
  gutter: 24px
  margin-desktop: 64px
  margin-mobile: 20px
  max-width: 1440px
---

## Brand & Style

The design system is engineered for the high-octane world of supercar enthusiasts, evoking the visceral sensation of a 200mph sprint. The brand personality is aggressive, prestigious, and technologically advanced. It targets a demographic that values engineering excellence and cinematic aesthetics.

The visual style is a fusion of **Glassmorphism** and **High-Contrast Neon**. It utilizes deep obsidian surfaces layered with translucent glass panels to create a sense of cockpit instrumentation. Carbon fiber textures and sharp, angular motifs represent aerodynamic precision, while vibrant neon glows simulate the heat of friction and the blur of motion at high speeds. The emotional response is one of adrenaline, exclusivity, and raw power.

## Colors

The palette is rooted in a "Pitch Black" environment to maximize the impact of emissive light sources. 

- **Racing Red (Primary):** Used for critical actions, performance peaks, and primary branding. It carries a heavy neon glow to simulate tail lights.
- **Fire Orange (Secondary):** Represents heat, RPM gauges, and secondary highlights.
- **Speed Blue (Accent):** A high-frequency contrast color used for technical data, electric power indicators, and nitrogen-boost metaphors.
- **Backgrounds:** Absolute black (#000000) is mandatory to ensure the glass effects and neon glows pop with cinematic depth.

## Typography

This design system employs a tiered typography strategy to reflect automotive instrumentation:

1.  **Display & Headlines (Anybody):** A variable font with an aggressive width. It should be used in its widest, boldest settings for impact. Italics should be used frequently to suggest forward motion.
2.  **Data & Metrics (JetBrains Mono):** A technical, monospaced font for engine specs, lap times, and performance counters. It conveys precision and "live" telemetry.
3.  **UI & Navigation (Space Grotesk):** A modern, geometric sans-serif that remains legible at smaller sizes while maintaining a futuristic edge.

All headings should favor uppercase styling to reinforce a bold, commanding presence.

## Layout & Spacing

The layout follows a **Fluid Grid** model with generous margins to allow high-resolution car photography to breathe. 

- **Desktop:** 12-column grid with 24px gutters. Content is often staggered or slightly overlapping to create a dynamic, non-linear flow.
- **Mobile:** 4-column grid with 20px margins. Components should stack vertically, prioritizing full-bleed imagery.
- **Spacing Logic:** Use an 8px base unit. Larger gaps (64px+) are used between major content sections to emphasize the premium, spacious feel of a luxury showroom.
- **Safe Zones:** Always leave clear "visual lanes" for background animations or 3D models to peek through the UI.

## Elevation & Depth

Depth is not created with traditional shadows, but through **Optical Layering** and **Luminance**:

- **Layer 0 (Base):** Pitch Black or subtle Carbon Fiber texture.
- **Layer 1 (Glass):** Backdrop-blur (20px+) with a 10% white border. These "containers" represent the cockpit dashboard.
- **Layer 2 (Emissive):** Neon glows (drop-shadows with 0 offset and 15px+ spread) in Racing Red or Fire Orange indicate interactivity or active status.
- **Z-Axis:** Components should utilize a 3D tilt effect (approx 5-10 degrees) on hover, responding to the user's cursor to simulate a physical interface.

## Shapes

The shape language is **Sharp and Aerodynamic**. 

- **Primary Radius:** 0px (Sharp). This reinforces the aggressive, "cut by wind" aesthetic of supercars.
- **Secondary Accents:** Use 45-degree clipped corners (chamfers) for buttons and status indicators instead of rounded corners.
- **Decorative Elements:** Racing flag motifs (chevrons) and slanted separators (italicized dividers) are used to break up horizontal sections.

## Components

- **Performance Counters:** Large, monospaced digits with a flickering "odometer" animation. They must feature a subtle Speed Blue glow.
- **Glassmorphism Car Cards:** Transparent containers with a `backdrop-filter: blur(16px)`. The border should be a 1px gradient from White (20% opacity) to Transparent.
- **Action Buttons:** Sharp-edged with a "Racing Red" fill. On hover, the button should expand slightly and emit a heavy red neon glow.
- **Progress Bars (RPM Style):** Segmented bars that transition from Speed Blue to Fire Orange as they fill, ending in a flashing Racing Red at 100%.
- **3D Tilt Elements:** Any card containing car imagery must apply a CSS `perspective` and `rotate3d` transform on mouse-over.
- **Racing Flag Accents:** Used as headers for lists or tab indicators, consisting of alternating black and dark-gray micro-squares.
- **Input Fields:** Bottom-border only, using a monospaced font. When focused, the border glows in Fire Orange.