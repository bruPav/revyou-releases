# revyou-releases

Public download host for **Revyou** builds. This repository contains **no
source code** — only the workflow that builds the private source and the
compiled binaries published as releases.

## Download

Grab the latest build from the [latest release](../../releases/latest):

| Platform | File |
|---|---|
| Linux | `revyou-linux-x86_64.tar.gz` |
| Windows | `revyou-windows-x86_64.zip` |
| macOS (Intel + Apple Silicon) | `revyou-macos-universal.dmg` |

Direct links:

- https://github.com/bruPav/revyou-releases/releases/latest/download/revyou-linux-x86_64.tar.gz
- https://github.com/bruPav/revyou-releases/releases/latest/download/revyou-windows-x86_64.zip
- https://github.com/bruPav/revyou-releases/releases/latest/download/revyou-macos-universal.dmg

The Linux and Windows builds are portable folders (unzip and run). The macOS
build is unsigned: first launch needs right-click → **Open**.

## How builds run

`.github/workflows/build.yml` builds three platforms from
`bruPav/Revyou` (private) using the `REVYOU_PAT` secret, then publishes the
artifacts to the `latest` release.

To trigger: **Actions → Build → Run workflow** (optionally set a branch/tag).
