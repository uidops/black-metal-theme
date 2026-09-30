# Black Metal — Zed theme

A Zed port of [metalelf0/black-metal-theme-neovim](https://github.com/metalelf0/black-metal-theme-neovim),
the Black Metal colorscheme collection for Neovim.

**128 themes** — 16 bands × 4 variants, each with an opaque and a transparent-blur version:

| | variants |
|---|---|
| Bands | Bathory, Burzum, Dark Funeral, Darkthrone, Emperor, Gorgoroth, Immortal, Impaled Nazarene, Khold, Marduk, Mayhem, Nile, Taake, Thyrfing, Venom, Windir |
| Each band | `dark`, `dark Alt`, `light`, `light Alt` |
| Each variant | opaque + `Blur` |

Every theme name is prefixed with `BlackMetal`, e.g. `BlackMetal Burzum`,
`BlackMetal Burzum Light Alt`, `BlackMetal Burzum Light Alt Blur`.

## Blur variants

The `Blur` themes use one 72%-opaque
tint layer (`background`, `surface.background`, `status_bar`, `title_bar`) over
Zed's blurred window, with every layer *inside* the window set to fully
transparent `#00000000` — editor, gutter, panels, tabs, borders, scroll tracks.
That way the whole window shows the same ~28% of the blurred desktop with no
seams, while text, syntax, line numbers, guides and terminal ANSI colors stay
fully opaque and crisp.

Blur only renders where macOS allows window transparency: turn off
**System Settings → Accessibility → Display → Reduce transparency**, and expect
the effect to only show over other windows rather than over the desktop
wallpaper.

## Install

Clone this repository, then in Zed open the command palette and run
`extensions: install dev extension`, selecting the clone.

Or skip extensions entirely and copy the theme file into your user themes
directory:

```bash
mkdir -p ~/.config/zed/themes
cp themes/black-metal.json ~/.config/zed/themes/
```

Either way, pick a theme from the command palette with `theme selector: toggle`.

## Credits

- Original palettes, highlight groups and terminal colors:
  [metalelf0/black-metal-theme-neovim](https://github.com/metalelf0/black-metal-theme-neovim)
- Ported to the [Zed](https://zed.dev) theme format
  ([schema v0.2.0](https://zed.dev/schema/themes/v0.2.0.json)).

## License

Apache 2.0 — see [LICENSE](LICENSE), same as the upstream Neovim theme.
