# CodexUse Desktop Releases

Official downloads for CodexUse.

CodexUse is a desktop companion for AI coding CLIs. It helps you keep multiple accounts logged in, switch profiles fast, and avoid rate limit surprises.

This repo only hosts release artifacts and changelogs. It does not contain the app source code.

## Download

- Latest release: https://github.com/hweihwang/codexuse-desktop-releases/releases/latest
- macOS (Apple Silicon): https://github.com/hweihwang/codexuse-desktop-releases/releases/latest/download/CodexUse-mac-arm64.dmg
- Linux (ARM64): https://github.com/hweihwang/codexuse-desktop-releases/releases/latest/download/CodexUse-linux-arm64.AppImage

## What you get

- Profile switching across multiple accounts (tray or window)
- Works with Codex CLI and Claude Code (pick per profile)
- Rate limit telemetry so you can see throttling before 429s
- Auto-roll to a fresh profile when you hit a threshold
- Local-first: reads and writes the same `~/.codex` files your CLIs use

## Install

### macOS

1. Download the `.dmg` from the latest release.
2. Open it, then drag CodexUse into Applications.
3. Launch CodexUse.

If macOS blocks the app, right-click the app and choose Open once.

### Linux

1. Download the `.AppImage` from the latest release.
2. Make it executable: `chmod +x CodexUse-linux-*.AppImage`
3. Run it: `./CodexUse-linux-*.AppImage`

## Changelog

- Release notes (canonical): https://github.com/hweihwang/codexuse-desktop-releases/releases
- Changelog file (mirror): `CHANGELOG.md`

## Links

- Website: https://codexuse.com
- Support: email `hoangmaths96@gmail.com`
