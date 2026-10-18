# Guarita review target

Static, fictional test fixture operated by Guarita at https://review-target.guarita.dev.

This repository contains only the technical test page, its custom-domain configuration and a public ownership proof when provisioned. It contains no Guarita application source, credentials, account IDs, scan reports, customer information, billing code or reviewer passwords.

The site provides an authorized target for Guarita's ownership verification and basic scanner. GitHub Pages response headers can produce real findings (such as a missing Content-Security-Policy) useful for testing catalog remediation prompts. No scan outcome is predeclared here.

The `.well-known/guarita-verification.txt` file is a deliberately public challenge, not an authentication credential. Keep the file for subsequent ownership revalidation. Do not replace it with passwords, API keys or OAuth tokens.

Reviewer accounts, reports, evidence and execution scripts are maintained separately. No marketplace approval or partnership is implied by this fixture.

Copyright 2026 Guarita. All rights reserved.
