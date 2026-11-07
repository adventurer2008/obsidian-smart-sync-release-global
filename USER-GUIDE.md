# Smart Sync user guide

Current Stable version: **1.1.9**. Refresh the Global version list in Hub and choose Stable for updates.

<!-- LANGUAGES:START -->
[English](USER-GUIDE.md) · [Simplified Chinese](docs/i18n/zh-CN/USER-GUIDE.md) · [Traditional Chinese](docs/i18n/zh-TW/USER-GUIDE.md) · [Japanese](docs/i18n/ja/USER-GUIDE.md) · [Korean](docs/i18n/ko/USER-GUIDE.md) · [German](docs/i18n/de/USER-GUIDE.md) · [French](docs/i18n/fr/USER-GUIDE.md) · [Spanish](docs/i18n/es/USER-GUIDE.md) · [Brazilian Portuguese](docs/i18n/pt-BR/USER-GUIDE.md) · [Russian](docs/i18n/ru/USER-GUIDE.md)
<!-- LANGUAGES:END -->

Applies to Smart Sync (`smart-sync-global`). [Website](https://smartsync.cc/) · [Downloads](https://smartsync.cc/download/) · [Privacy](https://smartsync.cc/privacy/).

## Install or update

Use Obsidian **1.12.7 or newer**.

### Install from Obsidian Community plugins

Once Smart Sync is listed in the Obsidian community directory, you can install it directly in Obsidian:

1. Open Settings → Community plugins in Obsidian.
2. If community plugins are disabled, select Turn on community plugins and review the notice shown by Obsidian.
3. Select Browse, search for Smart Sync, and open its listing (author: lihy).
4. Select Install, then Enable.

### Wujie Hub or manual download

In Wujie Hub, choose **Smart Sync → Stable** for the current stable package.

For manual installation, download `main.js`, `manifest.json` and `styles.css` from the matching [GitHub Release](https://github.com/adventurer2008/obsidian-smart-sync-release-global/releases). Check its `SHA256SUMS.txt`. Place the three files in `<vault>/.obsidian/plugins/smart-sync-global/` (or your custom configuration folder's `plugins/smart-sync-global/`). Reload Obsidian, then enable Smart Sync in Community plugins after reviewing the host's trust prompt yourself.

For an update, disable the plugin, replace **only those three program files**, then reload and enable it. Preserve `data.json`, secret storage, synchronization checkpoints and all notes. Do not copy another device's plugin settings or credentials into this vault. Keep the previous program files and an independent backup; downgrading program files cannot undo cloud deletions or other completed cloud operations. Do not run multiple sync providers on the same vault without resolving their interactions.

## Sign in and connect your first vault

1. Open **Settings → Smart Sync → Sign in**. Choose Google, GitHub or email. Social sign-in uses the system browser; email verification uses a short-lived code in the plugin dialog.
2. Return to Obsidian after authorization. Automatic checks resume after a temporary network failure or returning to the app. If still waiting, use **Check sign-in** in the pending dialog. If the request expires, reopen Sign in. Never share a sign-in code.
3. Create a cloud vault or select an existing vault, then follow the encryption-passphrase prompt. Keep the passphrase safe: account login cannot recover it. A matching vault name alone does not identify the same cloud vault.
4. Review synchronization direction, attachment downloads, exclusions and configuration scope before synchronizing existing files.
5. Run **Synchronize notebook now**, open **Sync tasks and history**, and wait for completion. Check representative notes, attachments and original modification times before connecting another device.

If a vault-creation reply is lost, use the pending operation's recovery message and check existing cloud vaults. Do not repeatedly create new vaults with different names.

## Add another device

If you are signed in but have not connected this local vault, **Add device** first guides you to select a cloud vault explicitly. Connect the intended vault before approving another device; the plugin does not select one automatically.

Install the same regional plugin, sign in to the same account and select the same cloud vault. Use its original encryption passphrase. The device-management flow also offers a six-digit pairing code: obtain it on the new device, approve it from an already connected device using **Add device**, and compare the displayed fingerprint before approving. Include leading zeroes. Expired or used codes must be regenerated.

Review each device's local filters and attachment policy. A cloud upload finishing on one device does not mean every other device has downloaded it.

## Synchronization, attachments and offline recovery

Use two-way synchronization for ordinary editing. Upload only, receive only, update-existing and paused modes deliberately restrict which changes move; read the direction prompt before switching modes. Stopping a round pauses automatic synchronization until you choose **Sync now** or **Retry**.

Markdown notes are prioritized before attachments during full and incremental body transfers. Directory, rename and deletion dependencies still take their safe order, and an active transfer can finish before newly queued notes. Embedded images or PDFs may arrive later. Choose the attachment download policy in synchronization preferences; use **Download pending attachments** when needed. Metadata inspection and network conditions still affect total time.

Local edits remain local while offline. When the network returns, reopen Obsidian, resume synchronization if paused, and inspect remaining tasks. On phones and tablets, keep Obsidian in the foreground until important changes finish. Locking the screen or backgrounding the app can suspend it; desktop tray settings do not provide mobile background execution.

Sync carries the source file's original modification time when that metadata is available. An old cloud revision lacking it cannot be treated as having preserved the original time; resynchronize from a source that retains it. A merge producing new content has a new modification time.

LAN acceleration is optional. Check its connection status; if direct connections are unsupported or no peer is available, cloud synchronization remains the fallback. Same-network discovery is not a guarantee that a direct link will work.

## Recover earlier versions and deleted notes

Open a synchronized note and choose **View note history and restore** from its context menu, or **Show active note history** from the command palette. Review the revision and differences before restoring. Use **Show deleted notes** to review recoverable deleted content. Availability depends on the vault's retention policy; expired or purged history cannot be restored.

Use **Retention, usage and cleanup** to review history policy and cloud usage. Cleanup and purge actions permanently remove eligible history; back up first and read the confirmation. History is not a substitute for an independent backup.

## Sync selected Obsidian settings

Expand synchronization preferences and the configuration categories. Editor preferences, appearance, hotkeys, bookmarks, community plugin code, plugin data, plugin enablement, themes and snippets have separate controls. Review individual exclusions before enabling a category. Plugin enablement changes can require restarting Obsidian. Desktop-only plugins are skipped on mobile; check third-party plugin compatibility before enabling their code or data there.

Filter presets apply this device's exclusions, attachment threshold and configuration scope. Applying one pauses synchronization; review it and resume explicitly. Presets do not copy account keys or bind another cloud vault. Use **Export encrypted configuration recovery** for protected recovery and store its password separately; never share the recovery file and password together.

## Sorting, pins, recent files and search

Enable sorting and set the root rule; deeper levels can inherit the parent rule or use a custom one. Use a note's context menu to **Pin**, **Unpin**, **Move to bottom** or **Remove from bottom**. Pin changes wait for synchronization to reach other devices.

Enable recent files to use the clock tab in the left sidebar or **Recent files** command; disabling it stops recording opened files. Enable note search to search locally available notes. Attachments that have not downloaded are not locally available content.

## Password-protect a note or selected text

Open a Markdown note, select text in editing mode if needed, then run **Encrypt selected text** or **Encrypt entire note**. Set and confirm a separate password, read the warning and save. Click encrypted content to unlock it; its actions include **Edit**, **Lock**, **Change password** and **Decrypt permanently**. Edit through the secure editing window so saves remain encrypted.

Titles remain visible. Linked images and attachments are not automatically encrypted with the selected text. Earlier history and backups may retain plaintext. Permanent decryption writes ordinary plaintext locally and synchronizes it normally. Password hints are not encrypted. Passwords are not recoverable.

Use **Note encryption settings** to choose the inactivity lock timeout, or **Lock all encrypted content now**. Closing the note, leaving the vault or moving the app to the background also locks it. If saving fails, follow **Recover encrypted drafts** to recover a separate encrypted note with the original password; do not delete the original to repair the error.

## Desktop tray and Windows startup

On supported desktop hosts, **Advanced → Run in background with tray icon** is on by default. Closing the vault window keeps it running; click its tray icon to restore it. Its menu can close only this vault. Unsupported tray hosts retain normal closing. Mobile hides this option.

**Launch to tray at login** is Windows-only and off by default. Enabling it creates this vault's shortcut in the current user's Startup folder and enables the background tray. Ordinary launches stay visible. Custom Obsidian profiles cannot enable startup because the host may route requests to another instance. Disable login startup before disabling the tray, uninstalling or reverting to a version without startup support. macOS, Linux, Android, iPhone and iPad do not show the Windows startup switch.

## Storage plans and payments

Open the storage-plan entry in settings to view the current plan. Mobile tries to open the system browser directly; use the offered link if the handoff fails or cannot be confirmed. Review the amount, currency, interval and renewal terms before paying. Checkout uses USD through the provider assigned to your account: Stripe by default, or Dodo Payments for eligible accounts. Reopening an unpaid purchase resumes its original checkout. Existing orders and subscriptions keep their provider; do not pay again while a result is uncertain. Return to the app and verify the plan update; inspect an uncertain order before paying again.

The Free plan includes 50 MB, one cloud vault and unlimited devices. Paid capacities and current terms are shown on the [plans page](https://smartsync.cc/pricing/). Storage is shared across the account's cloud vaults.

## Sign out, revoke a device or delete an account

Signing out retains local notes. If offline sign-out cannot confirm remote revocation, revoke the device from another connected device when immediate removal is needed. Uninstalling does not delete the cloud account.

Cloud deletion is destructive: verify an independent local backup first. Delete cloud vaults through vault management and wait for cleanup. Open **Account → Danger zone → Delete account**, verify the same account when prompted, and type **DELETE** exactly. Paid service time does not prevent deletion. This removes account access and connected identities; local notes remain. Read the [retention policy](https://smartsync.cc/privacy/).

## Troubleshooting and device limits

Read the recovery action shown with the error. At a device or vault limit, connect an existing vault, revoke an unused device, or choose a suitable plan. Export diagnostics manually if support needs them; the Global client does not upload diagnostic telemetry. Send the visible error, plugin/Obsidian versions and platform to [admin@smartsync.cc](mailto:admin@smartsync.cc). Remove passwords, tokens, verification codes and private note content.


## Interface language

This version supports English, Simplified and Traditional Chinese, Japanese, Korean, German, French, Spanish, Brazilian Portuguese and Russian.

Choose Follow Obsidian or an explicit language in Interface language near the top of Smart Sync settings. The choice applies only to this local vault on this device. Save it, finish any active synchronization, then reload the plugin or restart Obsidian to update settings, commands and menus together.

This changes display text only. Service region, accounts, cloud vaults, encryption passwords, file contents and synchronization progress do not change. Different devices may use different languages.
