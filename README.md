# Sky Vanguard Releases

Official public release repository for Sky Vanguard, published by Skytrace Studios.

This repository contains Windows installers, updater metadata, and release notes for official player-facing builds.

Private source code and development tooling remain in the separate repository `Sky-Vanguard-DEV`.

## Repository contents

- Windows installer artifacts
- updater manifest files
- public release notes

## Release layout

- `artifacts/<version>/` contains installer assets for each published version
- `latest.json` describes the newest version for updater checks

## Version info

Current release details live in `latest.json` to avoid duplicate version strings drifting out of sync.
