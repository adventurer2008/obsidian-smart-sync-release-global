# Smart Sync

Sync notes, attachments and selected settings with client-side encryption. Keep original file modification times, manage devices and recover earlier versions. Additional local tools include sorting, pinned notes, recent files and password-protected note content.

Plugin ID: `smart-sync-global`. Version 1.1.5 includes the maintained account, settings and mobile browser-handoff fixes. Download the three plugin files from [Releases](https://github.com/adventurer2008/obsidian-smart-sync-release-global/releases), or select Smart Sync in Wujie Hub, then follow the [user guide](USER-GUIDE.md). Publication here does not mean Obsidian has approved or listed the plugin.

## Account and payments

An account is required for hosted synchronization. Sign in with Google, GitHub or an emailed code. A free storage tier is available; additional storage is a paid subscription. See current [plans](https://pay.smartsync.cc/pay/plans) before purchase. Stripe handles checkout and recurring subscriptions. Account sign-in does not replace the encryption passphrase; keep that passphrase safe.

To delete an account, first delete its cloud vaults and wait for cleanup. The plugin then requires identity verification and confirmation. Account deletion does not automatically refund payments. Contact [support](mailto:admin@smartsync.cc) for payment/refund questions; see the [terms](https://smartsync.cc/terms/).

## Privacy and compatibility

Protected content and paths are encrypted on the device before upload. Account identity, vault/device labels, usage and other operational metadata are outside content encryption. Encryption does not replace backups or device security. Read the [privacy policy](https://smartsync.cc/privacy/) and [user guide](USER-GUIDE.md).

The Global client keeps diagnostic logs on the device; you can export them manually. It does not upload diagnostic telemetry. Device presence, local vault-size reports and peer discovery support your device-management and synchronization features. The service uses Oracle Cloud hosting, private Cloudflare R2 storage, Tencent QQ Mail for account emails, Stripe for payments and optional Google/GitHub identity providers. Server request logging is described in the privacy policy.

On Windows, explicitly enabling **Launch to tray at login** creates a shortcut in your current user's Startup folder outside the vault. Disable that option before uninstalling or reverting to a version without the feature. Other platforms hide this option. Desktop tray behavior uses the host's desktop APIs and safely falls back to normal closing when unavailable.

The plugin uses shared desktop and mobile controls. Mobile operating systems may suspend background synchronization; reopen Obsidian and confirm important changes finish uploading. Desktop-only capabilities are hidden or guarded on mobile. Fresh physical-device acceptance for this exact candidate remains incomplete; synthetic tests do not establish support on every device.

## Source and build

Development takes place only in [the canonical Client repository](https://github.com/adventurer2008/obsidian-smart-sync-client). `SOURCE-SNAPSHOT.json` identifies the exact exported commit and file hashes. Do not edit the generated runtime here. Server code, deployment tools and credentials are excluded.

Use Node 26.12.1, run `npm ci --ignore-scripts`, then `npm run build`. The build verifies the source snapshot and produces `main.js`, `manifest.json` and `styles.css`. Building locally does not install the plugin, publish a Release or pass official Community review. See [Community preparation](https://github.com/adventurer2008/obsidian-smart-sync-release-global/blob/main/COMMUNITY.md) for current gates.

Client source uses [Apache-2.0](LICENSE); dependency terms are in [THIRD-PARTY-NOTICES.md](THIRD-PARTY-NOTICES.md). A source license does not grant hosted-service access or rights to the private Server.

The fixed Client source and reproducible artifacts are bound to their recorded release checks. Physical-platform acceptance remains limited to its separate evidence; see [the review record](https://github.com/adventurer2008/obsidian-smart-sync-release-global/blob/main/COMMUNITY.md).