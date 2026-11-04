# Community review record

Change: CHG-20261104-GLOBAL-COMMUNITY-SUBMIT.

Name: Smart Sync. ID: smart-sync-global. Repository: adventurer2008/obsidian-smart-sync-release-global.

Description: Sync notes and attachments with client-side encryption and hosted cloud storage. Includes sorting, pinned notes and recent files.

Homepage: https://smartsync.cc/ · Privacy: https://smartsync.cc/privacy/ · Terms: https://smartsync.cc/terms/ · Support: admin@smartsync.cc.

An account is required for hosted sync. A Free plan is available; optional paid storage uses Stripe subscriptions. The README discloses network services, metadata, local diagnostics and the optional Windows Startup shortcut outside the vault. Global automatic diagnostic telemetry is disabled. No self-install/update mechanism is used.

## Fixed candidate

Version:1.1.4. Minimum Obsidian:1.12.7. Canonical Client:b9e7504a85e3853cbece3a749dcdc8328cfab50e.

Candidate digest:e4315743e838c24742e471613962c9ed2bc51e5d9f2fb2fc784a2999ddbd358c.

SOURCE-SNAPSHOT.json binds generated public source and accepted artifact hashes. Two snapshot builds match byte for byte and match the canonical Global build. SHA256SUMS.txt lists the three plugin artifacts. No private Server source, deployment scripts, credentials or historical private files are exported.

The exported complete Windows Node26.12.1 suite passed338 tests, zero failed/skipped. WSL passed337, zero failed, one Windows-only NTFS-stream check skipped. A prior Windows run of the preceding candidate intermittently failed an attachment-relative-order assertion; focused and complete reruns passed, and the observation remains recorded in the canonical validation report. WSL is not native Linux acceptance.

The exact Client protocol/codec completed synthetic encrypted writes and reads over HTTPS against both staging and production. Plaintext and original source mtime matched. Both owned synthetic vaults reached complete erasure with zero pending objects. All155 files in the frozen service runtime were hash-verified. Separate environments and configured Google/GitHub/email methods were checked. These checks do not replace real user sign-in, payment or native-host acceptance.

## Local lint and official review

Global local lint reports zero errors and seven reviewed warnings. Six fetch references preserve cancellation, bounded streaming and redirect rejection that a mechanical requestUrl substitution would lose. The .obsidian literal is a reserved-path rejection guard, not host configuration access. Five window-timer warnings were fixed. No lint rule is suppressed. Local results are not official scan approval.

The user completed the initial submission form and its commitments. The listing was then saved with account/service disclosures and Optional payment details, and Publish completed. Official dashboard: "Your entry is live. An automated review is in progress." The queued1.1.4 review points at distribution commit8d88ef6f11892519b409a2928f31da8e5da222c2. Status:Pending, not approved.

Community entry: https://community.obsidian.md/plugins/smart-sync-global

GitHub Release: https://github.com/adventurer2008/obsidian-smart-sync-release-global/releases/tag/1.1.4

All11 public Release attachments were downloaded anonymously and hash-verified. The tag resolves to the fixed distribution commit. The initial Community refresh encountered a short cooldown and an older no-release cache; a later supported refresh recognized1.1.4 and queued its scan. No new version or duplicate entry was created to bypass the cooldown.

Partial official results observed while Pending: dependency vulnerability check passes; recommendations cover artifact attestations, extra documentation attachments, vault enumeration and clipboard access. CSS warnings cover display:contents compatibility and one !important declaration. The platform explicitly says results are incomplete and more checks are running. These findings are not represented as completed approval; no existing Release assets were removed or overwritten to silence recommendations.

## Acceptance boundaries

Fresh physical acceptance on Windows, macOS, Linux desktop, Android, iPhone/iOS and iPad/iPadOS remains incomplete for this exact candidate. Prior Windows user testing applies to its earlier installed bundle. Native install/upgrade, secure storage, browser return, narrow/touch layouts, background/lock/restart, offline recovery and mixed-device source-mtime behavior need separate device evidence. Unsupported native controls remain hidden or guarded.

No real Live card payment was made for this candidate. Production checkout uses real Stripe payments; staging uses test mode. Client publication and Community review do not certify the service or all platforms.
