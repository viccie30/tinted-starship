# Tinted Starship <img alt="Color wheel" src="https://raw.githubusercontent.com/tinted-theming/home/refs/heads/main/color_wheel.png" width="100" align="right" style="padding-top:0.6rem;">

Tinted terminal is a [Tinted Theming] terminal template repository
containing [Base16], [Base24] and [Tinted8] terminal theme files for [Starship].

Have a look at the [Tinted Theming Gallery] for examples of theme colors.

## Install

1. Copy one or more palettes from the files in the [themes directory](themes/)
   into your Starship configuration file.
   By default, this is `~/.config/starship.toml`.
2. Set the global `palette` variable to the theme you want to use.
   For instance, if you want to use `base24-gruvbox-dark`, write `palette = 
   base24-gruvbox-dark`.

## Use

Use the provided colors in [Starship]'s [style strings].
All themes, no matter if they're [Base16], [Base24], or [Tinted8], provide
access to the following colors.
If a theme does not provide a specific color, it will be marked as a fallback
in the theme.

### Foreground and background colors

`background` is the default background color (dark for dark themes, light
for light themes).
`foreground` is the default foreground (i.e. text) color (light for dark
themes, dark for light themes).

Both `background` and `foreground` also have 4 other variants.
`background-extreme` is darker than `background` for dark themes and
lighter than `background` for light themes. Conversely, `foreground-extreme` is
lighter than `foreground` for dark themes and darker than `foreground` for
light themes.

| Color                      |                            Dark theme                            |                           Light theme                            |
|----------------------------|:----------------------------------------------------------------:|:----------------------------------------------------------------:|
| `background-most-extreme`  | ![#181a1f](https://placehold.co/88x44/181a1f/fff?text=%23181a1f) | ![#fafafa](https://placehold.co/88x44/fafafa/000?text=%23fafafa) |
| `background-extreme`       | ![#21252b](https://placehold.co/88x44/21252b/fff?text=%2321252b) | ![#f0f0f1](https://placehold.co/88x44/f0f0f1/000?text=%23f0f0f1) |
| `background`               | ![#282c34](https://placehold.co/88x44/282c34/fff?text=%23282c34) | ![#e7e7e9](https://placehold.co/88x44/e7e7e9/000?text=%23e7e7e9) |
| `background-less-extreme`  | ![#3f4451](https://placehold.co/88x44/3f4451/fff?text=%233f4451) | ![#dfdfe1](https://placehold.co/88x44/dfdfe1/000?text=%23dfdfe1) |
| `background-least-extreme` | ![#4f5666](https://placehold.co/88x44/4f5666/fff?text=%234f5666) | ![#cacace](https://placehold.co/88x44/cacace/000?text=%23cacace) |
|                            |                                                                  |                                                                  |
| `foreground-least-extreme` | ![#545862](https://placehold.co/88x44/545862/000?text=%23545862) | ![#a0a1a7](https://placehold.co/88x44/a0a1a7/fff?text=%23a0a1a7) |
| `foreground-less-extreme`  | ![#9196a1](https://placehold.co/88x44/9196a1/000?text=%239196a1) | ![#696c77](https://placehold.co/88x44/696c77/fff?text=%23696c77) |
| `foreground`               | ![#abb2bf](https://placehold.co/88x44/abb2bf/000?text=%23abb2bf) | ![#383a42](https://placehold.co/88x44/383a42/fff?text=%23383a42) |
| `foreground-extreme`       | ![#e6e6e6](https://placehold.co/88x44/e6e6e6/000?text=%23e6e6e6) | ![#202227](https://placehold.co/88x44/202227/fff?text=%23202227) |
| `foreground-most-extreme`  | ![#ffffff](https://placehold.co/88x44/ffffff/000?text=%23ffffff) | ![#090a0b](https://placehold.co/88x44/090a0b/fff?text=%23090a0b) |

### Base24 colors

All [Base24 colors], `base00` through `base17`.
For [Base16] themes, `base10` through `base17` are synthesized using the
regular [Base24 fallbacks].
For [Tinted8] themes, all colors are synthesized from [Tinted8 colors].

### Tinted8 palette

All [Tinted8 colors], with periods replaced by hyphens.
For instance, `palette.magenta-bright` is available as `palette-magenta-bright`.
For [Base16] and [Base24] themes, all colors are synthesized from [Base24
colors].

### Tinted8 theming properties

The `ui.global.*` and `ui.status.*` [Tinted8 theming properties], with periods
replaced by hyphens.
For instance `ui.status.success` is available as `ui-status-success`.
For [Base16] and [Base24] themes, all colors are synthesized from [Base24
colors] using the [Tinted8 Builder default colors].

## Team

This theme is maintained by the following persons and a bunch of [awesome
contributors](https://github.com/tinted-theming/YOUR_PROJECT_HERE/graphs/contributors).

| [![Jamy](https://github.com/jamygolden.png?size=100)](https://github.com/JamyGolden) | [![viccie30](https://github.com/viccie30.png?size=100)](https://github.com/viccie30) |
|--------------------------------------------------------------------------------------|--------------------------------------------------------------------------------------|
| [Jamy](https://github.com/JamyGolden)                                                | [Victor](https://github.com/viccie30)                                                |

## Community

* [Tinted Theming Home](https://github.com/tinted-theming/home)
* Have something you want to discuss, but you're not sure it warrants an issue?
  Feel free to stop
  by [#tinted-theming:matrix.org](https://matrix.to/#/#tinted-theming:matrix.org)
  on [Matrix](https://matrix.org/).

## License

[MIT License](./LICENSE)

[Tinted Theming Gallery]: https://tinted-theming.github.io/tinted-gallery/
[Base16]: https://github.com/tinted-theming/home/blob/main/styling.md
[Base24]: https://github.com/tinted-theming/base24/blob/main/styling.md
[Tinted8]: https://github.com/tinted-theming/home/blob/specs/tinted8/styling.md
[Tinted Theming]: https://github.com/tinted-theming/home
[Starship]: https://starship.rs
[Base24 colors]: https://github.com/tinted-theming/base24/blob/main/styling.md#specific-colors-and-their-usages
[Tinted8 colors]: https://github.com/tinted-theming/home/blob/main/specs/tinted8/styling.md#palette-definition
[Base24 fallbacks]: https://github.com/tinted-theming/base24/blob/main/styling.md#base24-fallbacks
[Tinted8 theming properties]: https://github.com/tinted-theming/home/blob/main/specs/tinted8/styling.md#theming-properties
[Tinted8 Builder default colors]: https://github.com/tinted-theming/home/blob/main/specs/tinted8/builder.md#builder-default-colors
[style strings]: https://starship.rs/advanced-config/#style-strings
