# Darktable Spektrafilm — Builds

 Automated builds from the [spektrafilm](https://github.com/piratenpanda/darktable/tree/spektrafilm) branch.

Come work together! Feedback, issues, anything is welcome at [discuss.pixls.us](https://discuss.pixls.us/t/spektrafilm-darktable-module-implementation-discussion/58744)

> **⚠️ HIGHLY EXPERIMENTAL** — back up your darktable data dir before testing: Linux `~/.config/darktable/`, macOS `~/Library/Application Support/darktable/`, Windows `%APPDATA%\darktable\`. Use `--library <path>` to keep your main setup safe.

**Latest version:** 20260823-549f935

## Latest Builds

| Platform | Architecture | Download |
|----------|-------------|----------|
| Linux AppImage | x86_64 | [darktable-spektrafilm-20260823-549f935-x86_64.AppImage](https://github.com/piratenpanda/dt-spektrafilm-builds/releases/download/spektrafilm-builds/darktable-spektrafilm-20260823-549f935-x86_64.AppImage) |
| Linux AppImage | ARM64 | [darktable-spektrafilm-20260823-549f935-aarch64.AppImage](https://github.com/piratenpanda/dt-spektrafilm-builds/releases/download/spektrafilm-builds/darktable-spektrafilm-20260823-549f935-aarch64.AppImage) |
| Windows | x86_64 | [darktable-spektrafilm-20260823-549f935-x86_64.exe](https://github.com/piratenpanda/dt-spektrafilm-builds/releases/download/spektrafilm-builds/darktable-spektrafilm-20260823-549f935-x86_64.exe) |
| macOS | ARM64 (Apple Silicon) | [darktable-spektrafilm-20260823-549f935-arm64.dmg](https://github.com/piratenpanda/dt-spektrafilm-builds/releases/download/spektrafilm-builds/darktable-spektrafilm-20260823-549f935-arm64.dmg) |
| macOS | x86_64 (Intel) | [darktable-spektrafilm-20260823-549f935-x86_64.dmg](https://github.com/piratenpanda/dt-spektrafilm-builds/releases/download/spektrafilm-builds/darktable-spektrafilm-20260823-549f935-x86_64.dmg) |

## Recent Commits

| Date | Commit | Author | Message |
|------|--------|--------|---------|
| 2026-08-23 | [549f93528](https://github.com/piratenpanda/darktable/commit/549f93528) | t | spektrafilm: drop the blank line at end of file |
| 2026-08-23 | [648e3f9ee](https://github.com/piratenpanda/darktable/commit/648e3f9ee) | t | spektrafilm: solve the output scale in its own slot |
| 2026-08-23 | [9dc90ea4a](https://github.com/piratenpanda/darktable/commit/9dc90ea4a) | t | spektrafilm: retry the grain tables after a failed OpenCL upload |
| 2026-08-23 | [46bd66114](https://github.com/piratenpanda/darktable/commit/46bd66114) | t | spektrafilm: declare the tile memory the module uses |

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

