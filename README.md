# Luxury Restaurant Website & QR Menu Studio

A framework-free starter project for a premium restaurant website and browser-based menu editor. Built with HTML, CSS, vanilla JavaScript and JSON; no build step or paid API is required.

## Open the project

**Recommended (Replit):** create/import a Replit project, upload this folder's files preserving the folder structure, then use Replit's static/web preview. The pages use `fetch('data/menu.json')`, so use a local web server/preview rather than opening the HTML as a `file://` URL.

- Customer website: `index.html`
- Editor: `menu-editor.html`

For local development with Python installed, run `python -m http.server 8000` from the project folder and open `http://localhost:8000`.

## Main features

- Responsive editorial restaurant landing page and menu.
- Light, dark and system appearance choices on both pages, saved separately in browser storage.
- Four customer-menu palette presets; custom hex and colour inputs in the editor.
- Restaurant profile, category and item management, live preview, JSON import/export and CSV import.
- Browser-local draft recovery and helpful validation messages.
- Keyboard focus styles, semantic labels, reduced-motion support and responsive layouts.

## Important static-hosting limitation

The editor's browser draft does **not** automatically update `data/menu.json` on the hosted website. Export JSON, replace `data/menu.json` in the project, add image files referenced by project-relative paths, then redeploy/republish. Browser storage is local to that browser/device and is not a shared database.

## Images and licensing

The sample uses remotely hosted Unsplash image URLs for demonstration; remote images require network access and may change. For reliable production use, download/commission properly licensed images and store them in `assets/images/`, then change the image paths. The included SVG is a local fallback placeholder. Do not copy photos from other templates without checking their license.

## Files

See `CUSTOMIZATION.md`, `DEPLOYMENT.md` and `TESTING.md` for detailed instructions and verification scope.
