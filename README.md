# Svoopy legal pages

A static, responsive GitHub Pages site containing:

- `index.html` — legal-page landing page
- `privacy-policy.html` — Privacy Policy
- `terms-and-conditions.html` — Terms & Conditions
- `assets/svoopy-mark.png` — cropped Svoopy mark used in the header
- `assets/svoopy-logo-full.png` — original supplied logo image

The pages use embedded CSS, relative navigation, and no external libraries, fonts, scripts, or image CDNs.

## Remaining client details before publishing

Replace the remaining operator/contact placeholders in both policy pages and the landing page:

- `[LEGAL OPERATOR NAME]` (confirm whether the Play Console display name is also the legal operator name)
- `[COUNTRY / JURISDICTION]` and `[COUNTRY / GOVERNING LAW]`
- `[BUSINESS ADDRESS IF REQUIRED]`
- `[SUPPORT AND ACCOUNT-DELETION EMAIL]` (one shared email)

The email links currently point to `mailto:replace-support-email@example.invalid`. Replace every such `href` with the client’s actual email, for example `href="mailto:help@yourdomain.com"`, and replace the visible placeholder text. The `.invalid` address is intentionally non-functional.

The policies reflect the supplied Svoopy behavior: the in-app support path is **Admin Chat Drawer → Help & Support → Customer Support → Chat Now**; account deletion is handled by an administrator and normally takes 7–14 working days after any eligible withdrawal/payment matter is resolved; failed or unconfirmed payments do not unlock replay access; and a replay with active paid access remains available to that purchaser until the access period ends. The account-deletion-under-€100 balance rule is intentionally not stated.

Remove the yellow operator-details banners from the HTML pages once the remaining operator/contact placeholders have been filled. Confirm that the final copy matches the production app.

## GitHub Pages

1. Upload the files in this folder to the repository root, or put them in a `docs` folder and select that folder as the Pages source. Keep the `assets` folder alongside the HTML pages.
2. In the repository, open **Settings → Pages** and configure deployment from the branch and folder containing `index.html` (commonly `main` and `/(root)`).
3. After deployment, the pages will be available at paths similar to `/privacy-policy.html` and `/terms-and-conditions.html`.

The links between pages are relative, so they work on a GitHub Pages project site as well as on a custom domain.
