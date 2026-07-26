# Darktable Spektrafilm — Builds

 Automated builds from the [spektrafilm-draft](https://github.com/Arecsu/darktable/tree/spektrafilm-draft) branch.

Come work together! Feedback, issues, anything is welcome at [discuss.pixls.us](https://discuss.pixls.us/t/spektrafilm-darktable-module-implementation-discussion/58744)

> **⚠️ HIGHLY EXPERIMENTAL** — back up your darktable data dir before testing: Linux `~/.config/darktable/`, macOS `~/Library/Application Support/darktable/`, Windows `%APPDATA%\darktable\`. Use `--library <path>` to keep your main setup safe.

**Latest version:** 20260726-69a1eb6

## Latest Builds

| Platform | Architecture | Download |
|----------|-------------|----------|
| Linux AppImage | x86_64 | [darktable-spektrafilm-20260726-69a1eb6-x86_64.AppImage](https://github.com/Arecsu/dt-spektrafilm-builds/releases/download/spektrafilm-builds/darktable-spektrafilm-20260726-69a1eb6-x86_64.AppImage) |
| Linux AppImage | ARM64 | [darktable-spektrafilm-20260726-69a1eb6-aarch64.AppImage](https://github.com/Arecsu/dt-spektrafilm-builds/releases/download/spektrafilm-builds/darktable-spektrafilm-20260726-69a1eb6-aarch64.AppImage) |
| Windows | x86_64 | [darktable-spektrafilm-20260726-69a1eb6-x86_64.exe](https://github.com/Arecsu/dt-spektrafilm-builds/releases/download/spektrafilm-builds/darktable-spektrafilm-20260726-69a1eb6-x86_64.exe) |
| macOS | ARM64 (Apple Silicon) | [darktable-spektrafilm-20260726-69a1eb6-arm64.dmg](https://github.com/Arecsu/dt-spektrafilm-builds/releases/download/spektrafilm-builds/darktable-spektrafilm-20260726-69a1eb6-arm64.dmg) |
| macOS | x86_64 (Intel) | [darktable-spektrafilm-20260726-69a1eb6-x86_64.dmg](https://github.com/Arecsu/dt-spektrafilm-builds/releases/download/spektrafilm-builds/darktable-spektrafilm-20260726-69a1eb6-x86_64.dmg) |

## Recent Commits

| Date | Commit | Author | Message |
|------|--------|--------|---------|
| 2026-07-26 | [69a1eb6](https://github.com/Arecsu/darktable/commit/69a1eb6) | piratenpanda | more fixes for BW films, expose development time for films and papers that support it |
| 2026-07-26 | [6797d15](https://github.com/Arecsu/darktable/commit/6797d15) | piratenpanda | remove stale code, make algorithms adhere to spektrafilm ref code, add missing glare stage and scanner feature set |
| 2026-07-25 | [ccea8c2](https://github.com/Arecsu/darktable/commit/ccea8c2) | piratenpanda | safeguard scan button from resetting |
| 2026-07-23 | [c6e5c93](https://github.com/Arecsu/darktable/commit/c6e5c93) | piratenpanda | fix USM oversharpening on zoom out |

## Required: Film & Print Data Pack

Download the [spektrafilm-data-pack.zip](https://github.com/Arecsu/dt-spektrafilm-builds/raw/main/spektrafilm-data-pack.zip) and extract it **anywhere** — you'll get a `spektrafilm/` folder. Then move or copy that folder into your darktable config directory:

| Platform | Darktable config directory |
|----------|---------------------------|
| Linux | `~/.config/darktable/` |
| macOS | `~/Library/Application Support/darktable/` |
| Windows | `%APPDATA%\darktable\` |

The final structure should look like this:

```
spektrafilm/
├── pack.json
├── spectra_lut.f32
└── profiles/
    ├── kodak_portra_400.json
    ├── fujifilm_velvia_100.json
    └── ...
```
