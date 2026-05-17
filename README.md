# Sky Vanguard Releases

Public distribution repository for Sky Vanguard player downloads and updater metadata.

This repository is intended to contain:

- Windows installer artifacts
- updater manifest files
- public release notes

Private source code and development files live in the separate repository `Sky-Vanguard-DEV`.

## Current layout

- `artifacts/<version>/` contains installer assets for a released version
- `latest.json` describes the newest version for updater checks

## Current version

- `1.2.2`

## Notes

The long-term updater flow can move installer binaries to GitHub Release assets if you want cleaner downloads later. For now, this repo is set up to hold the public installer files and release metadata in one place.
