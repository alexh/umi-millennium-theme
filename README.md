# UMI for Millennium

UMI is an ornate industrial theme for the Steam client via [Millennium](https://steambrew.app/). It uses warm-dark chrome, cream content panels, layered bevels, subtle SVG grain, and hazard-orange activation states.

![UMI theme splash](assets/splash.svg)

## Install

1. Install Millennium from the [Steam Homebrew docs](https://docs.steambrew.app/users/index).
2. Clone this repo into your Millennium themes directory:

```sh
git clone https://github.com/alexh/umi-millennium-theme.git ~/.local/share/Steam/millennium/themes/UMI
```

3. Open Steam, go to `Steam` -> `Millennium` -> `Themes`, then select `UMI`.

For local development, symlink the repo instead:

```sh
ln -s ~/dev/umi-millennium-theme ~/.local/share/Steam/millennium/themes/UMI
```

CSS changes hot-reload through Millennium. JavaScript or `skin.json` changes may require a Steam restart.

## Aesthetic

UMI uses a compact palette:

- Warm dark chrome: `#14090a`, `#1a0e08`, `#2a1c12`, `#3c3836`
- Cream content panels: `#fbf1c7`
- Activation orange: `#ff6700`
- Hazard striping: `#c94a00` and `#ff8a4a`

Orange is reserved for active, selected, focused, and primary action states.

## Structure

This theme uses Millennium's default patch layout:

- `webkit.css` loads into all Steam web views.
- `libraryroot.custom.css` and `.js` load into the main Steam window.
- `friends.custom.css` and `.js` load into the Friends UI.
- `bigpicture.custom.css` and `.js` load into Big Picture mode.

`skin.json` uses `UseDefaultPatches: true`, so it intentionally does not define custom `Patches` or `Steam-WebKit` entries.

## Status

This is an early public extraction from the broader UMI desktop theme. Steam class names change frequently, so selectors may need updates as Steam ships new builds.

## License

MIT. See [LICENSE](LICENSE).
