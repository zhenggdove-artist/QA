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
- Click `選擇本機 QA 資料夾` and choose the local clone of this repository. The browser then writes `qa-config.json` and custom GIFs directly into that folder. No GitHub token, API permission, subscription, or payment is required.
- Click `儲存到本機 QA repository` when needed, or use the normal save button after the folder is connected. GitHub Desktop will show the changed files; review them, Commit, and Push manually.

After pushing, wait for GitHub Pages to finish deploying, then reload:

`https://zhenggdove-artist.github.io/QA/`

The page fetches `qa-config.json` without cache and saved GIF filenames include a version stamp, so other devices receive the new result instead of a cached previous GIF. The original game is not modified.
