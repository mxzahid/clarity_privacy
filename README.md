# Gut Feel legal site

A dependency-free static page containing Gut Feel's Privacy Policy and Terms of Service.

## Deploy to Vercel

1. Create a new Vercel project from this repository.
2. Leave **Root Directory** at the repository root — `index.html` is served from
   there. (An earlier layout nested it under `legal-site`; that is gone.)
3. Leave the framework preset as **Other** and deploy. There is no build command or output-directory setting.

You can also deploy this folder from a terminal with `npx vercel`.

Use the deployed page URL for the combined legal page. Direct document links are:

- Privacy Policy: `https://privacy.gutfeelapp.com/#privacy`
- Terms of Service: `https://privacy.gutfeelapp.com/#terms`

## Before publishing

- Confirm `support@gutfeelapp.com` is monitored for support, privacy, and legal requests.
- Confirm California is the intended governing law and add the operator's legal name and mailing address when available.
- Have qualified counsel review both documents for the markets where Gut Feel will be offered.
- Keep `index.html` synchronized with the `LegalDocument` enum in
  `clarity/frontend/Clarity/SettingsView.swift` when the product's data flows,
  vendors, retention, or pricing change. That enum is the copy users actually
  agree to in-app, so it is the source of truth and this page follows it — not
  the other way round. The effective date at the top of each must match
  `LegalDocument.updated`.

  The two drifted badly once already: the app moved to the Stripe/Link rail on
  2026-08-02 while this page still described Apple-only billing and named
  Superwall, a vendor no longer in the flow. Diff the two whenever either
  moves.
