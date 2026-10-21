# Testing record

## Environment and scope

This deliverable was assembled as a static HTML/CSS/JavaScript project. The authoring environment did not provide a connected Replit workspace or browser automation session, so Replit deployment, rendered visual appearance, real device widths and browser-console behavior cannot be claimed as verified here.

## Fixes applied in the follow-up build

- Separated editor appearance tokens from restaurant palette tokens so the brand palette no longer overrides the editor light/dark/system surfaces.
- Set the effective appearance in the document head to reduce the initial wrong-theme flash.
- Added a compatibility fallback for system-theme change events in browsers that do not support `MediaQueryList.addEventListener`.
- Static-hosting limitation remains: editing in the browser does not publish to all visitors.

## Automated checks run during packaging

- JSON syntax parsing: run locally before packaging.
- JavaScript syntax checks: run with Node.js where available.
- HTML/CSS/JS file existence and relative-path review.

## Manual acceptance checklist for Replit

- [ ] Both `index.html` and `menu-editor.html` load through the preview server.
- [ ] Light/dark/system appearance updates each page and persists after reload.
- [ ] System mode follows an operating-system appearance change.
- [ ] Customer menu renders profile, categories, visible/available dishes and prices from `data/menu.json`.
- [ ] Presets and hex/colour inputs synchronize; malformed hex values are rejected.
- [ ] Restaurant profile changes update the editor preview.
- [ ] Category add, rename, reorder, show/hide and guarded delete work.
- [ ] Item add, edit, duplicate, reorder, show/hide, search/filter and delete work.
- [ ] JSON export then import preserves supported profile, theme, category and item data.
- [ ] CSV import validates required fields and adds rows.
- [ ] Browser draft restores after refresh; draft is local to that browser.
- [ ] Missing remote images fall back to the included SVG.
- [ ] At widths 320, 375, 430, 768, 1024 and desktop, inspect horizontal overflow and touch controls.
- [ ] Verify focus rings, labels, contrast, and reduced-motion behavior in both appearances.
- [ ] After replacing `data/menu.json` and redeploying, the public page reflects the exported data.

## Known limitations / items requiring verification

- No server-side persistence, multi-user accounts, image uploads, reservation submission or automatic publish action is included.
- Local image selection is explicitly temporary; it does not upload or export image bytes.
- External Unsplash images and Google Fonts need internet access. Replace with properly licensed local assets for production reliability.
- The customer menu theme and appearance modes need final browser QA, especially for combinations of custom palettes and dark appearance.
- A category cannot be deleted while it contains menu items; move/delete those items first.
