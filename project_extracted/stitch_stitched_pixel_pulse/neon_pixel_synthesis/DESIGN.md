---
name: Neon Pixel Synthesis
colors:
  surface: '#131318'
  surface-dim: '#131318'
  surface-bright: '#39383e'
  surface-container-lowest: '#0e0e13'
  surface-container-low: '#1b1b20'
  surface-container: '#1f1f24'
  surface-container-high: '#2a292f'
  surface-container-highest: '#35343a'
  on-surface: '#e4e1e9'
  on-surface-variant: '#ccc3da'
  inverse-surface: '#e4e1e9'
  inverse-on-surface: '#303035'
  outline: '#958da3'
  outline-variant: '#4a4457'
  surface-tint: '#d1bcff'
  primary: '#d1bcff'
  on-primary: '#3c0090'
  primary-container: '#7000ff'
  on-primary-container: '#ddcdff'
  inverse-primary: '#7212ff'
  secondary: '#d3fbff'
  on-secondary: '#00363a'
  secondary-container: '#00eefc'
  on-secondary-container: '#00686f'
  tertiary: '#ffade1'
  on-tertiary: '#5f004e'
  tertiary-container: '#ac008e'
  on-tertiary-container: '#ffc4e7'
  error: '#ffb4ab'
  on-error: '#690005'
  error-container: '#93000a'
  on-error-container: '#ffdad6'
  primary-fixed: '#e9ddff'
  primary-fixed-dim: '#d1bcff'
  on-primary-fixed: '#23005b'
  on-primary-fixed-variant: '#5700c9'
  secondary-fixed: '#7df4ff'
  secondary-fixed-dim: '#00dbe9'
  on-secondary-fixed: '#002022'
  on-secondary-fixed-variant: '#004f54'
  tertiary-fixed: '#ffd8ed'
  tertiary-fixed-dim: '#ffade1'
  on-tertiary-fixed: '#3b002f'
  on-tertiary-fixed-variant: '#86006f'
  background: '#131318'
  on-background: '#e4e1e9'
  surface-variant: '#35343a'
typography:
  display-lg:
    fontFamily: Hanken Grotesk
    fontSize: 48px
    fontWeight: '800'
    lineHeight: '1.1'
    letterSpacing: -0.02em
  display-lg-mobile:
    fontFamily: Hanken Grotesk
    fontSize: 36px
    fontWeight: '800'
    lineHeight: '1.1'
  headline-md:
    fontFamily: Hanken Grotesk
    fontSize: 24px
    fontWeight: '600'
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
    letterSpacing: 0.05em
rounded:
  sm: 0.125rem
  DEFAULT: 0.25rem
  md: 0.375rem
  lg: 0.5rem
  xl: 0.75rem
  full: 9999px
spacing:
  base: 8px
  container-padding: 24px
  gutter: 16px
  trail-width: 2px
---

## Brand & Style

This design system establishes a high-fidelity bridge between nostalgic pixel art and cutting-edge interface design. The brand personality is immersive and energetic, utilizing a **Retro / Vaporwave** aesthetic filtered through a **Modern Minimalist** lens. 

The UI is designed to disappear where necessary to highlight the pixel-based content, yet provides high-contrast, tactile feedback when interacted with. The emotional response should be one of "digital craftsmanship"—where the organic flow of "noise waves" meets the rigid, mathematical precision of modern typography. The style leverages deep dark textures to provide a canvas for vibrant, glowing elements that represent data trails and user movement.

## Colors

The palette is anchored by a "Void Black" textured neutral that prevents the vibrant accents from causing eye fatigue. 

- **Primary (Deep Purple):** Used for structural elements, primary branding, and depth-heavy containers.
- **Secondary (Electric Cyan):** Used for "Noise Waves," active states, and successful interactions. It represents flow and connectivity.
- **Tertiary (Neon Pink):** Reserved for "Trails," highlights, and high-priority call-to-actions.
- **Functional Colors:** Error states utilize a high-saturation red (#FF3B3B), while warnings use a vivid amber (#FFD600), both treated with the same glow-intensity as the core palette.

Backgrounds should utilize a subtle noise texture (3-5% opacity) overlaid on the neutral base to mimic the tactile feel of high-definition pixel canvases.

## Typography

To contrast the blocky nature of pixel art, the design system utilizes **Hanken Grotesk** for its sharp, contemporary, and highly legible characteristics. This sans-serif provides a professional "tech" feel that anchors the more whimsical pixel elements.

For technical metadata and small UI labels, **JetBrains Mono** is introduced. This monospaced font reinforces the "stitched" and "coded" nature of the application, providing a structural counterpoint to the fluid headlines. All typography should maintain high contrast against the dark background, primarily using off-white (#F5F5F7) for body text and full-white (#FFFFFF) for headlines.

## Layout & Spacing

The layout operates on a **Fluid Grid** system that prioritizes organic movement. While the underlying structure is an 8px-based grid, the spacing between sections should feel "breathable" and asymmetrical to reflect the nature of pixel art composition.

- **Desktop:** 12-column grid with wide 32px gutters to allow the dark background texture to show through.
- **Mobile:** 4-column grid with 16px margins.
- **Organic Spacing:** Components should utilize "safe areas" that allow for overlapping "noise wave" decorations without obscuring critical text. Use fluid padding (e.g., `clamp`) to ensure the UI feels expansive on larger high-definition displays.

## Elevation & Depth

Depth is conveyed through **Glassmorphism** and **Tonal Layering** rather than traditional shadows. 

1. **Surface Layers:** The base level is the textured "Void Black."
2. **Interactive Layers:** Cards and panels use a semi-transparent blur (Backdrop Filter: 12px) with a subtle 1px inner border in a low-opacity Primary or Secondary color.
3. **Glow States:** Instead of drop shadows, active elements emit a "Neon Bloom"—a soft, colored outer glow (`box-shadow`) matching the element's primary accent color. This simulates light reflecting off the dark, textured surface.
4. **Trails:** Floating elements leave 2px trails (lines) that connect back to their origin point, visually "stitching" the UI together.

## Shapes

The shape language is **Soft (0.25rem)**. This subtle rounding provides a necessary modern touch that distinguishes the UI controls from the raw, square pixels of the artwork. 

- **Containers:** Large panels use `rounded-lg` (0.5rem) to feel like modern hardware displays.
- **Interactive Elements:** Buttons and inputs use the base 0.25rem radius to maintain a crisp, efficient look.
- **Pixel-Alignment:** Despite the rounding, all element dimensions should snap to the 8px base grid to ensure the layout remains cohesive with the pixel-art content.

## Components

- **Buttons:** High-contrast blocks with a solid Primary background. On hover, they should trigger a Tertiary "glow" and a subtle scaling effect. Use the label font for button text to emphasize the technical nature.
- **Chips/Tags:** Monospaced text inside a Secondary-colored outline with a light 10% fill. These represent the "stitches" in the data.
- **Input Fields:** Flat, dark backgrounds with a 1px Secondary border that "pulses" (changes opacity) when focused. 
- **Cards:** Glassmorphic containers with a backdrop blur. Top-right corners may feature a "pixel-bracket" icon to reinforce the theme.
- **Noise Waves:** Decorative background elements that animate slowly. They should be non-interactive and sit at the lowest z-index above the background texture.
- **Lists:** Clean, borderless rows separated by a 1px faint Primary line. Interactive rows should highlight with a cyan left-border "trail" on hover.