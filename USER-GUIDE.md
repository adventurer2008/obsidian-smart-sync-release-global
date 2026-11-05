# Smart Sync user guide

This guide applies to Smart Sync 1.1.5. Community listing approval and complete physical-device acceptance remain separate. Updates replace only main.js, manifest.json and styles.css; preserve existing per-device settings, secret storage, synchronization checkpoints and vault files.

## Install the review candidate

Use Obsidian1.12.7 or newer. Back up your vault and start with an isolated test vault. From the matching1.1.4 GitHub Release, download main.js, manifest.json and styles.css; verify them against SHA256SUMS.txt. Create a smart-sync-global folder inside your vault's configuration plugins folder (the default is .obsidian/plugins), and place all three files there. Reload Obsidian and enable Smart Sync in Community plugins after reviewing Obsidian's trust prompt yourself. Do not install a China package into this folder. Keep the previous plugin files for rollback and never overwrite your vault notes or plugin data.json to update the plugin.

## First connection

1. Back up your notes and use a separate test vault for the preview. Do not run multiple sync providers over the same vault without resolving their interactions.
2. Open the Smart Sync settings and select **Sign in**. Choose Google, GitHub or email. Social sign-in opens the provider in a browser; email verification stays in the plugin dialog.
3. Return to Obsidian after browser authorization. The account information should refresh automatically. If verification is interrupted or expires, reopen Sign in and follow its status message.
4. Create a cloud vault or select an existing one. Keep the encryption passphrase safe: signing in again cannot recover a forgotten encryption passphrase.
5. Review sync direction, attachment downloads, exclusions and configuration scope before synchronizing existing notes.
6. Run synchronization and review the task result. Important notes must finish uploading before closing or suspending the app.

Use the same account and select the same cloud vault on another device. Account identity, cloud-vault selection and local vault contents are separate; a matching vault name alone does not establish a matching cloud vault.

## Storage and purchase

Open the plan entry in plugin settings to view current capacity and purchase more storage. Mobile storage actions try to open the system browser directly; if the handoff cannot be confirmed, use the offered link. Check the current amount, currency and billing period on the payment page. Selecting a paid plan opens Stripe checkout directly. After paying, return to the app and verify the plan update. If the result is uncertain, inspect the existing order before paying again.

Free and paid plan limits are configured by the service and may differ. Current [plans](https://pay.smartsync.cc/pay/plans) and [terms](https://smartsync.cc/terms/) govern purchases. Contact [support](mailto:admin@smartsync.cc) for refund requests. Canceling renewal and deleting an account do not automatically refund a payment.

## Cloud-vault and account deletion

Cloud deletion is destructive. Keep a verified local backup first. Delete cloud vaults through vault management and wait for cleanup before selecting **Delete account** in the settings danger zone. Reverify the same account when prompted and enter the requested confirmation exactly. Paid service time does not prevent account deletion. Local notes are retained; account deletion is not a local-note eraser or a way to repair synchronization.

## Errors and device limits

Follow the displayed recovery action. After a lost creation reply, reopen the existing pending operation instead of creating another vault with a different name. Never send an encryption passphrase, login credential, emailed code or private note to support.

Mobile background and lock behavior depends on the operating system. Resume Obsidian, reconnect and inspect remaining tasks after interruption. Desktop tray/startup features are platform-specific and are not mobile background services. Physical-device acceptance remains bounded by the recorded device evidence; see [the preparation checklist](https://github.com/adventurer2008/obsidian-smart-sync-release-global/blob/main/COMMUNITY.md).