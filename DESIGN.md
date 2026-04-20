# Design System: Architectural Brutalism & Structural Integrity

## 1. Overview & Creative North Star
The Creative North Star for this design system is **"The Monolith."** 

Inspired by the raw, unapologetic strength of architectural brutalism, this system treats digital space like a construction site of premium materials. We are moving away from the "airy" and "rounded" trends of SaaS to embrace something more permanent: heavy weights, sharp 90-degree angles, and massive typographic scales. The design breaks the standard template look by using intentional asymmetry—think of a concrete slab cantilevered over a void. We rely on the raw power of `primary` (Navy) and `secondary` (Bold Red) to create a sense of industrial reliability.

## 2. Colors & Tonal Logic
Our palette is high-contrast and authoritative. We avoid the "safe" pastels of modern UI in favor of deep saturated tones and stark whites.

*   **Primary (#00003c / #000080):** The foundation. Use `primary` for structural elements and `primary_container` for large, immersive blocks of color.
*   **Secondary (#bc0100 / #eb0000):** The "Safety Red." This is used sparingly for high-impact CTAs, critical alerts, and brand accents that demand immediate attention against the navy.
*   **The "No-Line" Rule:** Sectioning is never achieved through 1px borders. We define boundaries through **Mass**. Use a shift from `surface` to `surface_container_low` to create a "poured concrete" effect where one section ends and another begins.
*   **Signature Textures:** For Hero sections and primary CTAs, use a subtle linear gradient transitioning from `primary` (#00003c) to `primary_container` (#000080) at a 45-degree angle. This adds "material soul" to the flat digital plane.

## 3. Typography
The typography is a dialogue between the industrial weight of **Space Grotesk** and the functional clarity of **Work Sans**.

*   **Display & Headlines (Space Grotesk):** These are our "Structural Beams." Use `display-lg` (3.5rem) and `headline-lg` (2rem) with tight letter spacing (-0.02em) to create a dense, powerful visual block. Headings should feel "heavy."
*   **Body & Titles (Work Sans):** These provide the "Blueprint Clarity." `body-lg` (1rem) is the workhorse. It must remain clean, legible, and unadorned to contrast with the aggressive headlines.
*   **Hierarchy Note:** Use all-caps for `label-md` and `label-sm` to reinforce the architectural labeling aesthetic often found on technical drawings.

## 4. Elevation & Depth
In Architectural Brutalism, depth isn't about "floating"—it's about **Stacking and Recessing**.

*   **The Layering Principle:** We use the `surface-container` scale (Lowest to Highest) to represent different planes of a structure. 
    *   `surface_container_lowest`: Background/Base.
    *   `surface_container`: Secondary information blocks.
    *   `surface_container_highest`: Interactive elements or highlighted modules.
*   **Ambient Shadows:** Traditional drop shadows are prohibited. If a lift is required, use a high-spread, low-opacity shadow (4% opacity) tinted with `primary`. This should feel like a soft occlusion shadow in a well-lit room, not a digital effect.
*   **The "Ghost Border":** For interactive states (like a focused input), use the `outline_variant` at 20% opacity. This creates a "blueprint line" that guides the eye without cluttering the "monolithic" feel of the containers.
*   **Glassmorphism:** Reserved exclusively for navigation overlays. Use `surface_variant` with a 12px backdrop-blur and 80% opacity to mimic frosted glass panels over industrial steel.

## 5. Components

*   **Buttons:** 
    *   **Primary:** Sharp 0px corners. Background: `secondary_container` (Red); Text: `on_secondary`. 
    *   **Secondary:** Sharp 0px corners. Background: `primary_container` (Navy); Text: `on_primary`. 
    *   **Padding:** Generous horizontal padding (24px) to emphasize the "block" nature.
*   **Cards:** Forbid divider lines. Separate content using a `surface_container_low` background against a `surface` page. Headlines within cards should be flush with the left edge to maintain a strong vertical axis.
*   **Input Fields:** Use a "Filled" style rather than outlined. Use `surface_container_high` as the field background with a 2px bottom-heavy border in `primary` on focus. No rounded corners (`0px`).
*   **Chips:** Rectangular blocks using `surface_container_highest`. They should look like small bricks of information.
*   **The "Structural Inset" (Special Component):** For testimonials or featured projects, use a `primary` background with an asymmetrical inset image that "breaks" the container's edge.

## 6. Do's and Don'ts

### Do:
*   **Embrace the 0px Radius:** Every element—buttons, cards, inputs—must have a `0px` border radius. Sharp corners imply precision and structural integrity.
*   **Use Massive Scale:** Don't be afraid of huge headlines. In this system, type is a graphic element, not just information.
*   **Intentional Asymmetry:** Align text to a 12-column grid, but allow large imagery to span 7 or 8 columns to create a dynamic, "unbalanced" but stable look.

### Don't:
*   **No Rounded Corners:** Never use `border-radius`. It softens the brand and destroys the "Architectural" feel.
*   **No Thin Dividers:** Avoid using 1px gray lines to separate content. Use whitespace or background color shifts.
*   **No Playful Animations:** Transitions should be "Heavy" and "Mechanical." Use `cubic-bezier(0.2, 0, 0, 1)` for transitions—it mimics the start-stop of heavy machinery.