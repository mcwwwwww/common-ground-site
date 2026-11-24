# Common Ground website (common-ground.agency)

Single-page marketing site for Common Ground (Rob Lewis & Petronella).

## How publishing works
- Every push to the `main` branch on GitHub goes live on https://www.common-ground.agency within about a minute (Vercel auto-deploy).
- No build step. What is in this folder is what is served.
- After making changes: commit with a short plain-English message and push to `main`.

## Files
- `index.html` is the whole site. It is a "Design Component" file: markup lives between `<x-dc>` and `</x-dc>`, styling is inline on each element, and a small `class Component extends DCLogic` script at the bottom handles the nav, mobile menu and scroll animations.
- `support.js` is the runtime that renders `index.html`. Do not edit or delete it.
- `assets/` holds images. Keep images under about 1 MB (resize to max 1600px wide).
- `favicon.png` is the browser tab icon.

## Rules
- Before pushing, open `index.html` in a browser and check the change looks right on desktop and phone width.
- Keep the mint/teal palette and the two fonts (Schibsted Grotesk headings, Hanken Grotesk body).
- The contact form posts to Formspree (`action="https://formspree.io/f/..."`). Only change the ID if asked.
- Never commit passwords or API keys.
