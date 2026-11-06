# Smart Sync 1.1.5

- Prevent repeated Danger zone controls and stale section headings when settings refresh after account changes.
- Keep account and device action labels readable on narrow screens with enlarged interface text.
- Recover automatic browser sign-in checks after temporary network failures or returning to Obsidian. Keep manual checks and same-account verification.
- Recover interrupted account creation and deletion flows with bounded retries and clear, localized guidance; preserve confirmation and account/vault isolation.
- Open the storage-plan browser directly on mobile when a valid account-bound entry is ready, with a conditional native-link fallback for uncertain or failed handoffs.
- Include the maintained synchronization, original source-mtime preservation, encryption, device management and local tools without removing their existing controls.

The associated Global service update retains the current hosted plan/checkout interface. Update only main.js, manifest.json and styles.css; preserve per-device data.json, secret storage, checkpoints and all vault files. Keep an independent backup and inspect current tasks before closing a device.
