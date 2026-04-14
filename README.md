# Ghostty Cursor Trails

Animated trail-effect for the text cursor in [Ghostty](https://ghostty.org/) terminal.

This repository features shaders designed to make it easier to track rapid cursor movement in your terminal and editors like Neovim. Reminiscent of the classic [Neovide](https://neovide.dev/), these shaders are tuned to feel snappy and to the point. ;)

## Tinkle

**Tinkle** provides a bunch of cool configuration options, and **Wisp** is a specially configured version of Tinkle (used by the author).

https://github.com/user-attachments/assets/e5e4d654-5c4f-41f7-acaa-9851c3aab190

## Boo

**Boo** should be quite nice as well, but has less tweakable features than Twinkle.

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
Inspired by [Neovide](https://neovide.dev/) cursor animations and partly derived from [ghostty-cursor-shaders](https://github.com/sahaj-b/ghostty-cursor-shaders) (Boo-Cursor).

## License

MIT
