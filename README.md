# Darktable Spektrafilm — Builds

 Automated builds from the [spektrafilm-draft](https://github.com/piratenpanda/darktable/tree/spektrafilm) branch.

Come work together! Feedback, issues, anything is welcome at [discuss.pixls.us](https://discuss.pixls.us/t/spektrafilm-darktable-module-implementation-discussion/58744)

> **⚠️ HIGHLY EXPERIMENTAL** — back up your darktable data dir before testing: Linux `~/.config/darktable/`, macOS `~/Library/Application Support/darktable/`, Windows `%APPDATA%\darktable\`. Use `--library <path>` to keep your main setup safe.

**Latest version:** 20260822-5b58ac6

## Latest Builds

| Platform | Architecture | Download |
|----------|-------------|----------|
| Linux AppImage | x86_64 | [darktable-spektrafilm-20260822-5b58ac6-x86_64.AppImage](https://github.com/piratenpanda/dt-spektrafilm-builds/releases/download/spektrafilm-builds/darktable-spektrafilm-20260822-5b58ac6-x86_64.AppImage) |
| Linux AppImage | ARM64 | [darktable-spektrafilm-20260822-5b58ac6-aarch64.AppImage](https://github.com/piratenpanda/dt-spektrafilm-builds/releases/download/spektrafilm-builds/darktable-spektrafilm-20260822-5b58ac6-aarch64.AppImage) |
| Windows | x86_64 | [darktable-spektrafilm-20260822-5b58ac6-x86_64.exe](https://github.com/piratenpanda/dt-spektrafilm-builds/releases/download/spektrafilm-builds/darktable-spektrafilm-20260822-5b58ac6-x86_64.exe) |
| macOS | ARM64 (Apple Silicon) | [darktable-spektrafilm-20260822-5b58ac6-arm64.dmg](https://github.com/piratenpanda/dt-spektrafilm-builds/releases/download/spektrafilm-builds/darktable-spektrafilm-20260822-5b58ac6-arm64.dmg) |
| macOS | x86_64 (Intel) | [darktable-spektrafilm-20260822-5b58ac6-x86_64.dmg](https://github.com/piratenpanda/dt-spektrafilm-builds/releases/download/spektrafilm-builds/darktable-spektrafilm-20260822-5b58ac6-x86_64.dmg) |

## Recent Commits

| Date | Commit | Author | Message |
|------|--------|--------|---------|
| 2026-08-22 | [5b58ac6db](https://github.com/piratenpanda/darktable/commit/5b58ac6db) | piratenpanda | add a post-compression scale beside the pre-compression boost |
| 2026-08-22 | [695a510c6](https://github.com/piratenpanda/darktable/commit/695a510c6) | piratenpanda | aim the pre-compression boost picker slightly higher |
| 2026-08-22 | [305872c1e](https://github.com/piratenpanda/darktable/commit/305872c1e) | piratenpanda | lead the download line with the percentage |
| 2026-08-22 | [5bf47ac04](https://github.com/piratenpanda/darktable/commit/5bf47ac04) | piratenpanda | let the pack-contents test fail instead of skipping |

## Data pack

If you are upgrading from an older build, delete the `spektrafilm` folder from your darktable config directory first.
