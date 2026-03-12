# Ghostty Cursor Trails

## Demos

| Shader                              | Demo                                                                                                                       |
| --------                            | ------                                                                                                                     |
| Boo-Cursor                          | ![boo-cursor]([https://add-link](https://github.com/hced/ghostty-cursor-trails/raw/refs/heads/main/demos/boo-cursor.mp4))  |

> [!NOTE]
> If you are using the Line cursor (default in Ghostty), these effects will trigger and freeze when you unfocus the terminal (when the  cursor changes to hollow block). To prevent this from happening, add `custom-shader-animation = always` to your Ghostty config.

## Usage

1. Clone the repo into your ghostty shaders directory:
```bash
git clone https://github.com/hced/ghostty-cursor-trails ~/.config/ghostty/shaders
```

2. In your `~/.config/ghostty/config`, add your shader like so:
```config
custom-shader = shaders/boo-cursor.glsl
# ...
```

## Acknowledgements
Inspired by [Neovide](https://neovide.dev/) cursor animations and partially based on [ghostty-cursor-shaders](https://github.com/sahaj-b/ghostty-cursor-shaders).

## License

MIT
