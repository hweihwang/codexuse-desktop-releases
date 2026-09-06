# CodexUse Desktop Releases

Plan with your best model. Build with the right model.

CodexUse is an independent Apple Silicon Mac app for the Codex app and Codex CLI. It keeps every Codex account in its own window, runs planners in their own Codex windows and workers in isolated Git worktrees, and lets you review before anything merges. This repository contains public download artifacts, not the app source. CodexUse is not affiliated with OpenAI.

## Download and install

1. Open Apple menu → About This Mac. The desktop app requires an Apple Silicon chip. Intel Mac, Windows, and Linux desktop builds are not shipped.
2. On an Apple Silicon Mac, download the DMG from the [latest release](https://github.com/hweihwang/codexuse-desktop-releases/releases/latest), or run `brew install --cask hweihwang/codexuse/codexuse`.
3. For a DMG install, open the image and drag CodexUse into Applications. Open CodexUse. If macOS reports a damaged or unverified download, stop and use the [troubleshooting guide](https://codexuse.com/docs/troubleshooting/). Do not disable macOS security checks.

Homebrew installs update with `brew upgrade --cask codexuse`, not the in-app updater.

Not sure which Mac you have? Read the [desktop guide](https://codexuse.com/docs/desktop/). The separate [CLI](https://codexuse.com/docs/cli/) runs on macOS, Windows, and Linux: `npm install -g codexuse-cli`. The CLI does not provide desktop feature parity.

## What CodexUse does

- **Work.** Describe a task, pick a folder and separate planner and worker accounts. The planner plans in its own Codex window. The worker builds in an isolated Git worktree and receives a bounded brief. Review and apply the changes to your working folder; you commit and push them yourself. Work does not replace native Codex subagents.
- **One Codex window per account.** Every OpenAI or custom-model account has one window. Open starts it, Show brings it to the front. CodexUse never opens a second window for the same account and never signs another account out.
- **Headroom, refill timers, Auto-roll.** See the usage windows and refill times Codex reports. Refill controls attempt short background requests; they do not add quota or accelerate refill times. Auto-roll can open another eligible account below a threshold you set; it does not move a running conversation.
- **Custom-model accounts.** Run OpenRouter, DeepSeek, Groq, or a local model inside the Codex app as its own account. Provider usage is billed by the provider; hosted ChatGPT features such as dictation are unavailable on those accounts.
- **Account Pool.** One local OpenAI-compatible API across selected accounts, with load balancing and failover. It is not a hosted service and does not raise any account's limit.
- **Telegram and Cloud Sync.** Telegram remote for tasks, and manual passphrase-encrypted Cloud Sync for accounts and settings. Cloud Sync does not upload run state or conversation history.

OpenAI accounts sign in with the Codex CLI OAuth flow and need no OpenAI API key. Custom-model accounts use your provider credential, stored in the macOS Keychain. MCP and Skills installers are not included.

## Trial and Pro

Try every app feature for 7 days. Then features lock until a Pro license is activated. Nothing is deleted. There is no permanent free tier.

Pro is a one-time lifetime license: $39 regular price, currently $19.50 with SUMMER50. One license supports up to 5 Macs. There is a 30-day refund window. Account quotas and provider charges remain separate.

Buy inside CodexUse to enable automatic activation. If you buy on the website, enter the license key from your Gumroad receipt in CodexUse. If you already paid, do not buy again.

## Links

- [Website](https://codexuse.com/)
- [Getting started](https://codexuse.com/docs/getting-started/)
- [Work](https://codexuse.com/docs/work/) · [Accounts](https://codexuse.com/docs/accounts/)
- [Documentation](https://codexuse.com/docs/)
- [Support](https://github.com/hweihwang/codexuse-desktop-releases/issues)
