# Svoopy legal pages and in-app text

This package contains the Svoopy legal website, copy-ready in-app policies, and the editable Manual Guide for the app’s Help page.

## Included files

- `index.html` — legal landing page and company contact details
- `privacy-policy.html` — web Privacy Policy
- `terms-and-conditions.html` — web Terms & Conditions
- `in-app-text/privacyPolicy.txt` — copy-ready in-app Privacy Policy
- `in-app-text/termsAndConditions.txt` — copy-ready in-app Terms & Conditions
- `in-app-text/manual-guide.txt` — editable Manual Guide content for the admin-managed Help page
- `assets/` — Svoopy logo assets used by the website

## Company details used

- Operator: Joy and Media Ltd
- Registration jurisdiction and Terms governing law: England and Wales
- Registered office: 71-75 Shelton Street, London WC2H 9JQ, United Kingdom
- Support and account-deletion email: info@joyandmedia.com

The company registration number was not supplied and has not been invented or inserted. UK company website disclosures generally require the company number as well as the registration jurisdiction and registered office; add it when available before public website publication.

## Publishing the website

Upload the contents of this folder to the repository root (or a `docs` folder) and configure GitHub Pages to publish that folder. Keep the `assets` folder alongside the HTML files. The site uses embedded CSS and relative links, without external scripts, fonts, or image CDNs.

## Updating in-app text

Paste the policy files into the admin/Firestore fields used by the app:

- `in-app-text/privacyPolicy.txt` → collection `csTermsAndConditions`, field `privacyPolicy`
- `in-app-text/termsAndConditions.txt` → collection `csTermsAndConditions`, field `termsAndConditions`

The Manual Guide is a separate editable content file for the admin-managed Help page. No content has been written to Firebase by this package; the files must be added through the app’s admin workflow.

For clickable in-app email or web links, use a separate clickable text widget if needed; the existing `TranslatedText` implementation is unchanged.
