# Darktable Spektrafilm — Builds

 Automated builds from the [spektrafilm](https://github.com/piratenpanda/darktable/tree/spektrafilm) branch, with the following upstream PR(s) cherry-picked on top: 22004.

Come work together! Feedback, issues, anything is welcome at [discuss.pixls.us](https://discuss.pixls.us/t/spektrafilm-darktable-module-implementation-discussion/58744)

> **⚠️ HIGHLY EXPERIMENTAL** — back up your darktable data dir before testing: Linux `~/.config/darktable/`, macOS `~/Library/Application Support/darktable/`, Windows `%APPDATA%\darktable\`. Use `--library <path>` to keep your main setup safe.

**Latest version:** 20260903-e75453c

## Latest Builds

| Platform | Architecture | Download |
|----------|-------------|----------|
| Linux AppImage | x86_64 | [darktable-spektrafilm-20260903-e75453c-x86_64.AppImage](https://github.com/piratenpanda/dt-spektrafilm-builds/releases/download/spektrafilm-builds/darktable-spektrafilm-20260903-e75453c-x86_64.AppImage) |
| Linux AppImage | ARM64 | [darktable-spektrafilm-20260903-e75453c-aarch64.AppImage](https://github.com/piratenpanda/dt-spektrafilm-builds/releases/download/spektrafilm-builds/darktable-spektrafilm-20260903-e75453c-aarch64.AppImage) |
| Windows | x86_64 | [darktable-spektrafilm-20260903-e75453c-x86_64.exe](https://github.com/piratenpanda/dt-spektrafilm-builds/releases/download/spektrafilm-builds/darktable-spektrafilm-20260903-e75453c-x86_64.exe) |
| Windows | ARM64 | [darktable-spektrafilm-20260903-e75453c-x86_64.exe](https://github.com/piratenpanda/dt-spektrafilm-builds/releases/download/spektrafilm-builds/darktable-spektrafilm-20260903-e75453c-x86_64.exe) |
| macOS | ARM64 (Apple Silicon) | [darktable-spektrafilm-20260903-e75453c-arm64.dmg](https://github.com/piratenpanda/dt-spektrafilm-builds/releases/download/spektrafilm-builds/darktable-spektrafilm-20260903-e75453c-arm64.dmg) |

## Recent Commits

| Date | Commit | Author | Message |
|------|--------|--------|---------|
| 2026-09-03 | [e75453c86](https://github.com/piratenpanda/darktable/commit/e75453c86) | piratenpanda | add spektrafilm pixel workflow |
| 2026-09-03 | [1ade92d36](https://github.com/piratenpanda/darktable/commit/1ade92d36) | piratenpanda | add gamut compression toggle |
| 2026-09-03 | [cc60d69a1](https://github.com/piratenpanda/darktable/commit/cc60d69a1) | piratenpanda | add GTK4 code |
| 2026-09-02 | [e7ea772f3](https://github.com/piratenpanda/darktable/commit/e7ea772f3) | piratenpanda | Spektrafilm analog film simulation module |

## Data pack

If you are upgrading from an older build, delete the `spektrafilm` folder from your darktable config directory first, so the module doesn't keep using outdated data:

| Platform | Folder to delete |
|----------|------------------|
| Linux | `~/.config/darktable/spektrafilm/` |
| macOS | `~/Library/Application Support/darktable/spektrafilm/` |
| macOS | `~/.config/darktable/spektrafilm/` |
| Windows | `%APPDATA%\darktable\spektrafilm\` |

> ** Current builds use ~/.local/share/darktable as the pack download directory on Linux. Other platforms accordingly.   

Then:

1. Enable **Preferences → Security → "allow spektrafilm to download data packs"**.
2. **Restart darktable** — the setting only takes effect after a restart.
3. Open the spektrafilm module on a photo. If a data pack is missing, a **"download data pack"** button appears — click it and the module downloads the data pack it needs, verifying the download before it's used.

