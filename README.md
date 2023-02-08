# Yaru for Steam

A skin to make Steam look more like a native Ubuntu app.

This is a fork of [Adwaita-for-Steam](https://github.com/tkashkin/Adwaita-for-Steam), all the credit goes to them.

The Yaru icon assets (any and all source `.svg` files under `Yaru/` or related rendered `.png` files) are licensed under the terms of the [Creative Commons Attribution-ShareAlike 4.0 License](https://creativecommons.org/licenses/by-sa/4.0/).

<p align="center"><img src="screenshot.png?raw=true"/></p>

## Current state and plans

* **Main window**: done.
* **Settings**: mostly done.
* **New library, new chat, other web-based client parts**: partially done.
* **Overlay**: done.
* **Small mode**: done.
* **Old library, old chat, other old unused windows**: not planned.
* **Recoloring**: colors can be changed via making a new theme. See `color_themes` dir.
* **Light theme**: not planned, would require redrawing all assets to be visible on light backgrounds.

### Limitations

* **Rounded corners**: impossible to do in a Steam skin, use [Rounded Window Corners extension](https://github.com/yilozt/rounded-window-corners) or [mutter-rounded](https://github.com/yilozt/mutter-rounded) on GNOME
* **Height of menu/sidebar items**: doesn't seem to be possible to increase

## Requirements

* [Ubuntu fonts](https://design.ubuntu.com/font/) as static fonts. Some distros install it as a variable font that is not supported by Steam, see [#45](https://github.com/tkashkin/Adwaita-for-Steam/issues/45).
* The skin was created for the Linux version of Steam and wasn't tested on Windows or macOS. It will work with some visual problems.

## Previews

<details><summary>Previews</summary>

<details><summary>Adwaita</summary>

![Adwaita](/extras/colorthemes/adwaita/preview.png?raw=true)

</details>

<details><summary>Breeze</summary>

![Breeze](/extras/colorthemes/breeze/preview.png?raw=true)

</details>

<details><summary>Catppuccin-Frappe</summary>

![Catppuccin-Frappe](/extras/colorthemes/catppuccin-frappe/preview.png?raw=true)

</details>

<details><summary>Catppuccin-Macchiato</summary>

![Catppuccin-Macchiato](/extras/colorthemes/catppuccin-macchiato/preview.png?raw=true)

</details>

<details><summary>Catppuccin-Mocha</summary>

![Catppuccin-Mocha](/extras/colorthemes/catppuccin-mocha/preview.png?raw=true)

</details>

<details><summary>Dracula</summary>

![Dracula](/extras/colorthemes/dracula/preview.png?raw=true)

</details>

<details><summary>Kate</summary>

![Kate](/extras/colorthemes/kate/preview.png?raw=true)

</details>

<details><summary>Nord</summary>

![Nord](/extras/colorthemes/nord/preview.png?raw=true)

</details>

<details><summary>One Pro</summary>

![One Pro](/extras/colorthemes/one-pro/preview.png?raw=true)

</details>

<details><summary>Pop</summary>

![Pop](/extras/colorthemes/pop/preview.png?raw=true)

</details>

<details><summary>Tokyo Night</summary>

![Tokyo Night](/extras/colorthemes/tokyo-night/preview.png?raw=true)

</details>

<details><summary>Tomorrow Night</summary>

![Tomorrow Night](/extras/colorthemes/tomorrow-night/preview.png?raw=true)

</details>

<details><summary>Yaru</summary>

![Yaru](/extras/colorthemes/yaru/preview.png?raw=true)

</details>

</details>

## Installation

### With installer script

```bash
git clone https://github.com/Jupi007/Yaru-for-Steam
cd Yaru-for-Steam
./install.py
```

Run `./install.py -l` to see customization options.

Run `./install.py -c ${color_theme}` to change the color theme.

Run `./install.py -p ${patch_name}` to apply patches.

Run `./install.py -w {base, full, none}` to change the type of theme for web based elements of steam. base is a basic default, full includes heavier theming (including chat), and none disables this feature.

Run `./install.py -we ${web_extra_name}` to add an optional extra to the web theme.

Run `./install.py -h` to see all installer options.

### Manual installation

1. Download the [latest skin version](https://github.com/Jupi007/Yaru-for-Steam/archive/master.zip)
2. Extract `Adwaita` directory into Steam `skins` directory (create if it doesn't exist):
   * **Linux**: `~/.steam/steam/skins` or `~/.local/share/Steam/skins`
   * **Linux (flatpak)**: `~/.var/app/com.valvesoftware.Steam/.local/share/Steam/skins`
   * ~~Windows~~ (untested): `C:\Program Files (x86)\Steam\skins` by default
   * ~~macOS~~ (untested): `~/Library/Application Support/Steam/Steam.AppBundle/Steam/Contents/MacOS/skins`
3. Rename it into `Yaru`
4. Open Steam and select `Yaru` skin in Settings > Interface (restart Steam if it doesn't appear in the list)
