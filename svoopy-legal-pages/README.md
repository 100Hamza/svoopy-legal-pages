# Svoopy legal pages

A static, responsive GitHub Pages site containing:

- `index.html` — legal-page landing page
- `privacy-policy.html` — Privacy Policy
- `terms-and-conditions.html` — Terms & Conditions
- `assets/svoopy-mark.png` — cropped mark used in the header
- `assets/svoopy-logo-full.png` — original supplied logo image

The pages use embedded CSS, relative navigation, and no external libraries, fonts, scripts, or images.

## Before publishing

Replace every bracketed placeholder, including:

- `[FULL LEGAL NAME OF COMPANY]`
- `[COUNTRY]` and `[COUNTRY / GOVERNING LAW]`
- `[BUSINESS ADDRESS IF REQUIRED]`
- `[DATE]` and `[YEAR]`
- `[SUPPORT EMAIL]` / `[SUPPORT AND ACCOUNT-DELETION EMAIL]`
- `[IN-APP ACCOUNT-DELETION REQUEST PATH]`
- the account-deletion processing timeframe
- wallet refunds, treatment of balances below €100, and replay-removal refund/credit rules
- legal review placeholders for jurisdiction, liability, and disputes

The email links currently point to `mailto:replace-support-email@example.invalid`. Replace the `href` in each email link with the client's real address, for example `href="mailto:help@yourdomain.com"`, and replace the visible placeholder text too. The `.invalid` address is intentionally non-functional.

Confirm the descriptions match the production app and backend before publishing—especially public profile-location visibility, chat access, recording behavior, deletion steps, and payment rules. Remove the yellow draft-warning banners from the HTML pages after all placeholders and client-review items have been resolved.

## GitHub Pages

1. Upload the files in this folder to the root of a GitHub repository (or keep the folder and adjust the Pages source accordingly).
2. In the repository, open **Settings → Pages** and configure deployment from the branch and folder containing `index.html` (commonly `main` and `/(root)`).
3. After deployment, the pages will be available at paths similar to:
   - `/privacy-policy.html`
   - `/terms-and-conditions.html`

The links between pages are relative, so they work on a GitHub Pages project site as well as on a custom domain.
