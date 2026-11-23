# scaffolding.kairoscc.io redirect

Keeps every old scaffolding.kairoscc.io link working after the site moves to kairoscc.io.
GitHub Pages serves one custom domain per repo, so this goes in its own repo:

1. Create a public repo (e.g. `kairos-cc/scaffolding-redirect`) with these three files at its root.
2. Settings › Pages: deploy from `main`, custom domain `scaffolding.kairoscc.io`, enforce HTTPS.
3. Keep the existing `scaffolding` DNS CNAME pointing to `kairos-cc.github.io`.

`404.html` is a copy of `index.html`, so any path (e.g. `/small-team/`) redirects to its new page.
