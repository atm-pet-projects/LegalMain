# Legal links — placeholders and publishing checklist

Use this checklist before external TestFlight or App Store submission. Replace all placeholders below with final values, then verify links in the app and App Store Connect.

---

## Placeholders to replace

| Placeholder | Description | Current value |
|-------------|-------------|---------------|
| `[LEGAL_ENTITY_NAME]` | Legal operator name shown in Privacy Policy and Terms | *Not set — fill in before submission* |
| `[EFFECTIVE_DATE]` | Effective date for Privacy Policy and Terms (e.g. `26 May 2026`) | *Not set — fill in before submission* |
| `[PRIVACY_URL]` | Public URL for `legal/privacy.md` | *Not set — assign after GitHub Pages publish* |
| `[TERMS_URL]` | Public URL for `legal/terms.md` | *Not set — assign after GitHub Pages publish* |
| `[SUPPORT_URL]` | Public URL for `legal/support.md` | *Not set — assign after GitHub Pages publish* |

### Confirmed assumed values (no placeholder)

- **Support email:** atrufanov@alumni.ie.edu
- **Governing law / jurisdiction:** United Kingdom (England and Wales)

---

## GitHub Pages publishing checklist

1. **Create a public repo or public GitHub Pages site** for legal/support content (can be this repo or a dedicated docs repo).
2. **Add the markdown files:**
   - `legal/privacy.md`
   - `legal/terms.md`
   - `legal/support.md`
3. **Replace placeholders** in those files before or immediately after publish:
   - `[LEGAL_ENTITY_NAME]`
   - `[EFFECTIVE_DATE]`
   - Cross-links between documents once URLs are known
4. **Enable GitHub Pages** (Settings → Pages → source branch/folder).
5. **Verify public URLs** open in a private/incognito browser window **without login**.
6. **Record final URLs** and replace app placeholders:
   - `[PRIVACY_URL]`
   - `[TERMS_URL]`
   - `[SUPPORT_URL]`
7. **App Store Connect — Privacy Policy URL:** enter `[PRIVACY_URL]` (final).
8. **App Store Connect — Support URL:** enter `[SUPPORT_URL]` (final).
9. **Verify in-app legal links** (paywall footer, Settings legal rows) open the correct pages on device.
10. **Subscription review notes (if needed):** ensure Apple reviewers can reach Privacy Policy and Support URLs from the paywall or Settings.

---

## App areas likely needing final URL insertion

Search the codebase for placeholder strings and update when URLs are ready:

| Area | What to link |
|------|----------------|
| Paywall footer | Privacy Policy, Terms of Use (and/or Support if shown) |
| Settings legal rows | Privacy Policy, Terms of Use, Support |
| App Store Connect — App Privacy | Privacy Policy URL field |
| App Store Connect — App Information | Support URL field |
| TestFlight / App Review notes | Mention where reviewers find legal and support pages |

---

## Pre-submission review

- **Review these documents** (`legal/privacy.md`, `legal/terms.md`, `legal/support.md`) before external TestFlight or App Store submission.
- Confirm `[LEGAL_ENTITY_NAME]` and `[EFFECTIVE_DATE]` are correct for your situation.
- Confirm published pages match the current app behavior (storage, subscriptions, notifications, no analytics/ads).
- Have qualified counsel review if you need formal legal sign-off beyond MVP/TestFlight readiness.

---

## Suggested final URL pattern (GitHub Pages)

After publishing, URLs often look like:

```
https://<username>.github.io/<repo>/privacy.html
https://<username>.github.io/<repo>/terms.html
https://<username>.github.io/<repo>/support.html
```

Exact paths depend on your Pages configuration (root vs `/docs` folder, `.md` rendering vs HTML export). Use whatever URLs actually resolve publicly, then paste those into the app and App Store Connect.
