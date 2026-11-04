# Community preparation

Change: CHG-20261104-GITHUB-COMMUNITY-PREP. Status: source preview and listing draft only; no submission or installable Global Release.

## Listing draft

Name: Smart Sync

ID: smart-sync-global

Repository: adventurer2008/obsidian-smart-sync-release-global

Short description:

Sync notes and attachments with client-side encryption and hosted cloud storage. Includes sorting, pinned notes and recent files.

Long description:

Sync notes, attachments and selected settings through an independent hosted service. Protected content and paths are encrypted on your device before upload; account and operational metadata are outside that protection. Includes version recovery, device management, sorting, pinned notes and recent files. An account is required for hosted sync, with Google, GitHub or email sign-in. A free storage tier is available; larger storage uses paid Stripe subscriptions. Keep your encryption passphrase safe. Mobile background execution depends on the operating system.

Payments: optional. Free hosted storage is available; paid subscriptions provide additional capacity. Confirm the platform's current payment fields when submitting.

Homepage: https://smartsync.cc/

Privacy: https://smartsync.cc/privacy/

Terms: https://smartsync.cc/terms/

Support: admin@smartsync.cc

## Completed preparation

- Fixed public Client source is identified by SOURCE-SNAPSHOT.json with previewOnly=true; no private Server/history/tools are exported.
- Canonical pinned Node26 tests: Windows335 passed; WSL334 passed, one Windows-only NTFS stream check skipped.
- Both canonical regional builds and dependency closure passed. Global local Community lint: zero errors and12 warnings. Warnings cover fetch usage, window timers and a config-path reference; these remain review items.
- English guide, account/payment disclosures and legal links are prepared. All-platform acceptance and official review are not inferred from source publication.

## Remaining release/submission gates

- Freeze the exact version, Client/Server pairing and generated artifact hashes for public delivery. The preview version is not a published release.
- Complete the required staged/production acceptance for that complete source. Earlier scoped portal/runtime deployments do not prove the complete new Client/Server pair, particularly the source-only regional account changes.
- Review the12 lint warnings and verify their platform behavior. Local lint success is not official scan approval.
- Record real-host install/upgrade, browser return, secure storage, touch/narrow layouts, background/lock/restart, offline recovery and mixed-device body/source-mtime acceptance. Windows, macOS, Linux desktop, Android, iPhone and iPad require independent evidence; absent cases remain unverified.
- Publish matching three-file assets only after release gates pass. Preserve historical tags and artifacts.
- Submit the repository and listing through the official Community workflow afterward; review status must be read from the platform.

## Verified snapshot

Canonical Client commit: c1533adb3cab40637b9e1618ae731771402a6ce7. Preview version:1.1.4, minimum Obsidian1.12.7. The version identifies source preparation and is not a released installation recommendation.

Two Windows Node26.12.1 snapshot builds produced identical artifacts, matching the canonical Global build byte for byte. The exported complete Windows suite with explicit local Server pairing passed335 tests with zero failures/skips. These are local synthetic/build results; no hosted-service or native-device acceptance is implied.

| Artifact | SHA-256 |
| --- | --- |
| main.js | 64a9abbefa8b82ed14127062969644c6afb2dd3f5435f853aa38c7ab275e2a7d |
| manifest.json | 926cb2b550156edd54eba4f6f84f155d5d8828a342ecf85bc92feb2c3127e058 |
| styles.css | 5c79e29c861f843d51d6de41d3c740d93905131c6495e4754777ac7cfa725b0b |

No live payment was performed to prepare these materials. Generated main.js remains an ignored local build output until a separately gated binary Release.
