# Where To Eat — privacy policy hosting

This repository exists for one reason: Google Play and AdMob require a privacy
policy at a **public URL that does not require a login**. The app's own source
repository is private, so the policy is served from here instead.

**Live page:** https://abbadipod.github.io/where-to-eat-privacy/

Nothing else belongs in this repo. It contains no application code.

## Status: DRAFT

The published page is not the operative policy yet. Before the URL goes into
Play Console or AdMob:

1. Fill in every highlighted `TODO` in `index.html` — the responsible party's
   name, a contact email, and the effective date.
2. Implement the UMP consent flow in the app. The advertising section currently
   describes a consent step the app does not present. A policy that claims
   behaviour the binary lacks is a written misstatement, which is a worse
   position than an omission.
3. Remove the draft banner and the `<meta name="robots" content="noindex">` tag.
4. Make sure the Play Console Data Safety form matches this document exactly —
   mismatches between the two are a common cause of review rejection.

The source of truth for the wording lives with the app, at
`docs/privacy-policy.md` in the private `where-to-eat-app` repo, which also
carries the developer checklist. Keep the two in sync — if the app ever adds
analytics, crash reporting, accounts, or a backend, the "does NOT collect"
section here becomes false immediately.
