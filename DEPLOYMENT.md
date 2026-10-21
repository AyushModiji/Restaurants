# Publishing and updating

## Initial publish on Replit

1. Create a static website project in Replit or upload this project's complete folder structure.
2. Make sure `index.html`, `menu-editor.html`, `data/menu.json`, and `assets/` are at the project root/paths shown here.
3. Open the Replit web preview. If a page is opened directly as a local `file://` URL, fetching JSON may fail; use the preview/web server.
4. Test `index.html` and `menu-editor.html` using the preview URL.
5. Use Replit's publishing/deployment flow for your account and confirm the deployed URL yourself. This project does not deploy automatically.

## Publish menu changes

1. Open `menu-editor.html` in the running project.
2. Make changes and choose **Export JSON**.
3. Replace the project's `data/menu.json` with the exported file.
4. Add any new images to `assets/images/` and ensure their paths match the JSON.
5. Redeploy/republish through Replit.
6. Open the published customer page and check names, prices, photos, category navigation, theme and mobile layout.

The editor's local draft is not the published source. Browser storage cannot overwrite a deployed project file, and this project does not include authentication, cloud synchronization, a database or an automated deployment API. Never treat an export or button click as a deployment confirmation.
