# Darktable Spektrafilm — Builds

 Automated builds from the [spektrafilm](https://github.com/piratenpanda/darktable/tree/spektrafilm) branch.

Come work together! Feedback, issues, anything is welcome at [discuss.pixls.us](https://discuss.pixls.us/t/spektrafilm-darktable-module-implementation-discussion/58744)

> **⚠️ HIGHLY EXPERIMENTAL** — back up your darktable data dir before testing: Linux `~/.config/darktable/`, macOS `~/Library/Application Support/darktable/`, Windows `%APPDATA%\darktable\`. Use `--library <path>` to keep your main setup safe.

**Latest version:** 20260824-cef3766

## Latest Builds

| Platform | Architecture | Download |
|----------|-------------|----------|
| Linux AppImage | x86_64 | [darktable-spektrafilm-20260824-cef3766-x86_64.AppImage](https://github.com/piratenpanda/dt-spektrafilm-builds/releases/download/spektrafilm-builds/darktable-spektrafilm-20260824-cef3766-x86_64.AppImage) |
| Linux AppImage | ARM64 | [darktable-spektrafilm-20260824-cef3766-aarch64.AppImage](https://github.com/piratenpanda/dt-spektrafilm-builds/releases/download/spektrafilm-builds/darktable-spektrafilm-20260824-cef3766-aarch64.AppImage) |
| Windows | x86_64 | [darktable-spektrafilm-20260824-cef3766-x86_64.exe](https://github.com/piratenpanda/dt-spektrafilm-builds/releases/download/spektrafilm-builds/darktable-spektrafilm-20260824-cef3766-x86_64.exe) |
| macOS | ARM64 (Apple Silicon) | [darktable-spektrafilm-20260824-cef3766-arm64.dmg](https://github.com/piratenpanda/dt-spektrafilm-builds/releases/download/spektrafilm-builds/darktable-spektrafilm-20260824-cef3766-arm64.dmg) |
| macOS | x86_64 (Intel) | [darktable-spektrafilm-20260824-cef3766-x86_64.dmg](https://github.com/piratenpanda/dt-spektrafilm-builds/releases/download/spektrafilm-builds/darktable-spektrafilm-20260824-cef3766-x86_64.dmg) |

## Recent Commits

| Date | Commit | Author | Message |
|------|--------|--------|---------|
| 2026-08-24 | [cef376638](https://github.com/piratenpanda/darktable/commit/cef376638) | Benjamin Grimm-Lebsanft | make diffusion checkboxes reset on collapsible reset |
| 2026-08-24 | [419cadf65](https://github.com/piratenpanda/darktable/commit/419cadf65) | piratenpanda | spektrafilm: put the diffusion switches inside their sections |
| 2026-08-24 | [22010494c](https://github.com/piratenpanda/darktable/commit/22010494c) | piratenpanda | spektrafilm: fold the diffusion tab into film and print |
| 2026-08-24 | [0da246e72](https://github.com/piratenpanda/darktable/commit/0da246e72) | piratenpanda | spektrafilm: strip trailing whitespace |

## Data pack

** Current builds use ~/.local/share/darktable as the pack download directory on Linux. Other platforms accordingly **    

If you are upgrading from an older build, delete the `spektrafilm` folder from your darktable config directory first, so the module doesn't keep using outdated data:

| Platform | Folder to delete |
|----------|------------------|
| Linux | `~/.config/darktable/spektrafilm/` |
| macOS | `~/Library/Application Support/darktable/spektrafilm/` |
| macOS | `~/.config/darktable/spektrafilm/` |
| Windows | `%APPDATA%\darktable\spektrafilm\` |

Then:

1. Enable **Preferences → Security → "allow spektrafilm to download data packs"**. (newer builds don't have this option anymore)
2. **Restart darktable** — the setting only takes effect after a restart.
3. Open the spektrafilm module on a photo. If a data pack is missing, a **"download data pack"** button appears — click it and the module downloads the data pack it needs, verifying the download before it's used.
