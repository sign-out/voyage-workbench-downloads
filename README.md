# Voyage Workbench downloads

Public downloads for the Voyage Workbench personal preview app.

## Download version 0.2.0

Open the [0.2.0 preview release](https://github.com/sign-out/voyage-workbench-downloads/releases/tag/v0.2.0) and choose:

| Platform | Asset |
| --- | --- |
| Android phones (ARM64; Android 13+) | `Voyage-Workbench-0.2.0-arm64.apk` |
| Android x86-64 devices/emulators | `Voyage-Workbench-0.2.0-x86_64.apk` |
| Android, both architectures | `Voyage-Workbench-0.2.0-universal.apk` |
| Windows x64 portable | `Voyage Workbench 0.2.0.exe` |
| Linux x64 | `Voyage-Workbench-0.2.0-linux-x64.tar.gz` |

For most Android phones, use the ARM64 APK. Allow installation from the source used to open it. Extract the entire Linux archive and launch `linux-unpacked/voyage-workbench`, keeping its resources together. Verify downloads with `SHA256SUMS-0.2.0.txt`.

## What to expect

Voyage API connections use **Alpha only**, not production or Beta. Voyage import and remote save supplement local saving. Your Voyage account/key must have Creator API access; the app cannot bypass server entitlement checks.

This preview includes Android large-world export fixes, shape-aware import review with per-change rejection, improved map navigation and character editing, and mobile layout fixes.

Windows is unsigned. Android APKs are non-debuggable release builds signed with a development certificate, not store releases. Physical ARM64 devices and native Windows execution have not been certified. Provider use requires appropriate credentials and platform support; not every live provider/account has been qualified.

This repository contains release downloads and documentation, not credentials, private worlds, local projects, signing keys or account login state. Third-party runtime notices and source material accompany the release. This is an independent workbench, not an official Voyage release.
