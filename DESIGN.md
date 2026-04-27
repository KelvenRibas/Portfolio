---
name: Cyber-Minimalist Portfolio
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
  on-surface-variant: '#cbc7ab'
  inverse-surface: '#e5e2e1'
  inverse-on-surface: '#313030'
  outline: '#949278'
  outline-variant: '#494832'
  surface-tint: '#d2cc00'
  primary: '#ffffff'
  on-primary: '#343200'
  primary-container: '#efe811'
  on-primary-container: '#6a6700'
  inverse-primary: '#646100'
  secondary: '#f5fff4'
  on-secondary: '#00391f'
  secondary-container: '#11ffa0'
  on-secondary-container: '#007144'
  tertiary: '#ffffff'
  on-tertiary: '#680012'
  tertiary-container: '#ffdad8'
  on-tertiary-container: '#ca002d'
  error: '#ffb4ab'
  on-error: '#690005'
  error-container: '#93000a'
  on-error-container: '#ffdad6'
  primary-fixed: '#efe811'
  primary-fixed-dim: '#d2cc00'
  on-primary-fixed: '#1e1d00'
  on-primary-fixed-variant: '#4b4900'
  secondary-fixed: '#55ffa9'
  secondary-fixed-dim: '#00e38d'
  on-secondary-fixed: '#002110'
  on-secondary-fixed-variant: '#005230'
  tertiary-fixed: '#ffdad8'
  tertiary-fixed-dim: '#ffb3b2'
  on-tertiary-fixed: '#410008'
  on-tertiary-fixed-variant: '#92001e'
  background: '#131313'
  on-background: '#e5e2e1'
  surface-variant: '#353534'
typography:
  h1:
    fontFamily: Space Grotesk
    fontSize: 64px
    fontWeight: '700'
    lineHeight: '1.1'
    letterSpacing: -0.02em
  h2:
    fontFamily: Space Grotesk
    fontSize: 48px
    fontWeight: '700'
    lineHeight: '1.1'
    letterSpacing: -0.01em
  h3:
    fontFamily: Space Grotesk
    fontSize: 32px
    fontWeight: '600'
    lineHeight: '1.2'
    letterSpacing: 0em
  body-lg:
    fontFamily: Inter
    fontSize: 18px
    fontWeight: '400'
    lineHeight: '1.6'
    letterSpacing: 0em
  body-md:
    fontFamily: Inter
    fontSize: 16px
    fontWeight: '400'
    lineHeight: '1.6'
    letterSpacing: 0em
  mono-label:
    fontFamily: Space Grotesk
    fontSize: 14px
    fontWeight: '500'
    lineHeight: '1.0'
    letterSpacing: 0.1em
  code-data:
    fontFamily: Inter
    fontSize: 13px
    fontWeight: '400'
    lineHeight: '1.4'
    letterSpacing: 0em
spacing:
  unit: 4px
  gutter: 24px
  margin: 64px
  container-max: 1440px
---

## Brand & Style

This design system establishes a high-fidelity, dystopian digital environment translated into a sleek, professional portfolio. It merges **Cyberpunk Brutalism** with **Modern Minimalism**, focusing on technical precision, high-contrast readability, and "glitch-in-the-shell" aesthetics. 

The personality is cold, expert, and unapologetically technical. The UI should feel like a high-end neural interface—utilitarian but punctuated by aggressive neon accents. Key visual drivers include ultra-thin architectural lines, monospaced data readouts, and intentional "digital artifacts" like scanlines and RGB shifts that suggest a live, slightly unstable system.

## Colors

The palette is rooted in absolute darks to create a "void" effect, allowing neon accents to behave like light sources. 

- **Primaries & Surfaces:** Deep Black (#0a0a0a) serves as the base layer, while Dark Gray (#121212) defines structural containers.
- **Accents:** Neon Yellow is the primary action color for high-priority CTAs. Neon Cyan is used for technical data, links, and success states. Neon Magenta is reserved for warnings, errors, and decorative "glitch" highlights.
- **Interaction:** Use high-vibrancy glows (filter: drop-shadow) sparingly to simulate neon tubes. All secondary text should utilize a mid-gray to maintain hierarchy against the intense accents.

## Typography

This design system utilizes a dual-font strategy to balance futuristic character with extreme legibility.

- **Headings:** Space Grotesk provides a geometric, technical feel with "open" apertures that feel cutting-edge. It should be used for all major section headers and hero statements.
- **Body & Data:** Inter is used for long-form content to ensure readability. For a "monospace" feel without sacrificing legibility, Inter is paired with increased letter spacing and strict grid alignment.
- **Styling:** Headings should occasionally use `text-transform: uppercase` or be bracketed (e.g., `[ SECTION_01 ]`) to reinforce the terminal aesthetic.

## Layout & Spacing

The layout follows a **Fixed Grid** system inspired by blueprint schematics. 

- **Grid:** A 12-column grid with generous 24px gutters. Content is strictly aligned to these lines to feel "engineered."
- **Rhythm:** Spacing follows a 4px base unit. Vertical rhythm is aggressive, using large gaps (64px+) between sections to maintain a minimalist, spacious feel.
- **The "Broken" Grid:** Occasionally offset elements by exactly one gutter width or use "hanging" labels in the margins to create a more dynamic, glitch-inspired composition.

## Elevation & Depth

Depth is conveyed through **Tonal Layers** and **Digital Overlays** rather than physical shadows.

- **Stacking:** Surface levels are distinguished by subtle shifts in black-to-gray values. There are no ambient shadows. 
- **Scanning Overlays:** A subtle, fixed-position SVG pattern of horizontal scanlines (1px height, 4% opacity) covers the entire viewport to give the "screen" texture.
- **Borders:** Depth is defined by 1px solid borders in #2a2a2a or primary accent colors. "Active" elements should have a glowing border-bottom or corner-bracket motifs.
- **Transparency:** Use backdrop-blur (10px+) with 80% opacity on navigation bars to simulate a "HUD" (Heads-Up Display) overlaying the content.

## Shapes

The shape language is strictly **Sharp (0px)**. Roundness is non-existent in this design system, reinforcing the aggressive, industrial nature of the theme.

To add visual interest without using curves:
- **Beveled Corners:** Use CSS `clip-path` to create "cut" corners (45-degree angles) on buttons and large cards.
- **Brackets:** Enclose images or important data points in 1px thin bracket lines rather than standard boxes.
- **Notches:** Use small rectangular "cut-outs" in the corners of containers to simulate hardware ports or modular panels.

## Components

- **Buttons:** Rectangular, sharp-edged. The primary state is solid Neon Yellow with black text. Hover state triggers a "glitch" animation (a 2px horizontal jitter) and an RGB split effect.
- **Inputs:** Underlined only (1px solid #2a2a2a). On focus, the line turns Neon Cyan with a subtle outer glow. Label text should be monospaced and sit above the line.
- **Cards:** No background by default; defined by 1px borders. Use a "corner-accent" style where only the top-left and bottom-right corners have colored brackets.
- **Chips/Badges:** Small, uppercase monospaced text inside a thin border. Use Neon Magenta for "Critical" tags and Neon Cyan for "Info" tags.
- **Status Indicators:** Use a blinking 4px square next to titles to simulate a "live" system heartbeat.
- **Data Tables:** Minimalist with no vertical lines. Horizontal lines should be thin and dim (#1a1a1a).
- **Glitch Text:** Apply a CSS animation to titles that occasionally "twitches" the text or shifts the color channels for 100ms.