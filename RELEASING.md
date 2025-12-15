# Releasing CodexUse Desktop

This repository is a download host for installers and auto-update metadata.
The app source code is maintained privately.

## The simple flow

1. Publish the build from the app repo.
   - This creates or updates a GitHub Release tagged `vX.Y.Z` in this repo and uploads artifacts.
2. Edit the GitHub Release body for `vX.Y.Z`.
   - That text is your changelog for users.

Fast path (CLI):

- `gh release edit vX.Y.Z --repo hweihwang/codexuse-desktop-releases --notes-file -`

Paste notes, then press Ctrl+D.

## Optional: keep `CHANGELOG.md` in sync

Copy the same notes into `CHANGELOG.md` under a new `## X.Y.Z (YYYY-MM-DD)` section, then commit and push.

## Notes template

- 1 sentence summary
- Highlights (3 to 6 bullets)
- Fixes (optional)
- Known limitations (keep it honest)
