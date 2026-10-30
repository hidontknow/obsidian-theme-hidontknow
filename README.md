# Hidontknow

English | [简体中文](README.zh-CN.md)

A clean Obsidian theme with light and dark modes. Reading view and editing view look the same. The heading styles draw on [Phycat](https://github.com/sumruler/obsidian-theme-phycat), and the colors and components draw on [Blue Topaz](https://github.com/whyt-byte/Blue-Topaz_Obsidian-css). The file explorer styles are adapted from Phycat (MIT); everything else is original.

Requires Obsidian 1.14.0 or later.

![Hidontknow in light mode](screenshots/screenshot.png)

## Features

- **Headings**: H1 is centered with a gradient underline that grows on hover. H2 is a gradient pill. H3 has a colored bar on the left. H4 uses the accent color. Headings look the same in reading and editing view, long H2 headings stay one pill when they wrap, and clicking a heading in the editor places the cursor correctly.
- **Spacing**: Reading view uses the same spacing as editing view, with one blank line between blocks, so content barely moves when you switch views.
- **Text**: Bold text and inline code use the accent color. Blockquotes have a tinted background. Code blocks have an accent bar on the left. Tables have rounded corners and striped rows. Horizontal rules use a gradient.
- **Code highlighting**: Reading view (Prism) and editing view (CodeMirror) use the same colors for keywords, strings, numbers, comments and attributes.
- **File explorer**: Rounded rows, rainbow folders (top-level folders cycle through 7 colors) and thin indent guides. File icons show the file type: notes, images, PDF, audio, video, code, Office documents / spreadsheets / presentations, archives, Canvas, Base and Excalidraw. Files and folders line up.
- **Other**: Tags are pills, external links have no trailing arrow icon, callouts have a colored bar on the left, and completed tasks are dimmed.
- Respects the system "reduce motion" setting.

## Installation

Search for **Hidontknow** in **Settings → Appearance → Themes → Manage** (once the theme is listed in the theme directory).

Manual installation:

1. Create a folder named `Hidontknow` in your vault's `.obsidian/themes/` folder.
2. Copy `theme.css` and `manifest.json` into it.
3. Open **Settings → Appearance → Themes** and select **Hidontknow**.

## Changing the accent color

The accent color comes from `--accent-h/s/l`, and the theme sets separate defaults for light and dark mode. To use another color, add a CSS snippet:

```css
.theme-light { --accent-h: 340; --accent-s: 75%; --accent-l: 55%; }
.theme-dark  { --accent-h: 340; --accent-s: 70%; --accent-l: 65%; }
```

In dark mode the H2 pill uses dark text, so keep the dark `--accent-l` at 60% or higher.

## Companion plugin: Pele Mermaid (experimental)

The [Pele Mermaid](https://github.com/hidontknow/obsidian-pele-mermaid) plugin renders Mermaid diagrams with [Pele](https://github.com/obsidianmd/pele) instead of the built-in mermaid.js. The theme colors Pele diagrams for light and dark mode. Without the plugin, Mermaid diagrams are rendered by mermaid.js as usual.

## Development

```bash
npm install
npm run lint
```

## Credits

- [Blue Topaz](https://github.com/whyt-byte/Blue-Topaz_Obsidian-css), MIT, © whyt-byte
- [Phycat](https://github.com/sumruler/obsidian-theme-phycat), MIT, © XuJilong

## License

[MIT](LICENSE) © hidontknow. The file explorer styles are adapted from Phycat (MIT) and the file explorer icons come from [Lucide](https://lucide.dev) (ISC). See [THIRD-PARTY-NOTICES.md](THIRD-PARTY-NOTICES.md) for their licenses.
