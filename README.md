# Model Watcher (Brave/Chrome extension)

What it does
- Watches page network calls (fetch/XHR) and extracts `display_model` and `user_selected_model` from JSON responses.
- Shows a small draggable/minimizable overlay in the page with display and user-selected values and a colored status chip.
- Badge: OK (green) when display == user-selected; ! (red) otherwise.

Install (Brave/Chrome)
1) Open brave://extensions (or chrome://extensions)
2) Enable "Developer mode"
3) Click "Load unpacked" and select this folder

Configure
- Options page lets you toggle the in‑page overlay.

Permissions
- Minimal: `storage`, `tabs`. Host access is restricted to `https://*.perplexity.ai/*`.

Build/Package
- Zip for store upload: zip the contents of this folder (all files inside `model-watcher/`).
- For development, use “Load unpacked” with this folder.

Privacy
- See PRIVACY.md. No data is collected or sent anywhere; everything runs locally.

License
- MIT (see LICENSE).
