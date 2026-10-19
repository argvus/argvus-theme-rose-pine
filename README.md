# Rosé Pine theme for ARGVUS

Official ARGVUS Dark theme, `rose-pine`, with its Sticky and Float variants.

[![CI](https://github.com/argvus/argvus-theme-rose-pine/actions/workflows/ci.yml/badge.svg)](https://github.com/argvus/argvus-theme-rose-pine/actions/workflows/ci.yml)
[![Release](https://github.com/argvus/argvus-theme-rose-pine/actions/workflows/release.yml/badge.svg)](https://github.com/argvus/argvus-theme-rose-pine/actions/workflows/release.yml)
[![License](https://img.shields.io/badge/License-GPL--3.0-blue.svg)](LICENSE)

## Theme identity

| Field | Value |
| --- | --- |
| Theme ID | `rose-pine` (Float variant: `rose-pine-float`) |
| Display name | Rosé Pine |
| Mode | `dark` |
| Default highlight | `#C4A7E7` |
| GTK color scheme | `prefer-dark` |
| Calendar stylesheet | `rose-pine` |
| Package | `argvus-theme-rose-pine` |
| Wallpaper | `/usr/share/backgrounds/argvus/abstract/dark/rose-pine-abstract-dark.jxl` |

The values above are the ones declared in
`src/usr/share/argvus/appearance/themes.d/rose-pine/theme.toml`, the manifest that the
desktop reads. The manifest is the source of truth; this page describes it.

## Installing

The package depends on `argvus` and `argvus-appearance`, so pacman installs them with it.

```sh
sudo pacman -S argvus-theme-rose-pine
```

Select the theme in the Control Center (Appearance > Themes), or run
`argvus theme-switch rose-pine`.

## Files

The package installs the theme's per-component files under `/usr/share/argvus` (and the
calendar stylesheet under `/etc/argvus/taskbar/calendar/themes`). Each component that
the theme styles has its own directory, listed by `find src -type f` in this repository.

## Development

Validate with `make validate` before building. The design rules are in
[DEVELOPMENT.md](DEVELOPMENT.md); the ARGVUS documentation for themes is in
`argvus/docs/en/user-guide/appearance.md` of the `argvus` repository.

## License

GPL-3.0-only. See [LICENSE](LICENSE).
