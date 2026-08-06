Original prompt: Add durable GIF saving and cross-device publishing to the standalone QA GitHub Pages template without changing the original game.

## Completed

- Moved custom GIF drafts from localStorage to IndexedDB.
- Added local repository publishing for questions, layout settings, and custom assets without GitHub tokens or API writes.
- Added cache-busted config loading and versioned GIF asset paths.
- Verified the standalone page locally and checked JavaScript parsing.
- Reduced the published template to one question at runtime, including old local snapshots and reset state.
- Added a preloaded, muted, looping MP4 fallback for the first transparent GIF so mobile browsers do not freeze on its first frame.
- Composited the fallback video on black to preserve the template's transparent-on-black visual appearance.
- Verified at a 390px mobile viewport that only one question loads and the video `currentTime` advances while looping.

## Remaining

- Connect the editor to the local `QA` folder, save, then review/commit/push the generated files with GitHub Desktop.
- Wait for the GitHub Pages deployment after each publish.
