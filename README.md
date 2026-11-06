# Smart Sync

<!-- LANGUAGES:START -->
[English](README.md) · [Simplified Chinese](docs/i18n/zh-CN/README.md) · [Traditional Chinese](docs/i18n/zh-TW/README.md) · [Japanese](docs/i18n/ja/README.md) · [Korean](docs/i18n/ko/README.md) · [German](docs/i18n/de/README.md) · [French](docs/i18n/fr/README.md) · [Spanish](docs/i18n/es/README.md) · [Brazilian Portuguese](docs/i18n/pt-BR/README.md) · [Russian](docs/i18n/ru/README.md)
<!-- LANGUAGES:END -->

Encrypted synchronization for your Obsidian notes, attachments and selected settings. Preserve original file modification times, recover retained versions and manage your devices.

The Global application server runs on Oracle Cloud in Ashburn, United States. Encrypted object data is stored privately using Cloudflare R2.

We value data security and privacy. Notes, attachments and file paths are encrypted on your device with AES-256-GCM before upload. Encryption and decryption happen on your devices; the service stores encrypted content, and your encryption password is separate from your account login.

**Current version: 1.1.5** · Obsidian **1.12.7+** · Plugin ID: `smart-sync-global`.

[Website](https://smartsync.cc/) · [Download / update](https://smartsync.cc/download/) · [Operation manual](USER-GUIDE.md) · [Plans](https://smartsync.cc/pricing/)

## Get started

1. Back up your notes and try a separate vault first. In Wujie Hub, choose **Smart Sync → Stable**, or download the three plugin files from [Releases](https://github.com/adventurer2008/obsidian-smart-sync-release-global/releases).
2. Install `main.js`, `manifest.json` and `styles.css` in your vault's `.obsidian/plugins/smart-sync-global/` folder. Reload Obsidian and review its trust prompt before enabling the plugin. Updates replace only these three files; preserve settings, secret storage, checkpoints and notes.
3. Open **Settings → Smart Sync → Sign in**, choose Google, GitHub or email, then create or select a cloud vault. Keep its encryption passphrase safe; account login cannot recover it.
4. Review sync preferences, run synchronization and confirm completion before adding another device. Follow the [step-by-step manual](USER-GUIDE.md) for pairing, recovery and troubleshooting.

## Features

- Notes-first synchronization, attachment download policies, exclusions, task progress and optional LAN acceleration with cloud fallback.
- History and deleted-note recovery within retention limits, device pairing/revocation and encrypted configuration recovery.
- Selected Obsidian settings, compatible plugins, themes and snippets synchronized across devices.
- Folder-level sorting, pinned/bottom notes, recent files and local note search.
- Password-protected whole notes or selected text, secure editing and encrypted draft recovery. Titles, linked attachments and earlier plaintext history have separate privacy boundaries.
- Desktop tray where supported and optional Windows launch at login. Mobile systems can suspend background work; return to Obsidian and confirm uploads finish.

Version 1.1.5 also improves narrow-screen action labels, settings refresh, interrupted account operations and browser sign-in recovery. Choose from ten interface languages in Smart Sync settings.

## Account, payments and privacy

Hosted synchronization requires an account. The Free plan currently includes 50 MB, one cloud vault and unlimited devices; paid plans add capacity. Payments are charged in USD. Stripe is the default provider; some accounts may be assigned Dodo Payments. Existing orders and subscriptions stay with their original provider. Review [plans](https://smartsync.cc/pricing/) and [terms](https://smartsync.cc/terms/) before paying.

Content and paths are encrypted on the device. Account identity, vault/device labels, usage and operational metadata are outside content encryption. The Global client keeps diagnostics locally for manual export and does not upload diagnostic telemetry. Encryption and history do not replace independent backups. Read the [privacy policy](https://smartsync.cc/privacy/).

For account deletion, first delete cloud vaults and wait for cleanup, then use **Account → Danger zone → Delete account**, verify the same identity and enter the requested confirmation. Local notes remain.

Questions: [admin@smartsync.cc](mailto:admin@smartsync.cc). Include your platform and plugin/Obsidian versions; never send passwords, tokens, email codes or private notes.
