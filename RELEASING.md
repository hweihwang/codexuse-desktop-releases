# Releasing CodexUse Desktop (this repo)

This repository is a download host. The app source code is maintained privately. GitHub Releases are published here because Electron auto-updates read from this repo.

The goal: every GitHub Release has good notes, and `CHANGELOG.md` stays the canonical history.

## Before you publish a new version

1. Update `CHANGELOG.md` under `Unreleased` (keep it user-facing).
2. Commit and push the changelog to `main` in this repo.

## Publish (from the app repo)

Run your normal build and publish flow from the app repo. Electron Builder publishes assets to:

https://github.com/hweihwang/codexuse-desktop-releases

It will create or update a GitHub Release tagged `vX.Y.Z` and upload installers plus the `latest-*.yml` files used by auto-update.

## Add release notes on GitHub

Because this repo has almost no commit history, GitHub auto-generated notes are not useful here.
Use the matching section from `CHANGELOG.md` as the release body.

Example (edit notes after publish):

1. Open the release: https://github.com/hweihwang/codexuse-desktop-releases/releases
2. Click "Edit"
3. Paste the `CHANGELOG.md` notes for that version

If you prefer the CLI and you have `gh` authenticated:

- `gh release edit vX.Y.Z --repo hweihwang/codexuse-desktop-releases --notes-file -`

Then paste notes into stdin and press Ctrl+D.

## Writing good notes (quick checklist)

- Start with a 1 sentence summary.
- Add 3 to 6 bullets under "Highlights".
- Call out anything that changes behavior or requires action.
- Mention platform support changes (macOS, Linux, Windows).
