![UV Carry](assets/hero/uv-carry-hero.png)

https://github.com/user-attachments/assets/814005e5-9117-4d86-b45c-b37a2d7fc038

# UV Carry

**Move UVs. Carry Textures.**

English · [Português (Brasil)](README.pt-BR.md)

A Blender 5.1 add-on that keeps the texture with the UVs. Move, rotate, scale or pack UV islands with Blender's own tools, press `Ctrl+Enter`, and every texture of their materials follows them. Merge the islands of many materials into one atlas in a single step.

- **Your tools, your shortcuts.** G, R, S and UV > Pack Islands stay Blender's. Nothing is written while you move; the texture work happens once, at `Ctrl+Enter`.
- **Every map at once.** Colour, packed ORM channels, alpha and tangent-space normal maps, which keep their relief when an island turns.
- **Merge materials into one atlas.** Set a material as Carry Into, pack the islands and press `Ctrl+Enter`: every channel of the atlas takes what each island's own material gives it.
- **Several islands at once**, each under its own move. `Ctrl+Enter` with no move pads the selected islands instead.
- **Undo and save.** `Ctrl+Z` restores the texels, the UVs and the materials together; Save Carried Images writes the changed images, after a backup of each file.
- **Nothing silent.** What cannot be carried exactly is refused before anything is written, with a message that names the material and the input.

## In numbers

A kitbashed character of 7 materials, carried into one atlas with one `Ctrl+Enter`:

| | Before | After |
| --- | --- | --- |
| Materials | 7 | 1 |
| Textures | 22 | 3 |
| Texture memory | 677 MB | 128 MB |
| UV islands carried | | 1,802 |

## How it works

![How a carry works](assets/how/how-it-works.svg)

UV Carry remembers where the islands started, lets Blender move them as it always does, and at `Ctrl+Enter` carries each island's texels from where it started to where it ended. A move by whole texels is copied bit for bit; rotations and scales are resampled from the island's own texels only, so nothing bleeds in from a neighbour.

## UV Carry and UV Carry Lite

| | [UV Carry Lite](https://github.com/ghbanck/UV-Carry-Lite) | UV Carry |
| --- | :---: | :---: |
| Move, rotate and scale islands with G, R and S | ✓ | ✓ |
| Several islands at once, and padding | ✓ | ✓ |
| UV > Pack Islands | | ✓ |
| Tangent-space normal maps | | ✓ |
| Carry Into: many materials into one atlas | | ✓ |

## Pricing

Every tier is the same add-on with every feature, and includes lifetime updates.

| Tier | Artists | Price |
| --- | --- | --- |
| Individual | 1 | US$ 39 |
| Small Studio | up to 5 | US$ 99 |
| Studio | up to 15 | US$ 199 |
| Production | up to 50 | US$ 399 |

A tier is the price for a team of its size, and pays for every update, support and the official build. It does not limit what the GPL lets anyone do with the code: there is no activation, no license server and no hardware lock, and studios buy the tier that covers their artists, on trust. Each release is a versioned zip with its SHA-256, so a studio can pin a version in its own pipeline and roll back.

## Requirements

Blender 5.1. Tested with Blender 5.1.1 on Windows 11.

## License

Copyright (C) 2026 Gustavo Banck. The add-on's code is licensed under the GNU General Public License, version 3 or any later version, and comes with it.

The GPL covers the code, not the names: "UV Carry", "UV Carry Lite" and the UV Carry logo are the author's. A modified or redistributed copy keeps every right the GPL gives, but must not be called by these names or carry the logo.
