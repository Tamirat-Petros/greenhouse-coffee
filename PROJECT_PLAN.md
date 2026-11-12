# Greenhouse Coffee: Project Plan

## Implementation status

- The responsive single-page café site is implemented in React 19 and Vite 8. It includes hero, story, menu, services, gallery, visit details, opening hours, and footer.
- `src/App.jsx` composes reusable brand, navigation, smoke-decoration, and section-intro components. Menu and service content are stored in small data arrays.
- `src/App.css` contains section and responsive layout styles; `src/index.css` contains global palette, typography, focus, and reduced-motion rules.
- Original coffee, leaf, and smoke branding is drawn as SVG; the matching favicon is `public/favicon.svg`.
- Photography is sourced from Unsplash image URLs. Contact and location details are explicitly identified as fictional portfolio information.
- Existing npm scripts and dependencies were retained. Build and lint checks pass.

## Final architecture

```text
src/
  App.jsx          # Page composition, data, and small reusable UI components
  App.css          # Section styling and mobile/tablet breakpoints
  index.css        # Global design tokens, typography, focus, reduced motion
  main.jsx         # React entry point
  assets/          # Existing Vite starter images (unused by the café page)
public/
  favicon.svg      # Original coffee, leaf, and smoke mark
  icons.svg        # Unused Vite starter sprite
```

For this medium-sized static site, keeping the cohesive page components and content arrays in one JSX module avoids scattering closely related content across many tiny files. Extract them into `components/`, `sections/`, and `data/` if the site grows or content is maintained independently.

## Milestones

1. **Foundation and brand shell — complete:** Replaced starter metadata; established palette, typography, responsive shell, original SVG identity, favicon, and hero.
2. **Informational sections — complete:** Added About, menu with fictional ETB prices, services, and photo gallery.
3. **Visit details and responsive polish — complete:** Added fictional Addis Ababa address/contact, hours, map presentation, mobile navigation, focus states, and reduced-motion support.
4. **Final review — complete:** `npm run build` and `npm run lint` pass. The UI implementation has focused local commits and has not been pushed.

## Decisions and dependencies

- Retain React, Vite, JSX, and plain CSS; no extra dependencies are needed for this informational site.
- Use browser-native links for email, telephone, map directions, and section navigation.
- Use restrained smoke line art as original SVG decoration, without animation that could distract from reading.
- Remote Unsplash photography uses the image service's stable photo IDs and browser-side size/quality parameters. Images load lazily below the hero.
