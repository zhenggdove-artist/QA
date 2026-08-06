Original prompt: Add durable GIF saving and cross-device publishing to the standalone QA GitHub Pages template without changing the original game.

## Completed

- Moved custom GIF drafts from localStorage to IndexedDB.
- Added local repository publishing for questions, layout settings, and custom assets without GitHub tokens or API writes.
- Added cache-busted config loading and versioned GIF asset paths.
- Verified the standalone page locally and checked JavaScript parsing.

## Remaining

- Connect the editor to the local `QA` folder, save, then review/commit/push the generated files with GitHub Desktop.
- Wait for the GitHub Pages deployment after each publish.
