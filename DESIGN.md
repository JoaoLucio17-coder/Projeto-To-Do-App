---
name: Frutiger Aero Revival
colors:
  surface: '#f6faff'
  surface-dim: '#d6dae1'
  surface-bright: '#f6faff'
  surface-container-lowest: '#ffffff'
  surface-container-low: '#eff4fb'
  surface-container: '#e9eef5'
  surface-container-high: '#e4e9ef'
  surface-container-highest: '#dee3e9'
  on-surface: '#171c21'
  on-surface-variant: '#3e4851'
  inverse-surface: '#2c3136'
  inverse-on-surface: '#ecf1f8'
  outline: '#6e7882'
  outline-variant: '#bdc8d2'
  surface-tint: '#006492'
  primary: '#006492'
  on-primary: '#ffffff'
  primary-container: '#00b2ff'
  on-primary-container: '#004161'
  inverse-primary: '#8bceff'
  secondary: '#286c00'
  on-secondary: '#ffffff'
  secondary-container: '#97fb66'
  on-secondary-container: '#2b7300'
  tertiary: '#895100'
  on-tertiary: '#ffffff'
  tertiary-container: '#ef9206'
  on-tertiary-container: '#5a3400'
  error: '#ba1a1a'
  on-error: '#ffffff'
  error-container: '#ffdad6'
  on-error-container: '#93000a'
  primary-fixed: '#c9e6ff'
  primary-fixed-dim: '#8bceff'
  on-primary-fixed: '#001e2f'
  on-primary-fixed-variant: '#004b6f'
  secondary-fixed: '#97fb66'
  secondary-fixed-dim: '#7cdd4c'
  on-secondary-fixed: '#072100'
  on-secondary-fixed-variant: '#1c5200'
  tertiary-fixed: '#ffdcbc'
  tertiary-fixed-dim: '#ffb86b'
  on-tertiary-fixed: '#2c1700'
  on-tertiary-fixed-variant: '#683d00'
  background: '#f6faff'
  on-background: '#171c21'
  surface-variant: '#dee3e9'
typography:
  headline-lg:
    fontFamily: Quicksand
    fontSize: 40px
    fontWeight: '700'
    lineHeight: '1.2'
    letterSpacing: -0.02em
  headline-md:
    fontFamily: Quicksand
    fontSize: 28px
    fontWeight: '600'
    lineHeight: '1.3'
  body-lg:
    fontFamily: Quicksand
    fontSize: 18px
    fontWeight: '500'
    lineHeight: '1.5'
  body-md:
    fontFamily: Quicksand
    fontSize: 16px
    fontWeight: '400'
    lineHeight: '1.5'
  label-sm:
    fontFamily: Quicksand
    fontSize: 12px
    fontWeight: '600'
    lineHeight: '1'
    letterSpacing: 0.05em
rounded:
  sm: 0.5rem
  DEFAULT: 1rem
  md: 1.5rem
  lg: 2rem
  xl: 3rem
  full: 9999px
spacing:
  unit: 8px
  container-padding: 24px
  gutter: 16px
  margin-mobile: 16px
  margin-desktop: 64px
---

## Brand & Style

The design system is rooted in the "Frutiger Aero" aesthetic—a celebration of mid-2000s techno-optimism. It evokes a sense of freshness, clarity, and harmony between the digital and natural worlds. The brand personality is bright, accessible, and high-fidelity, designed to make productivity feel as effortless as a summer breeze.

The visual language utilizes **Skeuomorphic Glassmorphism**. Unlike modern flat design, this system embraces depth through physical metaphors: glossy surfaces that look like polished acrylic, buttons that feel like "jelly," and backgrounds that mimic the expansive depth of a clear blue sky. The emotional response is one of nostalgia and cleanliness, providing a tranquil environment for task management.

## Colors

The palette is anchored by the "Aero Blue" and "Grass Green" spectrum, creating a high-energy, high-contrast environment.

- **Primary (#00b2ff):** Used for interactive states and primary actions, representing the sky.
- **Secondary (#6bcb3c):** Used for "Complete" states and success indicators, representing lush fields.
- **Background (#d9e3f0):** A soft, atmospheric blue-grey that serves as the canvas for transparent layers.
- **Accent (#ffcce7):** A "soap bubble" pink used sparingly for highlights or notification pings.
- **Dark Blue (#0079bf):** Used for high-contrast text and grounding elements.

Gradients are mandatory. Avoid flat fills. Every color should include a linear gradient moving from a saturated base to a lighter, more crystalline top-edge.

## Typography

This design system uses **Quicksand** exclusively to maintain a soft, friendly, and organic feel. The rounded terminals of the typeface complement the bubble and droplet motifs found in the UI components.

Headlines should utilize a subtle "white glow" text shadow when placed over darker gradients to ensure legibility and enhance the "glass" effect. Body text should remain high-contrast (Dark Blue) to ensure the productivity aspect of the app is not lost in the aesthetic.

## Layout & Spacing

The layout philosophy follows a **Fluid Grid** with generous whitespace to simulate the feeling of an open landscape.

- **Mobile:** A single-column layout with 16px margins. Cards float atop the background with a minimum 12px vertical gap.
- **Desktop:** A 12-column grid. The main task list sits in a central 8-column container, while sidebars utilize glassmorphic panels that allow the background sky-gradients to peek through.

Spacing should feel "airy." Avoid tight clusters. Every major container should feel like an island floating within the UI.

## Elevation & Depth

Depth is the defining characteristic of the design system. It is achieved through three specific layers:

1.  **Backdrop:** High-saturation photographic gradients (skies, grass, sun flares).
2.  **Glass Layer:** Surfaces use `backdrop-filter: blur(12px)` with a 40% white opacity. They must feature a 1px solid white border at 50% opacity to simulate a "specular edge."
3.  **Floating Elements:** Interactive elements use "Jelly Shadows"—diffused, color-tinted shadows (e.g., a blue button casts a blue shadow) with an additional inner-white-glow to create a convex, 3D appearance.

Use "Water Droplet" highlights: small, high-opacity white circular gradients in the top-left corners of buttons to simulate a light source.

## Shapes

The shape language is dominated by **hyper-roundedness**. 

- **Primary Buttons/Inputs:** Use pill-shaped (fully rounded) corners to mimic organic, pebble-like forms.
- **Containers/Cards:** Use `rounded-xl` (1.5rem) to maintain a soft, friendly structure.
- **Icons:** Should be encased in circular glass containers or "bubbles."

Avoid sharp 90-degree angles entirely. Every corner should feel "huggable" and liquid.

## Components

### Buttons
Buttons are "Jelly" styled. They feature a dual-tone linear gradient, a 1px internal white border, and a "gloss overlay"—a semi-transparent white elliptical shape covering the top half of the button to simulate a reflective shine.

### To-Do Cards
Cards use the glassmorphism spec: blurred background, semi-transparent fill, and a crisp white outline. When a task is hovered, the card should scale slightly (1.02x) and the blur intensity should increase, making it feel like it's "lifting" toward the user.

### Checkboxes
Checkboxes are stylized as "Water Droplets." An empty state is a subtle, indented glass circle. A completed state fills the circle with the Secondary Green gradient and a white "liquid" checkmark.

### Progress Bars
The progress bar mimics a glass tube filled with green liquid. Use a "bubble" animation—small, rising white spheres—inside the filled portion of the bar to indicate active progress.

### Navigation
The navigation bar should be a floating pill at the bottom of the screen, utilizing a heavy backdrop blur to separate it from the scrolling content beneath.