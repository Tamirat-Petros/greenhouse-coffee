# Greenhouse Coffee: Project Plan

## Current project assessment

- The repository contains a Vite 8 and React 19 JavaScript starter, with `src/App.jsx`, `src/main.jsx`, `src/App.css`, `src/index.css`, and starter assets.
- `package.json` already provides `dev`, `build`, `preview`, and `lint` scripts. React, React DOM, Vite, the React Vite plugin, and Oxlint are installed.
- The current `App.jsx` and styles render the Vite starter counter and documentation links; none of the Greenhouse Coffee sections exist yet.
- `index.html` still has starter title/favicon references. `public/favicon.svg` and `public/icons.svg` are present starter assets; replace the favicon with original brand artwork when creating the identity. The starter markup references `/icons.svg`, which is not needed for the planned café page.
- Baseline `npm run build` and `npm run lint` both succeed. No `AGENTS.md` was found in the project tree.
- Git has no commits yet. The working tree is untracked, so the starter files and planning documents have not been committed.

## Proposed architecture

Keep a single-page React application and organize around reusable site components and clear content sections. Create these folders as implementation needs arise; do not add empty structure before it is useful.

```text
src/
  assets/                 # Local photography, textures, and original SVG brand mark
  components/             # Shared UI: Header, Footer, Button, SectionHeading
  data/                   # Menu, opening hours, services, and gallery metadata
  sections/               # Hero, About, Menu, Gallery, Services, Visit/Contact
  styles/                 # Design tokens and optional shared styles
  utils/                  # Small pure helpers only when repeated behavior needs them
  App.jsx                 # Page composition and top-level layout
  App.css                 # Page-level composition styles (or split as section styles grow)
  index.css               # Global reset, typography defaults, and global tokens/imports
  main.jsx                # React entry point
public/
  favicon.svg             # Original small-format brand icon, if useful
```

The structure deliberately avoids a `pages/` router because the planned site is one informational page. Shared navigation and footer belong in `components/`; distinct content areas belong in `sections/`; repeatable content belongs in `data/`. Keep CSS beside the app initially, extracting shared styles only as the site grows.

## Milestones

### 1. Foundation and brand shell

- Replace starter page content and browser metadata with Greenhouse Coffee identity.
- Draw an original SVG logo and favicon from the same visual idea.
- Establish color, type, spacing, and responsive layout tokens.
- Build the header/navigation and hero section with licensed photography.

### 2. Informational sections

- Add About, menu, gallery, and services sections.
- Move repeated menu and service content into focused data modules.
- Add accessible image descriptions and record image sources/license notes.

### 3. Visit details and responsive polish

- Add location, contact actions, and opening hours.
- Refine mobile navigation and responsive spacing/grid behavior.
- Add subtle interaction states and reduced-motion handling.

### 4. Final review

- Review page hierarchy, keyboard navigation, focus visibility, image loading, and responsive behavior.
- Run the existing lint and production build scripts; fix any issues.
- Update README project status and usage notes to reflect the finished site.

## Decisions and dependencies

- Retain the current React + Vite JavaScript toolchain and npm scripts; this already covers development, production builds, preview, and linting.
- Use plain CSS and browser-native links/interactions for the first version. This keeps the implementation beginner-friendly and avoids dependencies for a mostly static brochure site.
- Do not add a router, animation library, icon package, or CSS framework unless later requirements justify one.
- Source Unsplash/Pexels images with suitable free-use terms; save asset provenance alongside the downloaded assets or in a small attribution note.

## Git checkpoint

There is currently no commit history and no tracked baseline: the starter project is all untracked. A docs-only commit would leave the initial application files outside that checkpoint. Decide on a first repository commit that includes the initialized starter and these planning documents together, after reviewing the complete staged file list.
