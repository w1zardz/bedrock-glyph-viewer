# Minecraft Bedrock Glyph Viewer & Explorer

**Online tool for viewing, searching, and exploring Minecraft Bedrock Edition glyph sheets (font textures).**

> **[Open Glyph Viewer](https://w1zardz.github.io/bedrock-glyph-viewer/)** — works on mobile and desktop

![Dark theme](https://img.shields.io/badge/theme-dark-0d1117?style=flat-square)
![Mobile ready](https://img.shields.io/badge/mobile-ready-3fb950?style=flat-square)
![No dependencies](https://img.shields.io/badge/dependencies-none-58a6ff?style=flat-square)

## Features

- **Multi-sheet loading** — load multiple glyph PNG sheets at once (drag & drop or file picker)
- **Unicode search** — search by hex code (e.g. `E100`) and instantly find the glyph across all loaded sheets
- **Cell detail view** — tap any glyph cell to see hex code, position, PHP/JSON escape code, zoomed preview
- **Unicode converter** — convert hex codes to PHP `\u{XXXX}`, JSON `\uXXXX`, and raw Unicode characters
- **Quick load buttons** — preconfigured buttons for common Bedrock glyph sheets (E0–E8, B7)
- **Copy to clipboard** — one-tap copy of Unicode characters and escape sequences
- **Mobile-first dark UI** — optimized for phones and tablets, fully responsive
- **Zero dependencies** — single HTML file, no frameworks, no build step, works offline

## Supported Glyph Sheets

Works with any Minecraft Bedrock Edition glyph sheet PNG:

| Sheet | Grid | Cell Size | Unicode Range | Common Content |
|-------|------|-----------|---------------|----------------|
| `glyph_E0.png` | 16x16 | 16px | U+E000–E0FF | Custom icons, UI elements |
| `glyph_E1.png` | 16x16 | 16px | U+E100–E1FF | Items, tools, resources |
| `glyph_E2.png` | 16x16 | 16px | U+E200–E2FF | Blocks, materials |
| `glyph_E4.png` | 16x16 | 16px | U+E400–E4FF | Misc icons |
| `glyph_E5.png` | 16x16 | 16px | U+E500–E5FF | Misc icons |
| `glyph_E6.png` | 16x16 | 64px | U+E600–E6FF | Large icons, rank badges |
| `glyph_E7.png` | 16x16 | 64px | U+E700–E7FF | Large icons |
| `glyph_E8.png` | 16x16 | 67px | U+E800–E8FF | Large icons, custom badges |
| `glyph_B7.png` | 16x16 | 32px | U+B700–B7FF | Server icons |

## How to Use

1. **Open the tool**: [w1zardz.github.io/bedrock-glyph-viewer](https://w1zardz.github.io/bedrock-glyph-viewer/)
2. **Load your glyph PNGs**: drag & drop files onto the page, or use the file picker
3. **Browse the grid**: tap any cell to see its Unicode code and copy it
4. **Search by Unicode**: enter a hex code like `E100` to find and highlight the glyph
5. **Convert codes**: use the converter to get PHP/JSON escape sequences

## Use in Minecraft Bedrock Plugins (PocketMine-MP)

```php
// PHP (PocketMine-MP plugin)
$icon = "\u{E100}"; // Insert glyph as Unicode character
$message = "\u{E164} You received gold!";
$player->sendMessage($message);
```

```json
// JSON (resource pack UI, lang files)
{ "text": "\uE100 Custom icon" }
```

## For Server Developers

This tool is essential for **Minecraft Bedrock server developers** working with:

- **PocketMine-MP** (PMMP) plugins
- **Resource pack** glyph customization
- **Custom UI** with FormAPI, ScoreboardAPI
- **Server branding** with custom icons and rank badges
- **Nukkit** / **PowerNukkitX** servers

## Self-Hosting

Single HTML file — just download and open:

```bash
git clone https://github.com/w1zardz/bedrock-glyph-viewer.git
cd bedrock-glyph-viewer
open index.html
```

## Alternative to

- [nhanaz.github.io/glyph](https://nhanaz.github.io/glyph/) — the original inspiration
- This version adds: **multi-sheet support**, **Unicode search**, **mobile optimization**, **dark theme**

## Topics

`minecraft` `bedrock` `glyph` `glyph-viewer` `mcbe` `pocketmine` `pmmp` `resource-pack` `font` `unicode` `minecraft-bedrock` `bedrock-edition` `glyph-explorer` `minecraft-tools`

## License

MIT

---

Made for the Minecraft Bedrock community.
