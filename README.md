# Voyage Workbench downloads

Public downloads for the Voyage Workbench personal preview app.

## Download version 0.2.2

Open the [0.2.2 preview release](https://github.com/sign-out/voyage-workbench-downloads/releases/tag/v0.2.2) and choose:

| Platform | Asset |
| --- | --- |
| Android phones (ARM64; Android 13+) | `Voyage-Workbench-0.2.2-arm64.apk` |
| Android x86-64 devices/emulators | `Voyage-Workbench-0.2.2-x86_64.apk` |
| Android, both architectures | `Voyage-Workbench-0.2.2-universal.apk` |
| Windows x64 portable | `Voyage-Workbench-0.2.2-windows-x64.exe` |
| Linux x64 | `Voyage-Workbench-0.2.2-linux-x64.tar.gz` |

For most Android phones, use the ARM64 APK. Allow installation from the source used to open it. Extract the entire Linux archive and launch `linux-unpacked/voyage-workbench`, keeping its resources together. Verify downloads with `SHA256SUMS-0.2.2.txt`.

## What to expect

Voyage API connections use **Alpha only**, not production or Beta. Voyage import and remote save supplement local saving. Your Voyage account/key must have Creator API access; the app cannot bypass server entitlement checks.

Version 0.2.2 fixes false unconfirmed saves caused by server JSON key reordering. Confirmation compares actual values while preserving exact large-number distinctions and array ordering. Remote status feedback separates confirmed success, pending checks, genuine mismatches with differing paths, rejections and failures. The weak ETag fix, Android export fix, selective import review and UI/navigation improvements are retained.

Install the updated Android APK over the existing app to retain local projects. **Save to Voyage API** automatically checks an earlier pending attempt. If the current local version is already confirmed remotely, it reports success without another upload. If an older write is confirmed and newer local edits exist, it can proceed with a conditional save using the confirmed revision. Real differences and failed checks block further uploads; conflicting remote drafts are not overwritten automatically. **Reconcile save** is also available as an explicit read-only check.

Windows is unsigned. Android APKs are non-debuggable release builds signed with a development certificate, not store releases. Physical ARM64 devices and native Windows execution have not been certified. Provider use requires appropriate credentials and platform support; not every live provider/account has been qualified.

This repository contains release downloads and documentation, not credentials, private worlds, local projects, signing keys or account login state. Third-party runtime notices and source material accompany the release. This is an independent workbench, not an official Voyage release.
