# raffeyang.com
https://raffeyang.com
The Tao gives birth to one, one to two, two to three, and three to all things

## Maintenance

The homepage is a single `index.html` containing its styles and SVG artwork.
It uses system monospace fonts, no JavaScript, and no third-party resources.
Edit the inline `<style>` directly; no build or dependency installation is needed.
The favicon is `favicon.svg`. Light/dark mode follows the system theme, and
reduced motion disables all animations, including the cursor.

Preview with `python3 -m http.server 8000`, then open `http://localhost:8000`.
Use Safari + Safari MCP for browser automation. Check narrow screens,
light/dark themes, and reduced motion. Do not use Chrome/Chromium automation.
Production performance must be checked after deployment; source checks and
local measurements alone do not establish a deployed Lighthouse score.

GitHub Pages deploys pushes to `main` using `.github/workflows/static.yml`.

## LICENSE
[LICENSE](LICENSE)
