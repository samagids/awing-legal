# awing-legal

Public policy and support pages for the **Awing Learning** app.

This repository exists only so those two pages have a public HTTPS URL that
Apple and Google can fetch during review:

- https://samagids.github.io/awing-legal/privacy
- https://samagids.github.io/awing-legal/support

## Why this is a separate repository

GitHub Pages needs a **public** repository on the free plan. The app lives in
the private `samagids/awing-learning`, and making that public would also
publish the Awing dictionary PDFs, the family audio recordings, the Firestore
and Storage rules and the whole commit history. So only these pages are
public.

Before this repo existed, both store listings pointed at
`samagids.github.io/awing-ai-learning/privacy`, which had never resolved —
Pages had never been enabled, because the repo was private. Renaming the repo
could not have fixed that.

## Keeping it in sync

`privacy.md` here is generated from `docs/privacy.md` in the app repo: the app
repo's copy is the source of truth. When it changes, copy the body across and
keep the Jekyll front matter at the top of this one.

Jekyll renders `privacy.md` to `/privacy` and `support.md` to `/support`, so
the paths in the store listings must not gain a `.html`.
