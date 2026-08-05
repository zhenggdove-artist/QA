# QA

Standalone question-template site for the artwork.

This repository is intentionally isolated from the original game. It contains only the static template, its required assets, and the GitHub Pages workflow.

## GitHub Pages

The `main` branch is deployed by `.github/workflows/pages.yml`.

Published entry point:

`https://zhenggdove-artist.github.io/QA/`

## Editing and publishing

Open the published page and click `編輯模板`.

- `儲存題目與模板設定` saves a local draft in the current browser. Custom GIF files are stored in IndexedDB, so their size no longer consumes the small `localStorage` quota.
- `發布到 GitHub Pages` publishes the questions, layout settings, and custom GIFs for every device. It writes versioned files under `assets/custom/` and a `qa-config.json` file at the repository root.

The publish button requires a GitHub fine-grained personal access token. Create one for the `zhenggdove-artist/QA` repository only, with `Contents: Read and write`. Paste it into the page only when publishing; the page does not store it. Revoke the token in GitHub after publishing if it was created only for this task.

After publishing, wait for GitHub Pages to finish deploying, then reload:

`https://zhenggdove-artist.github.io/QA/`

The page fetches `qa-config.json` without cache and published GIF filenames include a version stamp, so other devices receive the new result instead of a cached previous GIF. The original game is not modified.
