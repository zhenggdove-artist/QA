Original prompt: Add durable GIF saving and cross-device publishing to the standalone QA GitHub Pages template without changing the original game.

## Completed

- Moved custom GIF drafts from localStorage to IndexedDB.
- Added GitHub Pages publishing for questions, layout settings, and custom assets.
- Added cache-busted config loading and versioned GIF asset paths.
- Verified the standalone page locally and checked JavaScript parsing.

## Remaining

- Publish a configuration from the editor using a user-created fine-grained GitHub token.
- Wait for the GitHub Pages deployment after each publish.
