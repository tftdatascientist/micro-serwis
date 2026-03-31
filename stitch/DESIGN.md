# Design System Strategy

## 1. Overview & Creative North Star
The Creative North Star for this design system is **"The Precision Architect."** 

In the world of electronics repair, precision is the baseline, but trust is the premium. This system moves away from the "cluttered hardware shop" aesthetic toward a high-end, editorial experience that mirrors the internal sophistication of the devices being repaired. By utilizing intentional asymmetry, expansive negative space, and a technical typographic scale, we position the brand as an elite laboratory rather than a basic workshop. We break the "template" look by overlapping structural elements and using tonal shifts instead of rigid grid lines to define the user journey.

## 2. Colors
The color strategy utilizes a spectrum of technical blues and sterile whites to evoke cleanliness, diagnostic accuracy, and modern tech-savviness.

*   **Primary (#006097) & Primary Container (#007abe):** These represent the "Action Layer." Use these for core navigation and critical touchpoints. 
*   **Surface Hierarchy & Nesting:** We treat the interface as a physical stack of components. To create depth, use the hierarchy of surface tokens:
    *   **Background (#f9f9f9):** The base canvas.
    *   **Surface Container Low (#f3f3f3):** Used for large structural sections (e.g., a "Services" area).
    *   **Surface Container Lowest (#ffffff):** Used for foreground cards or interactive modules sitting atop a "Low" section.
*   **The "No-Line" Rule:** 1px solid borders are strictly prohibited for sectioning. Boundaries must be defined solely through background color shifts. If a section ends, the background transitions from `surface` to `surface-container-low`.
*   **The "Glass & Gradient" Rule:** To provide "visual soul," use subtle gradients on primary CTAs (transitioning from `primary` to `primary-container`). For floating navigation or modal overlays, apply a backdrop-blur (16px–32px) with a semi-transparent `surface` color to achieve a frosted glass effect that feels premium and modern.

## 3. Typography
The typography system balances the technical rigidity of **Space Grotesk** with the humanist clarity of **Inter**.

*   **Display & Headlines (Space Grotesk):** These are the "Diagnostic" levels. The wide apertures and geometric shapes of Space Grotesk convey a tech-forward authority. Use `display-lg` (3.5rem) for hero statements to create an editorial, high-impact entry point.
*   **Titles & Body (Inter):** These are the "Communication" levels. Inter provides maximum legibility for service descriptions and technical specifications. 
*   **Hierarchy as Identity:** By pairing a massive `display-md` headline with a significantly smaller `body-lg` description, we create a high-contrast visual rhythm that feels more like a premium tech journal than a standard website.

## 4. Elevation & Depth
In this design system, depth is a functional tool, not a decoration. We achieve hierarchy through **Tonal Layering** rather than traditional drop shadows.

*   **The Layering Principle:** Stacking `surface-container-lowest` (#ffffff) on top of `surface-container-low` (#f3f3f3) creates a natural, soft lift. This mimics the way a motherboard sits within a chassis—integrated but distinct.
*   **Ambient Shadows:** Where floating elements (like a "Repair Status" popover) are required, shadows must be extra-diffused. Use the `on-surface` color at 6% opacity with a blur radius of 40px and a Y-offset of 12px. This creates a soft glow rather than a harsh edge.
*   **The "Ghost Border" Fallback:** If accessibility requires a container edge, use a "Ghost Border": the `outline-variant` token at 15% opacity. Never use 100% opaque borders.
*   **Glassmorphism:** For hero cards or interactive tech specs, use a semi-transparent surface color with a `backdrop-filter: blur(20px)`. This allows the brand's blues and grays to bleed through, softening the interface and making it feel like a high-end diagnostic tool.

## 5. Components

*   **Buttons:**
    *   **Primary:** A gradient from `primary` to `primary-container`. Use `xl` (0.75rem) roundedness. No border.
    *   **Secondary:** `surface-container-high` background with `on-surface` text. This feels "embedded" into the page.
*   **Cards:** Forbid divider lines. Separate content using `spacing-8` (2rem) of vertical white space or by nesting a `surface-container-lowest` card inside a `surface-container-low` wrapper.
*   **Input Fields:** Use the `surface-container-highest` (#e2e2e2) for the field background with a "Ghost Border." On focus, transition the border to `primary` at 100% opacity.
*   **Chips:** Use `lg` (0.5rem) roundedness. For repair status (e.g., "In Progress"), use `secondary-container` with `on-secondary-container` text.
*   **Repair Timeline (Custom Component):** A vertical sequence of cards where the active state is highlighted with a `primary` glassmorphism glow. Do not use a central line; use the shift in surface color to guide the eye.
*   **Checkboxes & Radios:** Use `md` (0.375rem) roundedness. Avoid the standard circular radio; use a subtle "inner-glow" effect using the `primary-fixed-dim` token when selected.

## 6. Do's and Don'ts

### Do:
*   **Do** use intentional asymmetry. Place a headline on the far left and a supporting image slightly offset to the right to create dynamic energy.
*   **Do** use the Spacing Scale religiously. Consistent gaps (e.g., `spacing-12` between major sections) are what make a design feel professional.
*   **Do** lean into "Tech-Glass." Use blurred overlays for mobile menus to maintain the sense of depth.

### Don't:
*   **Don't** use 1px solid black or dark grey borders. It breaks the "Precision Architect" illusion and looks dated.
*   **Don't** use standard "drop shadows." If it looks like a "box shadow" from 2010, it's too heavy.
*   **Don't** crowd the interface. If a customer is looking for a repair service, give the information room to breathe. High-end service is never rushed; the UI shouldn't be either.
*   **Don't** use icons without purpose. Every icon should feel like a technical schematic—thin lines, consistent 2px stroke, and matching the `outline` token color.