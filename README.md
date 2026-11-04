# Smart Sync

Sync notes, attachments and selected settings with client-side encryption. Keep original file modification times, manage devices and recover earlier versions. Additional local tools include sorting, pinned notes, recent files and password-protected note content.

Plugin ID: `smart-sync-global`. This repository contains a generated source preview for Community preparation. No installable Global Release has been published here. The preview is not a stable-release recommendation.

## Account and payments

An account is required for hosted synchronization. Sign in with Google, GitHub or an emailed code. A free storage tier is available; additional storage is a paid subscription. See current [plans](https://pay.smartsync.cc/pay/plans) before purchase. Stripe handles checkout and recurring subscriptions. Account sign-in does not replace the encryption passphrase; keep that passphrase safe.

To delete an account, first delete its cloud vaults and wait for cleanup. The plugin then requires identity verification and confirmation. Account deletion does not automatically refund payments. Contact [support](mailto:admin@smartsync.cc) for payment/refund questions; see the [terms](https://smartsync.cc/terms/).

## Privacy and compatibility

Protected content and paths are encrypted on the device before upload. Account identity, vault/device labels, usage and other operational metadata are outside content encryption. Encryption does not replace backups or device security. Read the [privacy policy](https://smartsync.cc/privacy/) and [user guide](USER-GUIDE.md).

The plugin uses shared desktop and mobile controls. Mobile operating systems may suspend background synchronization; reopen Obsidian and confirm important changes finish uploading. Desktop-only capabilities are hidden or guarded on mobile. Fresh physical-device acceptance for this exact candidate remains incomplete; synthetic tests do not establish support on every device.

## Source and build

Development takes place only in [the canonical Client repository](https://github.com/adventurer2008/obsidian-smart-sync-client). `SOURCE-SNAPSHOT.json` identifies the exact exported commit and file hashes. Do not edit the generated runtime here. Server code, deployment tools and credentials are excluded.

Use Node 26.12.1, run `npm ci --ignore-scripts`, then `npm run build`. The build verifies the source snapshot and produces `main.js`, `manifest.json` and `styles.css`. Building locally does not install the plugin, publish a Release or pass official Community review. See [Community preparation](COMMUNITY.md) for current gates.

Client source uses [Apache-2.0](LICENSE); dependency terms are in [THIRD-PARTY-NOTICES.md](THIRD-PARTY-NOTICES.md). A source license does not grant hosted-service access or rights to the private Server.

CHG-20261104-GITHUB-COMMUNITY-PREP: replace the original placeholder with a fixed public Client source preview and review materials; no tag, binary Release or listing submission.
