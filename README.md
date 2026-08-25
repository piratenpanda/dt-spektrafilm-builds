# Darktable Spektrafilm — Builds

 Automated builds from the [spektrafilm](https://github.com/piratenpanda/darktable/tree/spektrafilm) branch.

Come work together! Feedback, issues, anything is welcome at [discuss.pixls.us](https://discuss.pixls.us/t/spektrafilm-darktable-module-implementation-discussion/58744)

> **⚠️ HIGHLY EXPERIMENTAL** — back up your darktable data dir before testing: Linux `~/.config/darktable/`, macOS `~/Library/Application Support/darktable/`, Windows `%APPDATA%\darktable\`. Use `--library <path>` to keep your main setup safe.

**Latest version:** 20260825-beaac15

## Latest Builds

| Platform | Architecture | Download |
|----------|-------------|----------|
| Linux AppImage | x86_64 | [darktable-spektrafilm-20260825-beaac15-x86_64.AppImage](https://github.com/piratenpanda/dt-spektrafilm-builds/releases/download/spektrafilm-builds/darktable-spektrafilm-20260825-beaac15-x86_64.AppImage) |
| Linux AppImage | ARM64 | [darktable-spektrafilm-20260825-beaac15-aarch64.AppImage](https://github.com/piratenpanda/dt-spektrafilm-builds/releases/download/spektrafilm-builds/darktable-spektrafilm-20260825-beaac15-aarch64.AppImage) |
| Windows | x86_64 | [darktable-spektrafilm-20260825-beaac15-x86_64.exe](https://github.com/piratenpanda/dt-spektrafilm-builds/releases/download/spektrafilm-builds/darktable-spektrafilm-20260825-beaac15-x86_64.exe) |
| Windows | ARM64 | [darktable-spektrafilm-20260825-beaac15-x86_64.exe](https://github.com/piratenpanda/dt-spektrafilm-builds/releases/download/spektrafilm-builds/darktable-spektrafilm-20260825-beaac15-x86_64.exe) |
| macOS | ARM64 (Apple Silicon) | [darktable-spektrafilm-20260825-beaac15-arm64.dmg](https://github.com/piratenpanda/dt-spektrafilm-builds/releases/download/spektrafilm-builds/darktable-spektrafilm-20260825-beaac15-arm64.dmg) |
| macOS | x86_64 (Intel) | [darktable-spektrafilm-20260825-beaac15-x86_64.dmg](https://github.com/piratenpanda/dt-spektrafilm-builds/releases/download/spektrafilm-builds/darktable-spektrafilm-20260825-beaac15-x86_64.dmg) |

## Recent Commits

| Date | Commit | Author | Message |
|------|--------|--------|---------|
| 2026-08-24 | [beaac153c](https://github.com/piratenpanda/darktable/commit/beaac153c) | piratenpanda | spektrafilm: put the diffusion switches inside their sections |
| 2026-08-24 | [960692120](https://github.com/piratenpanda/darktable/commit/960692120) | piratenpanda | spektrafilm: fold the diffusion tab into film and print |
| 2026-08-24 | [bc7032e9d](https://github.com/piratenpanda/darktable/commit/bc7032e9d) | piratenpanda | spektrafilm: strip trailing whitespace |
| 2026-08-24 | [db57043f9](https://github.com/piratenpanda/darktable/commit/db57043f9) | piratenpanda | spektrafilm: make the film and print sections collapsible |

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

