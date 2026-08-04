# Darktable Spektrafilm — Builds

 Automated builds from the [spektrafilm-draft](https://github.com/Arecsu/darktable/tree/spektrafilm-draft) branch.

Come work together! Feedback, issues, anything is welcome at [discuss.pixls.us](https://discuss.pixls.us/t/spektrafilm-darktable-module-implementation-discussion/58744)

> **⚠️ HIGHLY EXPERIMENTAL** — back up your darktable data dir before testing: Linux `~/.config/darktable/`, macOS `~/Library/Application Support/darktable/`, Windows `%APPDATA%\darktable\`. Use `--library <path>` to keep your main setup safe.

**Latest version:** 20260804-4628378

## Latest Builds

| Platform | Architecture | Download |
|----------|-------------|----------|
| Linux AppImage | x86_64 | [darktable-spektrafilm-20260804-4628378-x86_64.AppImage](https://github.com/Arecsu/dt-spektrafilm-builds/releases/download/spektrafilm-builds/darktable-spektrafilm-20260804-4628378-x86_64.AppImage) |
| Linux AppImage | ARM64 | [darktable-spektrafilm-20260804-4628378-aarch64.AppImage](https://github.com/Arecsu/dt-spektrafilm-builds/releases/download/spektrafilm-builds/darktable-spektrafilm-20260804-4628378-aarch64.AppImage) |
| Windows | x86_64 | [darktable-spektrafilm-20260804-4628378-x86_64.exe](https://github.com/Arecsu/dt-spektrafilm-builds/releases/download/spektrafilm-builds/darktable-spektrafilm-20260804-4628378-x86_64.exe) |
| macOS | ARM64 (Apple Silicon) | [darktable-spektrafilm-20260804-4628378-arm64.dmg](https://github.com/Arecsu/dt-spektrafilm-builds/releases/download/spektrafilm-builds/darktable-spektrafilm-20260804-4628378-arm64.dmg) |
| macOS | x86_64 (Intel) | [darktable-spektrafilm-20260804-4628378-x86_64.dmg](https://github.com/Arecsu/dt-spektrafilm-builds/releases/download/spektrafilm-builds/darktable-spektrafilm-20260804-4628378-x86_64.dmg) |

## Recent Commits

| Date | Commit | Author | Message |
|------|--------|--------|---------|
| 2026-08-03 | [4628378](https://github.com/Arecsu/darktable/commit/4628378) | piratenpanda | support pack v2 files, fix Tri-X column layout to follow upstream spektrafilM |
| 2026-08-03 | [1701fa1](https://github.com/Arecsu/darktable/commit/1701fa1) | piratenpanda | move to inline labels again for film, paper and format. Soft limit preflash range to 0.5 |
| 2026-08-02 | [d8e77c5](https://github.com/Arecsu/darktable/commit/d8e77c5) | piratenpanda | add format header |
| 2026-08-02 | [ac54937](https://github.com/Arecsu/darktable/commit/ac54937) | piratenpanda | clarify tool tips on user feedback |

## Data pack

The module downloads the spectral data pack it needs automatically. First enable **Preferences → Security → "allow spektrafilm to download data packs"**, then open the spektrafilm module on an image and click **"download data pack"** when it appears. Every file is verified against a checksum from the repository manifest before install, and downloaded packs are written to the `spektrafilm/packs` subfolder of your darktable config directory, so they are backed up with the rest of your configuration.
