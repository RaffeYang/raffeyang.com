# Minimal homepage performance

Approved direction: preserve the existing Taiji, contact text, Buddha illustration,
light/dark themes, and animation. Keep the site framework-free and JavaScript-free.

Remove unused Google Fonts and inline the small stylesheet in the document head
so rendering needs no secondary resource. Keep the favicon as a separate SVG.
Replace animated dimensions with transforms, preserve the morphing timing, and
disable every animation when reduced motion is requested. Allow the centered
content to fit narrow and short viewports without clipping or horizontal overflow.

Validate resource requests, appearance, responsive layout, themes, reduced motion,
and Lighthouse where a browser is available. Local scores are not production
scores; production must be measured after deployment. Do not promise a fixed
score independent of hosting latency and test conditions.
