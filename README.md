# Darktable Spektrafilm — Builds

 Automated builds from the [spektrafilm-draft](https://github.com/Arecsu/darktable/tree/spektrafilm-draft) branch.

Come work together! Feedback, issues, anything is welcome at [discuss.pixls.us](https://discuss.pixls.us/t/spektrafilm-darktable-module-implementation-discussion/58744)

> **⚠️ HIGHLY EXPERIMENTAL** — back up your darktable data dir before testing: Linux `~/.config/darktable/`, macOS `~/Library/Application Support/darktable/`, Windows `%APPDATA%\darktable\`. Use `--library <path>` to keep your main setup safe.

**Latest version:** 20260804-f95c05e

## Latest Builds

| Platform | Architecture | Download |
|----------|-------------|----------|
| Linux AppImage | x86_64 | [darktable-spektrafilm-20260804-f95c05e-x86_64.AppImage](https://github.com/Arecsu/dt-spektrafilm-builds/releases/download/spektrafilm-builds/darktable-spektrafilm-20260804-f95c05e-x86_64.AppImage) |
| Linux AppImage | ARM64 | [darktable-spektrafilm-20260804-f95c05e-aarch64.AppImage](https://github.com/Arecsu/dt-spektrafilm-builds/releases/download/spektrafilm-builds/darktable-spektrafilm-20260804-f95c05e-aarch64.AppImage) |
| Windows | x86_64 | [darktable-spektrafilm-20260804-f95c05e-x86_64.exe](https://github.com/Arecsu/dt-spektrafilm-builds/releases/download/spektrafilm-builds/darktable-spektrafilm-20260804-f95c05e-x86_64.exe) |
| macOS | ARM64 (Apple Silicon) | [darktable-spektrafilm-20260804-f95c05e-arm64.dmg](https://github.com/Arecsu/dt-spektrafilm-builds/releases/download/spektrafilm-builds/darktable-spektrafilm-20260804-f95c05e-arm64.dmg) |
| macOS | x86_64 (Intel) | [darktable-spektrafilm-20260804-f95c05e-x86_64.dmg](https://github.com/Arecsu/dt-spektrafilm-builds/releases/download/spektrafilm-builds/darktable-spektrafilm-20260804-f95c05e-x86_64.dmg) |

## Recent Commits

| Date | Commit | Author | Message |
|------|--------|--------|---------|
| 2026-08-04 | [f95c05e](https://github.com/Arecsu/darktable/commit/f95c05e) | piratenpanda | fix opencl for more than one opencl runtime |
| 2026-08-04 | [ec8d3b7](https://github.com/Arecsu/darktable/commit/ec8d3b7) | piratenpanda | add surface adaptation code |
| 2026-08-03 | [59c2dee](https://github.com/Arecsu/darktable/commit/59c2dee) | piratenpanda | support pack v2 files, fix Tri-X column layout to follow upstream spektrafilM |
| 2026-08-03 | [4631a17](https://github.com/Arecsu/darktable/commit/4631a17) | piratenpanda | move to inline labels again for film, paper and format. Soft limit preflash range to 0.5 |

## Data pack

If you are upgrading from an older build, delete the `spektrafilm` folder from your darktable config directory first, so the module doesn't keep using outdated data:

| Platform | Folder to delete |
|----------|------------------|
| Linux | `~/.config/darktable/spektrafilm/` |
| macOS | `~/Library/Application Support/darktable/spektrafilm/` |
| macOS | `~/.config/darktable/spektrafilm/` |
| Windows | `%APPDATA%\darktable\spektrafilm\` |

Then:

1. Enable **Preferences → Security → "allow spektrafilm to download data packs"**.
2. **Restart darktable** — the setting only takes effect after a restart.
3. Open the spektrafilm module on a photo. If a data pack is missing, a **"download data pack"** button appears — click it and the module downloads the data pack it needs, verifying the download before it's used.
