# 1m — privacy policy and support pages

The public pages for **1m**, an iOS app that turns logs and code on your screen into a
ready-made prompt for an LLM app on your phone.

This repository holds **only these pages**. The app's source is private and is not here.

| Page | URL |
| --- | --- |
| Overview | https://myagkiy.github.io/1m/ |
| Privacy Policy | https://myagkiy.github.io/1m/privacy/ |
| Support | https://myagkiy.github.io/1m/support/ |

The two lower rows are the URLs entered in App Store Connect. **They must not move.** Apple
re-checks them after release, and a dead privacy policy URL puts the listing at risk.

## Layout

```
index.html          overview
privacy/index.html  privacy policy
support/index.html  support page
assets/style.css    shared stylesheet
.nojekyll           serve the files as-is, no Jekyll processing
```

Published by GitHub Pages from the root of `main`.

No build step, no dependencies. The pages load no fonts, scripts, images or trackers from
anywhere — a privacy policy that phones a third party to render itself is not one anybody
should believe.

## Editing

Edit the HTML and push. GitHub Pages redeploys in about a minute.

When the privacy policy changes in substance, update the effective date at the top of
`privacy/index.html`. The previous wording stays in this repository's history, which is what
makes "the previous wording remains in the public page history" true.

## Three things that must agree

The privacy policy is one of three declarations about the same facts. If any one of them
changes, check the other two:

1. **This page** — `privacy/index.html`
2. **The App Store privacy label** — App Store Connect → App Privacy (currently *Data Not Collected*)
3. **The privacy manifest** — `PrivacyInfo.xcprivacy` in the app repository

Apple compares them, and a mismatch is grounds for rejection.
