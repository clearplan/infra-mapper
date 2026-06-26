# Security Policy

ClearPlan InfraMapper is a standalone, client-side HTML application. It has no server component, no backend API, and no telemetry — all data stays in the user's browser (local storage) or in JSON files they explicitly save.

## Reporting a Vulnerability

If you discover a security issue (e.g. an XSS vector in saved-file parsing, an unsafe `eval`-equivalent, or a supply-chain concern with a bundled library), please report it privately rather than opening a public issue.

**Contact:** ryan_o_beard@me.com

Please include:
- A description of the issue and its potential impact
- Steps to reproduce
- The app version (shown in the bottom-left of the nav bar)

We aim to acknowledge reports within 5 business days.

## Scope

- The current release published at https://github.com/clearplan/infra-mapper/releases/latest
- The bundled third-party libraries (Cytoscape.js, cytoscape-fcose, html2canvas, jsPDF) are out of scope for this repo — please report upstream — but we will track and re-bundle security patches.

## Supported Versions

Only the latest released version is supported. Older versions should be upgraded via the in-app **Check for Updates** routine.
