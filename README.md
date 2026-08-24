# Darktable Spektrafilm — Builds

 Automated builds from the [spektrafilm-draft](https://github.com/piratenpanda/darktable/tree/spektrafilm-draft) branch.

Come work together! Feedback, issues, anything is welcome at [discuss.pixls.us](https://discuss.pixls.us/t/spektrafilm-darktable-module-implementation-discussion/58744)

> **⚠️ HIGHLY EXPERIMENTAL** — back up your darktable data dir before testing: Linux `~/.config/darktable/`, macOS `~/Library/Application Support/darktable/`, Windows `%APPDATA%\darktable\`. Use `--library <path>` to keep your main setup safe.

**Latest version:** 20260824-2201049

## Latest Builds

| Platform | Architecture | Download |
|----------|-------------|----------|
| Linux AppImage | x86_64 | [darktable-spektrafilm-20260824-2201049-x86_64.AppImage](https://github.com/piratenpanda/dt-spektrafilm-builds/releases/download/spektrafilm-builds/darktable-spektrafilm-20260824-2201049-x86_64.AppImage) |
| Linux AppImage | ARM64 | [darktable-spektrafilm-20260824-2201049-aarch64.AppImage](https://github.com/piratenpanda/dt-spektrafilm-builds/releases/download/spektrafilm-builds/darktable-spektrafilm-20260824-2201049-aarch64.AppImage) |
| Windows | x86_64 | [darktable-spektrafilm-20260824-2201049-x86_64.exe](https://github.com/piratenpanda/dt-spektrafilm-builds/releases/download/spektrafilm-builds/darktable-spektrafilm-20260824-2201049-x86_64.exe) |
| macOS | ARM64 (Apple Silicon) | [darktable-spektrafilm-20260824-2201049-arm64.dmg](https://github.com/piratenpanda/dt-spektrafilm-builds/releases/download/spektrafilm-builds/darktable-spektrafilm-20260824-2201049-arm64.dmg) |
| macOS | x86_64 (Intel) | [darktable-spektrafilm-20260824-2201049-x86_64.dmg](https://github.com/piratenpanda/dt-spektrafilm-builds/releases/download/spektrafilm-builds/darktable-spektrafilm-20260824-2201049-x86_64.dmg) |

## Recent Commits

| Date | Commit | Author | Message |
|------|--------|--------|---------|
| 2026-08-24 | [22010494c](https://github.com/piratenpanda/darktable/commit/22010494c) | piratenpanda | spektrafilm: fold the diffusion tab into film and print |
| 2026-08-24 | [0da246e72](https://github.com/piratenpanda/darktable/commit/0da246e72) | piratenpanda | spektrafilm: strip trailing whitespace |
| 2026-08-24 | [75ce96555](https://github.com/piratenpanda/darktable/commit/75ce96555) | piratenpanda | spektrafilm: make the film and print sections collapsible |
| 2026-08-23 | [10ce5c16a](https://github.com/piratenpanda/darktable/commit/10ce5c16a) | piratenpanda | spektrafilm: fold "scan the film" into the paper selector |

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
4. Newer builds will use ~/.local/share/darktable as the pack download directory    

