# Greenhouse Coffee: Project Requirements

## Purpose

Create a polished, responsive website for Greenhouse Coffee, a fictional premium neighborhood coffee house. The site is a professional portfolio showcase and should make the brand and practical visit information clear to first-time guests.

## Audience and primary goals

- Help prospective guests understand the café's atmosphere and point of view.
- Let visitors browse coffee, food, and services.
- Make the café's location, contact details, and opening hours easy to locate.
- Present a coherent, credible brand experience on phones, tablets, and desktop screens.

## Required content and sections

1. **Home / Hero:** Original brand mark, concise welcoming headline and supporting copy, café photography, and a clear path to the menu or visit information.
2. **About Us:** A short, specific introduction to the fictional café, its hospitality, sourcing values, and atmosphere. Avoid generic filler copy.
3. **Coffee and food menu:** Readable, grouped offerings with names and concise descriptions; prices can be added when the fictional menu is established.
4. **Gallery:** A considered set of café, coffee, and food images with meaningful alternative text where images convey content.
5. **Services:** Clearly describe relevant offerings such as dine-in, takeaway, and Wi-Fi; include only services the fictional business actually supports.
6. **Location and contact:** Address, map or map link, and practical contact channels. Use clearly identified fictional portfolio details rather than real private contact information.
7. **Opening hours:** A legible weekly schedule, including any closed days or special notes.

## Functional requirements

- Provide clear navigation to the main sections, including a usable mobile layout.
- Make telephone, email, and map actions clickable when those details are supplied.
- Keep menu, hours, and other repeatable content in simple data modules so updates do not require editing layout markup.
- Ensure keyboard users can navigate links and controls, with visible focus styles and semantic headings/landmarks.
- Respect reduced-motion preferences; animation must remain subtle and must not block access to content.
- Use descriptive image alternatives for meaningful images and empty alternatives for decorative imagery.
- Keep the website informational; do not imply online ordering or reservations unless those functions are deliberately added later.

## Visual and content direction

- **Brand character:** Premium, welcoming, modern, and quietly connected to plants and the greenhouse idea.
- **Palette:** Warm espresso brown, cream or oat, muted leaf green, and a restrained copper or terracotta accent. Define reusable CSS custom properties.
- **Typography:** Pair an expressive, readable display face with a highly legible body face. Prefer a small number of weights and ensure the page remains usable if a web font fails to load.
- **Layout:** Generous spacing, clear hierarchy, balanced image and text regions, and responsive grids that adapt from mobile through desktop.
- **Photography:** Use high-quality, relevant, freely licensed images from Unsplash or Pexels. Record source and applicable license/attribution information with the assets. Optimize image dimensions and formats for the web.
- **Identity:** Create an original SVG Greenhouse Coffee logo; do not reuse another business's mark.
- **Motion:** Use brief, restrained transitions or reveal effects only where they improve feedback or orientation. Avoid requiring animation to understand content.
- **Copy:** Write concise, brand-specific copy. Do not use lorem ipsum or unverified claims about sourcing, sustainability, or services.

## Technical constraints

- Continue using the existing React + Vite project and its current JavaScript/JSX setup.
- Prefer the existing React, Vite, CSS, and Oxlint tooling. Add dependencies only when a concrete requirement cannot be met well with the current stack.
- Keep architecture appropriate for a medium-sized informational site; avoid introducing a routing framework, state library, or component system without a demonstrated need.
- Preserve and update the existing project configuration rather than replacing it wholesale.

## Acceptance criteria

- All seven required content areas are present and reachable through clear navigation.
- The layout works at mobile, tablet, and desktop widths without horizontal overflow or unreadable content.
- Brand colors, typography, image treatment, and spacing feel consistent and intentional.
- Keyboard focus, semantic structure, alternative text, and reduced-motion behavior are considered.
- The original SVG identity and image source/license notes are included in the project assets.
- Setup, development, build, preview, and lint instructions are documented and the project builds successfully.
