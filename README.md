# Darktable Spektrafilm — Builds

 Automated builds from the [spektrafilm-draft](https://github.com/Arecsu/darktable/tree/spektrafilm-draft) branch.

Come work together! Feedback, issues, anything is welcome at [discuss.pixls.us](https://discuss.pixls.us/t/spektrafilm-darktable-module-implementation-discussion/58744)

> **⚠️ HIGHLY EXPERIMENTAL** — back up your darktable data dir before testing: Linux `~/.config/darktable/`, macOS `~/Library/Application Support/darktable/`, Windows `%APPDATA%\darktable\`. Use `--library <path>` to keep your main setup safe.

**Latest version:** 20260730-036ba03

## Latest Builds

| Platform | Architecture | Download |
|----------|-------------|----------|
| Linux AppImage | x86_64 | [darktable-spektrafilm-20260730-036ba03-x86_64.AppImage](https://github.com/Arecsu/dt-spektrafilm-builds/releases/download/spektrafilm-builds/darktable-spektrafilm-20260730-036ba03-x86_64.AppImage) |
| Linux AppImage | ARM64 | [darktable-spektrafilm-20260730-036ba03-aarch64.AppImage](https://github.com/Arecsu/dt-spektrafilm-builds/releases/download/spektrafilm-builds/darktable-spektrafilm-20260730-036ba03-aarch64.AppImage) |
| Windows | x86_64 | [darktable-spektrafilm-20260730-036ba03-x86_64.exe](https://github.com/Arecsu/dt-spektrafilm-builds/releases/download/spektrafilm-builds/darktable-spektrafilm-20260730-036ba03-x86_64.exe) |
| macOS | ARM64 (Apple Silicon) | [darktable-spektrafilm-20260730-036ba03-arm64.dmg](https://github.com/Arecsu/dt-spektrafilm-builds/releases/download/spektrafilm-builds/darktable-spektrafilm-20260730-036ba03-arm64.dmg) |
| macOS | x86_64 (Intel) | [darktable-spektrafilm-20260730-036ba03-x86_64.dmg](https://github.com/Arecsu/dt-spektrafilm-builds/releases/download/spektrafilm-builds/darktable-spektrafilm-20260730-036ba03-x86_64.dmg) |

## Recent Commits

| Date | Commit | Author | Message |
|------|--------|--------|---------|
| 2026-07-29 | [036ba03](https://github.com/Arecsu/darktable/commit/036ba03) | piratenpanda | move to float16 LUT as reference, fix grain opencl path again, fix diffusion filters and clarify scatter |
| 2026-07-27 | [2d832d6](https://github.com/Arecsu/darktable/commit/2d832d6) | piratenpanda | Reset module to v1, remove special checkbox handling as this is now a proper bauhaus widget, add blank lines between routined, use GList where necessary, use dt_hash(), add underscore prefex to static routines |
| 2026-07-27 | [bd2b5ab](https://github.com/Arecsu/darktable/commit/bd2b5ab) | piratenpanda | follow the Bauhaus checkbox changes |
| 2026-07-26 | [92ff3a5](https://github.com/Arecsu/darktable/commit/92ff3a5) | piratenpanda | limit DIR coupler range to 1 to keep it invertible |

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
