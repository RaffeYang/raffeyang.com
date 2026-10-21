# Homepage performance implementation plan

**Goal:** Preserve the minimalist homepage while removing avoidable loading and animation work.

**Architecture:** A single HTML document contains all rendering styles and inline artwork. The SVG favicon remains separate. No build tools or runtime dependencies.

**Tech stack:** HTML, CSS, SVG, GitHub Pages.

## Tasks

- [x] Edit `index.html`: put styles inside `head`, remove Google Fonts connections and stylesheet, add a canonical URL, preserve metadata and artwork.
- [x] Replace table positioning with viewport-aware grid centering and a fluid inner width. Preserve 350px maximum content width and 24px monospace text.
- [x] Convert the two Taiji dimension animations to equivalent scale keyframes. Keep original timing and colors. Disable the cursor too in reduced-motion mode.
- [x] Remove obsolete `style.css` after inlining. Update `README.md` with the single-file maintenance and verification workflow.
- [x] Check resource references and 20 combinations of viewport, theme, and reduced motion. No horizontal overflow, clipped logo, active reduced-motion animations, or page errors were detected. Temporary test artifacts were subsequently deleted at the user's request.
- [ ] Recheck appearance with Safari + Safari MCP when available. This is the only permitted browser automation. Lighthouse scoring has not been completed; do not provision Chrome/Chromium.

Production publication is a separate action; source changes alone do not establish a production score.
