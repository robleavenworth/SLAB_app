# SLAB App

Update distribution for [SLAB](https://github.com/robleavenworth/SLAB) (Structured Library for Assessment Batteries).

This repo serves two purposes:

1. **Version checking** -- The app fetches `version.json` from GitHub Pages on launch to check for updates. If a newer version is available, users see a banner with a download link.
2. **Release hosting** -- New builds of `SLAB.html` are attached as GitHub Release assets for download.

## Releasing an update

1. Build `SLAB.html` from the [private repo](https://github.com/robleavenworth/SLAB).
2. Create a new GitHub Release on this repo and attach `SLAB.html` as an asset.
3. Update `version.json` with the new version number and push to `main`.

Users running older versions will see the update banner on their next launch.

## Files

| File | Purpose |
|------|---------|
| `version.json` | Served via GitHub Pages. Contains `version` (latest version string) and `url` (download link for the latest release asset). |
| `SLAB.html` | The built app file, kept here for convenience. Not served directly; users download it from GitHub Releases. |
