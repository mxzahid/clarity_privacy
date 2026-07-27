# Clarity legal site

A dependency-free static page containing Clarity's Privacy Policy and Terms of Service.

## Deploy to Vercel

1. Create a new Vercel project from this repository.
2. Set **Root Directory** to `legal-site`.
3. Leave the framework preset as **Other** and deploy. There is no build command or output-directory setting.

You can also deploy this folder from a terminal with `npx vercel`.

Use the deployed page URL for the combined legal page. Direct document links are:

- Privacy Policy: `https://YOUR-DOMAIN/#privacy`
- Terms of Service: `https://YOUR-DOMAIN/#terms`

## Before publishing

- Confirm `hello@gnsheep.com` is monitored for support, privacy, and legal requests.
- Confirm California is the intended governing law and add the operator's legal name and mailing address when available.
- Have qualified counsel review both documents for the markets where Clarity will be offered.
- Keep `index.html` synchronized with `clarity/frontend/Clarity/SettingsDrawer.swift` when the product's data flows, vendors, retention, or pricing change.
