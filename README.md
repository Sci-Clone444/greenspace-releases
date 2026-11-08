# Greenspace OS releases

Release builds and update manifests for Greenspace OS, a greenhouse / grow-facility controller.

This repository holds **only built, signed release files**, no source code. Installed Greenspace OS
systems read the update manifest from here to find out whether a newer version is available, then
download the release file from this repository's GitHub Releases.

## What is here

- **GitHub Releases** (`v<major>.<minor>.<patch>`): the release files of each version (application,
  later the Windows installer), their signatures and release notes.
- **Update manifests** (added with the first release): one per release channel (e.g. `stable`, `beta`),
  naming the newest version, its download link, checksum and signature.

Every release file is signed; an installed system refuses an update whose signature doesn't check out.

## Installing or updating

Installed systems update themselves from the dashboard. To install Greenspace OS on a new machine,
use the installer from the newest release.
