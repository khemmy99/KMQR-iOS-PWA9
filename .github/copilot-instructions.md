# Copilot Instructions for KMQR-iOS-PWA

## Project Overview
This project is a minimal iOS-focused Progressive Web App (PWA) for QR code generation and display. It is designed for simple deployment and use on iOS devices, leveraging a single HTML entry point and a minified JavaScript QR code library.

## Key Files
- `index.html`: Main entry point. Contains all UI and logic for the PWA.
- `qrcode.min.js`: Minified QR code generation library. Used directly in the HTML.
- `DEPLOY_INSTRUCTIONS.md`: Steps for deploying the PWA.
- `GITHUB_DESKTOP_STEPS.md`: Steps for using GitHub Desktop with this project.

## Architecture & Patterns
- **Single Page App**: All logic and UI are in `index.html`. No frameworks or build tools are used.
- **Direct Script Usage**: `qrcode.min.js` is loaded via a `<script>` tag. No npm/yarn or module bundlers.
- **No Backend**: All QR code generation is client-side. No server or API integration.
- **PWA Features**: If present, PWA logic (manifest, service worker) will be inlined or referenced in `index.html`.

## Developer Workflows
- **Edit and Test**: Open `index.html` directly in a browser (preferably Safari on iOS for best results).
- **Deploy**: Follow `DEPLOY_INSTRUCTIONS.md` for publishing updates.
- **Version Control**: Use `GITHUB_DESKTOP_STEPS.md` for GitHub Desktop workflows.
- **No Build Step**: There is no build or test automation. All changes are manual and visible immediately.

## Conventions
- **Keep It Simple**: Avoid adding dependencies, build tools, or frameworks unless absolutely necessary.
- **Minimize File Count**: Prefer editing `index.html` for UI/logic changes.
- **Direct Library Use**: Use minified libraries via `<script>` tags, not package managers.
- **Mobile-First**: Prioritize iOS/Safari compatibility in all changes.

## Examples
- To add a new feature, edit `index.html` and use functions from `qrcode.min.js`.
- To update deployment, follow the steps in `DEPLOY_INSTRUCTIONS.md`.

## External Dependencies
- Only `qrcode.min.js` is used. No other external libraries or services are integrated.

---
For any changes, keep the project minimal and focused on iOS PWA QR code generation.
