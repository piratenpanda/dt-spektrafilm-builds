# Darktable Spektrafilm — Builds

 Automated builds from the [spektrafilm-draft](https://github.com/Arecsu/darktable/tree/spektrafilm-draft) branch.

Come work together! Feedback, issues, anything is welcome at [discuss.pixls.us](https://discuss.pixls.us/t/spektrafilm-darktable-module-implementation-discussion/58744)

> **⚠️ HIGHLY EXPERIMENTAL** — back up your darktable data dir before testing: Linux `~/.config/darktable/`, macOS `~/Library/Application Support/darktable/`, Windows `%APPDATA%\darktable\`. Use `--library <path>` to keep your main setup safe.

**Latest version:** 20260725-ccea8c2

## Latest Builds

| Platform | Architecture | Download |
|----------|-------------|----------|
| Linux AppImage | x86_64 | [darktable-spektrafilm-20260725-ccea8c2-x86_64.AppImage](https://github.com/Arecsu/dt-spektrafilm-builds/releases/download/spektrafilm-builds/darktable-spektrafilm-20260725-ccea8c2-x86_64.AppImage) |
| Linux AppImage | ARM64 | [darktable-spektrafilm-20260725-ccea8c2-aarch64.AppImage](https://github.com/Arecsu/dt-spektrafilm-builds/releases/download/spektrafilm-builds/darktable-spektrafilm-20260725-ccea8c2-aarch64.AppImage) |
| Windows | x86_64 | [darktable-spektrafilm-20260725-ccea8c2-x86_64.exe](https://github.com/Arecsu/dt-spektrafilm-builds/releases/download/spektrafilm-builds/darktable-spektrafilm-20260725-ccea8c2-x86_64.exe) |
| macOS | ARM64 (Apple Silicon) | [darktable-spektrafilm-20260725-ccea8c2-arm64.dmg](https://github.com/Arecsu/dt-spektrafilm-builds/releases/download/spektrafilm-builds/darktable-spektrafilm-20260725-ccea8c2-arm64.dmg) |
| macOS | x86_64 (Intel) | [darktable-spektrafilm-20260725-ccea8c2-x86_64.dmg](https://github.com/Arecsu/dt-spektrafilm-builds/releases/download/spektrafilm-builds/darktable-spektrafilm-20260725-ccea8c2-x86_64.dmg) |

## Recent Commits

| Date | Commit | Author | Message |
|------|--------|--------|---------|
| 2026-07-25 | [ccea8c2](https://github.com/Arecsu/darktable/commit/ccea8c2) | piratenpanda | safeguard scan button from resetting |
| 2026-07-23 | [c6e5c93](https://github.com/Arecsu/darktable/commit/c6e5c93) | piratenpanda | fix USM oversharpening on zoom out |
| 2026-07-23 | [0c13f59](https://github.com/Arecsu/darktable/commit/0c13f59) | piratenpanda | restructure UI on feedback |
| 2026-07-23 | [476c000](https://github.com/Arecsu/darktable/commit/476c000) | piratenpanda | make grain adhere to reference implementation and set default parameters |

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
