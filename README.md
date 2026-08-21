# Darktable Spektrafilm — Builds

 Automated builds from the [spektrafilm-draft](https://github.com/Arecsu/darktable/tree/spektrafilm-draft) branch.

Come work together! Feedback, issues, anything is welcome at [discuss.pixls.us](https://discuss.pixls.us/t/spektrafilm-darktable-module-implementation-discussion/58744)

> **⚠️ HIGHLY EXPERIMENTAL** — back up your darktable data dir before testing: Linux `~/.config/darktable/`, macOS `~/Library/Application Support/darktable/`, Windows `%APPDATA%\darktable\`. Use `--library <path>` to keep your main setup safe.

**Latest version:** 20260821-6545711

## Latest Builds

| Platform | Architecture | Download |
|----------|-------------|----------|
| Linux AppImage | x86_64 | [darktable-spektrafilm-20260821-6545711-x86_64.AppImage](https://github.com/Arecsu/dt-spektrafilm-builds/releases/download/spektrafilm-builds/darktable-spektrafilm-20260821-6545711-x86_64.AppImage) |
| Linux AppImage | ARM64 | [darktable-spektrafilm-20260821-6545711-aarch64.AppImage](https://github.com/Arecsu/dt-spektrafilm-builds/releases/download/spektrafilm-builds/darktable-spektrafilm-20260821-6545711-aarch64.AppImage) |
| Windows | x86_64 | [darktable-spektrafilm-20260821-6545711-x86_64.exe](https://github.com/Arecsu/dt-spektrafilm-builds/releases/download/spektrafilm-builds/darktable-spektrafilm-20260821-6545711-x86_64.exe) |
| macOS | ARM64 (Apple Silicon) | [darktable-spektrafilm-20260821-6545711-arm64.dmg](https://github.com/Arecsu/dt-spektrafilm-builds/releases/download/spektrafilm-builds/darktable-spektrafilm-20260821-6545711-arm64.dmg) |
| macOS | x86_64 (Intel) | [darktable-spektrafilm-20260821-6545711-x86_64.dmg](https://github.com/Arecsu/dt-spektrafilm-builds/releases/download/spektrafilm-builds/darktable-spektrafilm-20260821-6545711-x86_64.dmg) |

## Recent Commits

| Date | Commit | Author | Message |
|------|--------|--------|---------|
| 2026-08-08 | [6545711](https://github.com/Arecsu/darktable/commit/6545711) | piratenpanda | remove patch file |
| 2026-08-08 | [5b47563](https://github.com/Arecsu/darktable/commit/5b47563) | piratenpanda | port unit test suite from reference |
| 2026-08-05 | [1c6ceff](https://github.com/Arecsu/darktable/commit/1c6ceff) | piratenpanda | remove references to the reference |
| 2026-08-05 | [80990be](https://github.com/Arecsu/darktable/commit/80990be) | piratenpanda | add switch for bandwidth adaption and rename section to advanced |

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
