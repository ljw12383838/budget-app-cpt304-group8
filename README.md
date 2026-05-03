# Budget App - CPT304 Enhanced Version

[![codecov](https://codecov.io/gh/YOUR-GITHUB-USERNAME/YOUR-REPO-NAME/branch/main/graph/badge.svg)](https://codecov.io/gh/YOUR-GITHUB-USERNAME/YOUR-REPO-NAME)

This is an enhanced version of the Personal Budget App for CPT304 Coursework 1: Research-Led Software Enhancement.

## Main Improvements

- Security: replaced unsafe HTML string rendering with DOM APIs and `textContent` to reduce XSS risk.
- Logic quality: added strict validation for title length, positive numeric amounts, maximum amount and two-decimal precision.
- Accessibility: rebuilt interactive controls with semantic buttons, form labels, ARIA tabs, status messages and visible keyboard focus.
- Internationalisation: added a working English/Chinese language toggle.
- Legal/privacy: added localStorage consent banner, privacy policy dialog and clear-data control.
- Testing: added Vitest coverage for the core maintainable modules: model, validation, storage, i18n and chart rendering.

## Run Locally

```bash
npm install
npm run start
```

Open the local URL printed by Vite, usually `http://localhost:5173`.

## Test and Coverage

```bash
npm test
npm run coverage
```

Current verified local result:

```text
Test Files  1 passed
Tests       17 passed
All files   89.81% statements, 86.76% branches, 86.66% functions, 95% lines
```

The coverage report is generated in `coverage/lcov.info` and can be uploaded to Codecov. The coverage configuration focuses on the core modules that are appropriate for unit testing. Browser-level behaviour in `app.js` is evidenced through manual functional testing and Lighthouse screenshots.

## Build

```bash
npm run build
```

## Deployment

Deploy the repository to Vercel as a static Vite project:

- Build command: `npm run build`
- Output directory: `dist`

Keep the deployment live for 7 consecutive days and screenshot the deployment history for the report.

## Evidence Needed for Report Section 6

- Vercel/Render 7-day live deployment log.
- Codecov badge or Istanbul coverage result showing 80%+.
- Lighthouse Accessibility screenshot showing 90+.
- Screenshot of the English/Chinese language toggle.
- Screenshot of the cookie/localStorage consent banner and privacy policy dialog.
