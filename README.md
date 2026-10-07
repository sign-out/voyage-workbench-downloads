# Voyage Workbench downloads

Public downloads for the Voyage Workbench personal preview app.

## Download version 0.2.1

Open the [0.2.1 preview release](https://github.com/sign-out/voyage-workbench-downloads/releases/tag/v0.2.1) and choose:

| Platform | Asset |
| --- | --- |
| Android phones (ARM64; Android 13+) | `Voyage-Workbench-0.2.1-arm64.apk` |
| Android x86-64 devices/emulators | `Voyage-Workbench-0.2.1-x86_64.apk` |
| Android, both architectures | `Voyage-Workbench-0.2.1-universal.apk` |
| Windows x64 portable | `Voyage-Workbench-0.2.1-windows-x64.exe` |
| Linux x64 | `Voyage-Workbench-0.2.1-linux-x64.tar.gz` |

For most Android phones, use the ARM64 APK. Allow installation from the source used to open it. Extract the entire Linux archive and launch `linux-unpacked/voyage-workbench`, keeping its resources together. Verify downloads with `SHA256SUMS-0.2.1.txt`.

## What to expect

Voyage API connections use **Alpha only**, not production or Beta. Voyage import and remote save supplement local saving. Your Voyage account/key must have Creator API access; the app cannot bypass server entitlement checks.

Version 0.2.1 fixes Voyage saves rejected with `400 invalid_revision`: both hosts convert Alpha's weak ETag into the quoted revision required by its save endpoint. An unchanged live Alpha draft was saved successfully and confirmed by read-back. The release also retains the Android large-world export fix, selective import review and UI/navigation improvements.

Install the updated Android APK over the existing app to retain local projects. Then select **Save to Voyage API** again; the previous explicit `invalid_revision` rejection is cleared safely. Actual uncertain network writes still require reconciliation, and conflicting newer remote drafts are not overwritten automatically.

Windows is unsigned. Android APKs are non-debuggable release builds signed with a development certificate, not store releases. Physical ARM64 devices and native Windows execution have not been certified. Provider use requires appropriate credentials and platform support; not every live provider/account has been qualified.

This repository contains release downloads and documentation, not credentials, private worlds, local projects, signing keys or account login state. Third-party runtime notices and source material accompany the release. This is an independent workbench, not an official Voyage release.
