
# Copilot Instructions for KMQR-iOS-PWA

## Project Purpose & Architecture
This project is a minimal, iOS-optimized Progressive Web App (PWA) for generating and displaying QR codes. It is intentionally simple: all logic, UI, and PWA features are contained in a single HTML file, with one minified JavaScript dependency for QR code generation.

**Key Files:**
- `index.html`: The only file you need to edit for UI, logic, and PWA features. All code runs client-side.
- `qrcode.min.js`: Minified QR code library, loaded via `<script>` in `index.html`.
- `DEPLOY_INSTRUCTIONS.md`: Manual deployment steps.
- `GITHUB_DESKTOP_STEPS.md`: GitHub Desktop workflow guide.

## Essential Patterns & Conventions
- **Single File App:** All features, UI, and logic are in `index.html`. Do not split code into multiple files or add frameworks.
- **No Build Tools:** There is no build, test, or automation pipeline. All changes are made directly to `index.html` and are live immediately.
- **Direct Library Use:** Use `qrcode.min.js` via `<script>` tag. Do not use npm, yarn, or any bundler.
- **No Backend:** All QR code generation is client-side. No server, API, or external service integration.
- **PWA Support:** If present, manifest and service worker logic are inlined or referenced in `index.html`.
- **iOS First:** Always test and optimize for iOS Safari. Avoid features unsupported on iOS.
- **Minimalism:** Do not add new dependencies, files, or complexity unless absolutely required for QR code PWA functionality.

## Developer Workflow
1. **Edit:** Make all changes in `index.html`.
2. **Test:** Open `index.html` in a browser (preferably Safari on iOS) to verify changes.
3. **Deploy:** Follow `DEPLOY_INSTRUCTIONS.md` for manual deployment.
4. **Version Control:** Use `GITHUB_DESKTOP_STEPS.md` for GitHub Desktop usage.

## Examples
- To add a new feature, edit `index.html` and call functions from `qrcode.min.js`.
- To update the UI, modify the HTML/CSS/JS directly in `index.html`.
- To deploy, follow the manual steps in `DEPLOY_INSTRUCTIONS.md`.

## Integration Points
- Only `qrcode.min.js` is used. No other libraries or services are integrated.
- All PWA logic (manifest, service worker) must be in or referenced from `index.html`.

---
**Summary:**
Keep the project minimal, iOS-focused, and single-file. Edit only `index.html` for all changes. Avoid adding complexity or dependencies. Use `qrcode.min.js` directly. Follow the provided markdown guides for deployment and version control.
