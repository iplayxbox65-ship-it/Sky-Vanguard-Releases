# Sky Vanguard Releases

<p align="center">
  <strong>Official public release repository for Sky Vanguard.</strong><br>
  Windows installers, updater metadata, and player-facing release notes published by Skytrace Studios.
</p>

<p align="center">
  <img alt="Current Version" src="https://img.shields.io/badge/current-1.2.11-blue?style=for-the-badge">
  <img alt="Platform" src="https://img.shields.io/badge/platform-Windows-lightgrey?style=for-the-badge">
  <img alt="Release Channel" src="https://img.shields.io/badge/channel-public%20release-success?style=for-the-badge">
</p>

---

## Overview

This repository is the public distribution point for **Sky Vanguard** builds. It contains the files required for players and update systems to retrieve the latest Windows release.

The private source code, development tools, and internal project files are kept separately in `Sky-Vanguard-DEV`.

---

## Latest release

| Field | Value |
| --- | --- |
| Current version | `1.2.11` |
| Installer | `Sky Vanguard-Setup-1.2.11.exe` |
| Manifest | `latest.json` |
| Published | `2026-05-20` |

Release metadata is maintained in [`latest.json`](./latest.json). The manifest is the source of truth for the current public build, installer filename, download URL, checksum, publish date, and release notes.

---

## Repository structure

```text
Sky-Vanguard-Releases/
├── artifacts/
│   └── <version>/
│       └── Sky Vanguard-Setup-<version>.exe
├── latest.json
└── README.md
```

| Path | Purpose |
| --- | --- |
| `artifacts/<version>/` | Stores installer files for each published version. |
| `latest.json` | Provides updater metadata for the newest public release. |
| `README.md` | Explains the release repository and distribution layout. |

---

## Installation

1. Open the latest release artifact listed in `latest.json`.
2. Download the Windows installer.
3. Run the installer and follow the setup prompts.
4. Launch Sky Vanguard after installation completes.

For safety, only download builds from this repository or links controlled by Skytrace Studios.

---

## Update metadata

`latest.json` follows this format:

```json
{
  "version": "1.2.11",
  "installerName": "Sky Vanguard-Setup-1.2.11.exe",
  "installerUrl": "https://...",
  "sha256": "...",
  "publishedAt": "2026-05-20T13:27:09.275Z",
  "notes": "Release notes for this version."
}
```

Applications, launchers, or update checkers should read `latest.json` instead of hardcoding version numbers.

---

## Verification

Each release manifest includes a SHA-256 checksum for the installer. This allows the downloaded file to be checked against the expected build hash before installation or update processing.

Current SHA-256:

```text
953DC0337774D57FD35FBB33AF6B84477CFA3A65FA2CEDA16BF68DB25214432A
```

---

## Notes for players

- This repository is for official release files only.
- Development builds are not published here.
- Source code is not included in this repository.
- Older release artifacts may remain available for reference or rollback support.

---

## Maintainer

Published by **Skytrace Studios**.

Repository maintained by **0wenDevelops**.
