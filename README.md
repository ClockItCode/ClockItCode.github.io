# ClockItCode — sites

This folder is the home for websites Claude generates for Allison. It's a git repo connected to
**github.com/ClockItCode/ClockItCode.github.io** and published with **GitHub Pages**.

- **Live URL:** https://clockitcode.github.io
- **Landing page:** `index.html` (a hub that links to each site)
- **Each new site:** lives in its own subfolder, e.g. `my-site/index.html` →
  served at `https://clockitcode.github.io/my-site/`

## Publishing a change
From this folder:

```sh
git add -A
git commit -m "update site"
git push
```

Changes go live at https://clockitcode.github.io within ~1 minute. (Or just ask Claude to build/update
a site and push it for you.)

## How it's wired
- Auth: the `gh` CLI is logged in as `ClockItCode`; HTTPS pushes authenticate automatically.
- Pages source: the `main` branch, repo root (automatic for a `<user>.github.io` repo).
