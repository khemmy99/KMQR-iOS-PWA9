


# Copilot Instructions for KMQR-iOS-PWA

## Project Architecture & Key Files
- **Single-file PWA:** All app logic, UI, and PWA features are in `index.html`. This includes HTML, CSS, JavaScript, manifest, and (if present) service worker logic.
- **External dependency:** Only `qrcode.min.js` is used, loaded via a `<script>` tag in `index.html` for QR code generation.
- **No backend:** All QR code generation and display is client-side. No server or API integration.
- **Supporting docs:**
	- `DEPLOY_INSTRUCTIONS.md`: Manual deployment steps.
	- `GITHUB_DESKTOP_STEPS.md`: GitHub Desktop workflow guide.

## Essential Patterns & Conventions
- **Edit only `index.html`:** All features, UI, and logic changes must be made in `index.html`. Do not split code into multiple files or add frameworks.
- **No build or automation:** There is no build, test, or automation pipeline. Changes are live immediately after editing `index.html`.
- **Direct library use:** Use `qrcode.min.js` directly. Do not use npm, yarn, or any bundler.
- **Minimalism:** Do not add new dependencies, files, or complexity unless absolutely required for core QR code PWA functionality.
- **iOS-first:** Always test and optimize for iOS Safari. Avoid features unsupported on iOS (e.g., some Web APIs, file system access).

## Developer Workflow
1. **Edit:** Make all changes in `index.html`.
2. **Test:** Open `index.html` in a browser (preferably Safari on iOS) to verify changes.
3. **Deploy:** Follow `DEPLOY_INSTRUCTIONS.md` for manual deployment.
4. **Version Control:** Use `GITHUB_DESKTOP_STEPS.md` for GitHub Desktop usage.

## Project-Specific Examples
- To add a feature, edit `index.html` and call functions from `qrcode.min.js` directly.
- To update the UI, modify HTML/CSS/JS in `index.html`.
- To add or update PWA features (manifest, service worker), do so in `index.html`.
- To deploy, follow the manual steps in `DEPLOY_INSTRUCTIONS.md`.

## Integration Points
- Only `qrcode.min.js` is used. No other libraries or services are integrated.
- All PWA logic (manifest, service worker) must be in or referenced from `index.html`.

---
**Summary:**
Keep the project minimal, iOS-focused, and single-file. Edit only `index.html` for all changes. Avoid adding complexity or dependencies. Use `qrcode.min.js` directly. Follow the provided markdown guides for deployment and version control.
