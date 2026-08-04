# Darktable Spektrafilm — Builds

 Automated builds from the [spektrafilm-draft](https://github.com/Arecsu/darktable/tree/spektrafilm-draft) branch.

Come work together! Feedback, issues, anything is welcome at [discuss.pixls.us](https://discuss.pixls.us/t/spektrafilm-darktable-module-implementation-discussion/58744)

> **⚠️ HIGHLY EXPERIMENTAL** — back up your darktable data dir before testing: Linux `~/.config/darktable/`, macOS `~/Library/Application Support/darktable/`, Windows `%APPDATA%\darktable\`. Use `--library <path>` to keep your main setup safe.

**Latest version:** 20260801-27b5243

## Latest Builds

| Platform | Architecture | Download |
|----------|-------------|----------|
| Linux AppImage | x86_64 | [darktable-spektrafilm-20260801-27b5243-x86_64.AppImage](https://github.com/Arecsu/dt-spektrafilm-builds/releases/download/spektrafilm-builds/darktable-spektrafilm-20260801-27b5243-x86_64.AppImage) |
| Linux AppImage | ARM64 | [darktable-spektrafilm-20260801-27b5243-aarch64.AppImage](https://github.com/Arecsu/dt-spektrafilm-builds/releases/download/spektrafilm-builds/darktable-spektrafilm-20260801-27b5243-aarch64.AppImage) |
| Windows | x86_64 | [darktable-spektrafilm-20260801-27b5243-x86_64.exe](https://github.com/Arecsu/dt-spektrafilm-builds/releases/download/spektrafilm-builds/darktable-spektrafilm-20260801-27b5243-x86_64.exe) |
| macOS | ARM64 (Apple Silicon) | [darktable-spektrafilm-20260801-27b5243-arm64.dmg](https://github.com/Arecsu/dt-spektrafilm-builds/releases/download/spektrafilm-builds/darktable-spektrafilm-20260801-27b5243-arm64.dmg) |
| macOS | x86_64 (Intel) | [darktable-spektrafilm-20260801-27b5243-x86_64.dmg](https://github.com/Arecsu/dt-spektrafilm-builds/releases/download/spektrafilm-builds/darktable-spektrafilm-20260801-27b5243-x86_64.dmg) |

## Recent Commits

| Date | Commit | Author | Message |
|------|--------|--------|---------|
| 2026-08-01 | [27b5243](https://github.com/Arecsu/darktable/commit/27b5243) | Arecsu | spektrafilm: run grain USM on absolute density to match reference |
| 2026-08-01 | [f58985b](https://github.com/Arecsu/darktable/commit/f58985b) | piratenpanda | blur whole grained desity field and not only delta to match reference and avoid oversharpening |
| 2026-07-29 | [194f9e1](https://github.com/Arecsu/darktable/commit/194f9e1) | yuri | fix(ui): add spektrafilm to modules list |
| 2026-07-31 | [0dad59a](https://github.com/Arecsu/darktable/commit/0dad59a) | piratenpanda | Updates to user feedback |

## Data pack

The module downloads the spectral data pack it needs automatically. First enable **Preferences → Security → "allow spektrafilm to download data packs"**, then open the spektrafilm module on an image and click **"download data pack"** when it appears. Every file is verified against a checksum from the repository manifest before install, and downloaded packs are written to the `spektrafilm/packs` subfolder of your darktable config directory, so they are backed up with the rest of your configuration.
