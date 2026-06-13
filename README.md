# CodexUse Desktop Releases

Official downloads for **CodexUse** — the local control plane for the Codex app and Codex CLI.

One cockpit for every Codex account: switch accounts without re-auth, watch live rate-limit headroom, orchestrate Codex App windows, and pool quota across accounts behind one local API.

This repo hosts download artifacts only. It does not contain the app source.

## Download

- **Latest release:** https://github.com/hweihwang/codexuse-desktop-releases/releases/latest
- **macOS (Apple Silicon):** https://github.com/hweihwang/codexuse-desktop-releases/releases/latest/download/stable-macos-arm64-CodexUse.dmg
- **Homebrew:** `brew install --cask hweihwang/codexuse/codexuse`
- **CLI (optional):** `npm install -g codexuse-cli`

macOS on Apple Silicon. Intel Mac and Linux desktop builds are not shipped.

## What you get

- **Codex App orchestration** — launch, focus, stop, and restart profile-matched Codex App windows from one cockpit.
- **Account switching without re-auth** — keep personal, work, and client profiles signed in locally; switch from the window, tray, or CLI.
- **Live rate-limit headroom** — usage and reset windows per account, so you switch before a 429.
- **Auto-roll (Pro)** — roll to an eligible profile when an account runs low, behind a confirm guardrail.
- **Accounts Pool (Pro)** — one local OpenAI-compatible API that shares quota across selected accounts with load-balancing and failover.
- **Telegram alerts and manual cloud sync (Pro).**
- **Local-first** — profiles, settings, and state stay on your machine. CodexUse signs in with the Codex CLI OAuth login and needs no API keys of its own.

Free covers 2 profiles, account switching, Codex App orchestration, and live headroom. Pro ($19.50 lifetime) adds Accounts Pool, auto-roll, unlimited profiles, Telegram alerts, MCP & Skills installs, and cloud sync.

## Install (macOS)

1. Download the `.dmg` from the latest release, or run `brew install --cask hweihwang/codexuse/codexuse`.
2. Open it, then drag CodexUse into Applications.
3. Launch CodexUse. If macOS blocks it, right-click the app and choose Open once.

Homebrew installs upgrade with `brew upgrade --cask codexuse` (not the in-app updater).

## Links

- Website: https://codexuse.com
- Docs: https://codexuse.com/docs/
- Support: https://github.com/hweihwang/codexuse-desktop-releases/issues
