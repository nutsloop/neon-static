# Neon Static

A clean, professional Sphinx theme with a static layout and no animations.

## Install

```bash
pip install -e /path/to/neon-static
```

Or in `requirements.txt`:

```
-e ../themes/neon-static
```

## Usage

```python
html_theme = "neon-static"

html_theme_options = {
    "light_logo": "logo-light.svg",
    "dark_logo": "logo-dark.svg",
    "sidebar_hide_name": False,
    "navigation_with_keys": True,
    "default_theme": "system",
}
```

## Theme options

- `light_logo`: logo for light mode
- `dark_logo`: logo for dark mode
- `sidebar_hide_name`: hide project name in the sidebar
- `navigation_with_keys`: enable keyboard navigation
- `default_theme`: `"dark"`, `"light"`, or `"system"`

Logo files are expected under `_static/` (for example, `_static/logo-light.svg`).

## Environment variables

These are read in the book build and passed into the theme.

- `NEONBOOK_THEME`: `neon-synth`, `neon-wave`, or `neon-static` (default: `neon-synth`)
- `NEONBOOK_PERF_LOG`: enable performance console logging (default: `off`)

`NEONBOOK_VHS`, `NEONBOOK_PERF_SOUND`, and `NEONBOOK_PERF_NOTIFY` are ignored by this theme.

For boolean flags, any value other than `0`, `off`, `false`, or `no` is treated as on.

## License

Apache License 2.0. See `LICENSE`.
