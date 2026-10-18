# Guarita review target

Static, fictional test fixture operated by Guarita at https://guarita-review-target.pages.dev.

This repository contains only the technical test page and a public ownership proof when provisioned. It contains no Guarita application source, credentials, account IDs, scan reports, customer information, billing code or reviewer passwords.

The site provides an authorized target for Guarita's ownership verification and basic scanner. It is deployed to a dedicated Cloudflare Pages project by uploading only `index.html`, `404.html`, `_headers` and the public proof file. No custom domain or other project's infrastructure is used. GitHub Pages is not the scanner origin.

The initial deployment had no custom response headers and produced a real missing Content-Security-Policy finding. The current `_headers` adds a policy for testing the remediation and retest flow. Historical findings belong to their original scan; future scan outcomes must be checked rather than assumed. The `404.html` file ensures missing paths return a real 404 instead of a single-page-app fallback.

The `.well-known/guarita-verification.txt` file is a deliberately public challenge, not an authentication credential. Keep the file for subsequent ownership revalidation. Do not replace it with passwords, API keys or OAuth tokens.

Reviewer accounts, reports, evidence and execution scripts are maintained separately. No marketplace approval or partnership is implied by this fixture.

Copyright 2026 Guarita. All rights reserved.
