

# Copilot Instructions for KMQR-iOS-PWA

## Project Overview & Architecture
This project is a minimal, iOS-first Progressive Web App (PWA) for generating and displaying QR codes. All logic, UI, and PWA features are contained in a single file: `index.html`. The only external dependency is the minified `qrcode.min.js` library, loaded via a `<script>` tag.

**Key Files:**
- `index.html`: All app logic, UI, and PWA features. Edit this file for any change.
- `qrcode.min.js`: Minified QR code generator, loaded directly in the HTML.
- `DEPLOY_INSTRUCTIONS.md`: Manual deployment steps.
- `GITHUB_DESKTOP_STEPS.md`: GitHub Desktop workflow guide.

## Essential Patterns & Conventions
- **Single File App:** All code (HTML, CSS, JS, manifest, service worker) is in or referenced from `index.html`. Do not split code into multiple files or add frameworks.
- **No Build/Automation:** There is no build, test, or automation pipeline. All changes are made directly to `index.html` and are live immediately.
- **Direct Library Use:** Use `qrcode.min.js` via `<script>`. Do not use npm, yarn, or any bundler.
- **No Backend:** All QR code generation is client-side. No server, API, or external service integration.
- **PWA Support:** Manifest and service worker logic (if present) are inlined or referenced in `index.html`.
- **iOS First:** Always test and optimize for iOS Safari. Avoid features unsupported on iOS (e.g., some Web APIs, file system access).
- **Minimalism:** Do not add new dependencies, files, or complexity unless absolutely required for QR code PWA functionality.

## Developer Workflow
1. **Edit:** Make all changes in `index.html`.
2. **Test:** Open `index.html` in a browser (preferably Safari on iOS) to verify changes.
3. **Deploy:** Follow `DEPLOY_INSTRUCTIONS.md` for manual deployment.
4. **Version Control:** Use `GITHUB_DESKTOP_STEPS.md` for GitHub Desktop usage.

## Project-Specific Examples
- To add a new feature, edit `index.html` and call functions from `qrcode.min.js` directly.
- To update the UI, modify the HTML/CSS/JS in `index.html`.
- To add or update PWA features (manifest, service worker), do so in `index.html`.
- To deploy, follow the manual steps in `DEPLOY_INSTRUCTIONS.md`.

## Integration Points
- Only `qrcode.min.js` is used. No other libraries or services are integrated.
- All PWA logic (manifest, service worker) must be in or referenced from `index.html`.

---
**Summary:**
Keep the project minimal, iOS-focused, and single-file. Edit only `index.html` for all changes. Avoid adding complexity or dependencies. Use `qrcode.min.js` directly. Follow the provided markdown guides for deployment and version control.
