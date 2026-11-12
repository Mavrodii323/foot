# foot

My [foot](https://codeberg.org/dnkl/foot) terminal configuration — a single `foot.ini`, no external theme files.

## What's in it

| Setting | Value |
|---|---|
| Font | Agave Nerd Font, size 11 |
| Cursor | block, blinking |
| Scrollback | 5000 lines |
| Background | `#1c1c1c` at 50% alpha (`alpha=0.5`) |
| Foreground | `#ffffff` |
| Palette | Snazzy-style: red `ff5c57`, green `5af78e`, yellow `f3f99d`, blue `57c7ff`, magenta `ff6ac1`, cyan `9aedfe` |

## Install

```bash
mkdir -p ~/.config/foot
cp foot.ini ~/.config/foot/foot.ini
```

Restart foot, or for a config you already have running:

```bash
foot --reload   # or: footclient --reload
```

## Notes

- Alpha (`alpha=0.5`) requires a running compositor that supports transparency — on Hyprland it works out of the box.
- The font needs [Agave Nerd Font](https://github.com/ryanoasis/nerd-fonts) installed; otherwise foot falls back to a default.
- Requires foot 1.16+ for `[colors-dark]` (light/dark mode aware colors).
