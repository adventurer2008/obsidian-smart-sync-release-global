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

The official submission form is prepared. Developer Policies agreement and the continued-maintenance commitment have not yet been accepted. No Community submission or approval is claimed by this preparation record; final platform status must be read from the official directory.

## Acceptance boundaries

Fresh physical acceptance on Windows, macOS, Linux desktop, Android, iPhone/iOS and iPad/iPadOS remains incomplete for this exact candidate. Prior Windows user testing applies to its earlier installed bundle. Native install/upgrade, secure storage, browser return, narrow/touch layouts, background/lock/restart, offline recovery and mixed-device source-mtime behavior need separate device evidence. Unsupported native controls remain hidden or guarded.

No real Live card payment was made for this candidate. Production checkout uses real Stripe payments; staging uses test mode. Client publication and Community review do not certify the service or all platforms.
