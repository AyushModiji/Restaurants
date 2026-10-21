# Customization guide

## Edit the restaurant profile

Open `menu-editor.html` in the project's web preview. Change restaurant name, tagline, description, address, phone, opening hours, currency and cover image. The page preview updates as you edit.

## Appearance vs. restaurant palette

The **Appearance** selector controls the editor's interface appearance (light/dark/system). The **Design preset** controls the restaurant's menu palette. These are separate preferences. The customer page also has its own appearance selector.

Available menu presets: Ivory & Forest, Midnight Luxe, Terracotta and Modern Minimal. Select a preset, then adjust individual colour values. Hex fields accept six-digit values such as `#234A3D`.

## Categories and items

- Add a category, rename it, reorder it, hide it from customers, or delete it when it has no items.
- Add/edit/duplicate/reorder/hide/delete dishes. Required item fields are name, non-negative price and category.
- The item search and category filter only change the editor list, not published content.
- Availability and visibility are separate: unavailable or hidden dishes do not appear on the customer page.

## Images

Enter a stable image URL or a project-relative path such as `assets/images/pumpkin-risotto.jpg`. Choosing a local image in the dialog makes a temporary browser preview possible; it does not upload the file or embed it in the exported JSON. To publish an image, add it to `assets/images/` in the project and update the item's path.

## Drafts and exports

Drafts use browser `localStorage` and do not sync between devices or browsers. Export JSON to create a portable snapshot. CSV imports add items rather than replacing existing ones; expected headers are shown in `data/example-menu.csv`.
