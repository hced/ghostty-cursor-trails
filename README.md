# Ghostty Cursor Trails

Animated trail-effect for the text cursor in [Ghostty](https://ghostty.org/) terminal.

This repository currently features a **Boo-Cursor** shader designed to make it easier to track rapid cursor movement in general CLI use and editors like Vim/Neovim. Similar in look to the classic [Neovide](https://neovide.dev/), this effect is tuned to feel smooth, snappy and straight to the point.

## Boo-Cursor

https://github.com/user-attachments/assets/a65eabf1-0152-42a7-9e0c-e07448eeeb32

> [!NOTE]
> If you are using the Line cursor (default in Ghostty), the effects from this shader will freeze when you unfocus the terminal as the cursor becomes a hollow block). You can prevent this by adding `custom-shader-animation = always` in your Ghostty config.

## Usage

1. Clone the repo into your `~/.config/ghostty/shaders` directory:
```bash
git clone https://github.com/hced/ghostty-cursor-trails ~/.config/ghostty/shaders
```

2. Enable it by adding this line in your `~/.config/ghostty/config`:
```config
custom-shader = shaders/ghostty-cursor-trails/boo-cursor.glsl
# ...
```

3. Activate it by running this command line (Linux; use equivalent command for macOS/Windows):
```bash
systemctl reload --user app-com.mitchellh.ghostty.service  # reload Ghostty config
```

## Acknowledgements
Inspired by [Neovide](https://neovide.dev/) cursor animations and partly derived from [ghostty-cursor-shaders](https://github.com/sahaj-b/ghostty-cursor-shaders).

## License

MIT
