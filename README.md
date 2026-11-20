# Server Security Center (SSC) – Downloads & Updates

This repository holds the installers and automatic updates of the **Server Security Center (SSC)**. The source code is private.

## Download

Latest version: **[Releases → Latest](https://github.com/smaramwbc/ssc-releases/releases/latest)**

| Platform | File |
|---|---|
| macOS 11 or later (Apple Silicon + Intel) | `SSC_<version>_macOS.dmg` |
| Windows 10/11 (x64) | `SSC_<version>_Windows-x64-setup.exe` |
| Ubuntu 22.04 / 24.04 (x86_64) | `SSC_<version>_Linux-amd64.deb` |

Checksums are in each release's `SHA256SUMS` file.

## Installation

- **macOS:** open the DMG and drag the app to *Applications*. The app is not notarized by Apple, so the first start is blocked. Then click **“Open Anyway”** in *System Settings → Privacy & Security*.
- **Windows:** run the installer.
- **Ubuntu:** `sudo apt install ./SSC_<version>_Linux-amd64.deb`

## Updates

Installed apps update themselves (*Settings → Updates*). The update source is:

```
https://github.com/smaramwbc/ssc-releases/releases/latest/download/latest.json
```

An update is only installed if the package is signed with the app's release key and the signature matches the announced version.
