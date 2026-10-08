# Care Without Barriers — website

Static landing page and privacy policy for the Care Without Barriers app. No build step:
plain HTML + one stylesheet. Colours mirror `MpColors` in the app.

```
index.html     landing page
privacy.html   privacy policy (draft — see below)
styles.css     shared styles, light + dark
assets/        icon and app screenshots (from marketing/store/screenshots/raw-ios in the app repo)
```

Preview locally:

```bash
python3 -m http.server 8080
```

Deploy: any static host (GitHub Pages, Vercel, Netlify) serving this folder's root.

## Before publishing the privacy policy

- Fill every highlighted `[PLACEHOLDER]` in `privacy.html` (operator, address, privacy
  contact, effective date, Vercel log retention).
- Confirm OpenAI zero data retention and the DPA (`docs/provider-retention.md` in the app repo).
- Complete the Quebec Law 25 transfer assessment.
- Counsel review (PIPEDA + provincial acts).
- Link the policy URL from the app (`privacy_policy_note`) and both store listings.
