![UV Carry](assets/hero/uv-carry-hero.png)

# UV Carry

**Move UVs. Carry Textures.**

English · [Português (Brasil)](README.pt-BR.md)

A Blender 5.1 add-on that keeps the texture with the UVs. Move, rotate, scale or pack UV islands with Blender's own tools, press `Ctrl+Enter`, and every texture of their materials follows them. Merge the islands of many materials into one atlas in a single step.

<p align="center">
  <a href="assets/store/uv-carry-store.mp4"><img src="assets/store/featured.png" alt="UV Carry: 13 materials and 32 textures into one atlas" width="100%"></a>
  <br>
  <a href="assets/store/uv-carry-store.mp4"><b>▶ Watch the video</b></a> (77 seconds)
</p>

- **Your tools, your shortcuts.** G, R, S and UV > Pack Islands stay Blender's. Nothing is written while you move; the texture work happens once, at `Ctrl+Enter`.
- **Every map at once.** Colour, packed ORM channels, alpha and tangent-space normal maps, which keep their relief when an island turns.
- **Merge materials into one atlas.** Set a material as Carry Into, pack the islands and press `Ctrl+Enter`: every channel of the atlas takes what each island's own material gives it.
- **Several islands at once**, each under its own move. `Ctrl+Enter` with no move pads the selected islands instead.
- **Undo and save.** `Ctrl+Z` restores the texels, the UVs and the materials together; Save Carried Images writes the changed images, after a backup of each file.
- **Nothing silent.** What cannot be carried exactly is refused before anything is written, with a message that names the material and the input.

## In numbers

Eight props, carried into one atlas with one `Ctrl+Enter`:

| | Before | After |
| --- | --- | --- |
| Materials | 13 | 1 |
| Textures | 32 | 3 |
| Texture memory | 512 MB | 96 MB |
| UV islands carried | | 1,715 |

![The UV editor and the UV Carry panel after the carry](assets/store/gallery_panel.png)

![The atlas: colour, ORM and normal](assets/store/gallery_atlas.png)

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

## Licenses

Coming soon. Every license is the same add-on with every feature, and includes lifetime updates.

| License | Artists | Price |
| --- | --- | --- |
| Individual | 1 | US$ 39 |
| Small Studio | up to 5 | US$ 99 |
| Studio | up to 15 | US$ 199 |
| Production | up to 50 | US$ 399 |

A seat is a person, not a machine: no activation, no license server, no hardware lock. Each release is a versioned zip with its SHA-256, so a studio can pin a version in its own pipeline and roll back. UV Carry is licensed under the GPL, version 3 or later.

## Requirements

Blender 5.1. Tested with Blender 5.1.1 on Windows 11.

## Credits

The props in the images and the video are from Poly Haven (CC0): Television 01, Boombox, Camera 01, Alarm Clock 01, Rubber Duck Toy, Ukulele 01, Food Apple 01 and Potted Plant 04.

Copyright (C) 2026 Gustavo Banck.
