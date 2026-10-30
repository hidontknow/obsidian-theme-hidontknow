# Hidontknow

一款简洁的 Obsidian 主题，支持亮色 / 暗色。设计参考了 [Phycat](https://github.com/sumruler/obsidian-theme-phycat) 的标题装饰和 [Blue Topaz](https://github.com/whyt-byte/Blue-Topaz_Obsidian-css) 的配色与组件风格，文件列表样式改编自 Phycat（MIT），其余为原创实现。

## 特性

- **标题**：H1 居中，带渐变下划线（悬停变长）；H2 渐变胶囊；H3 左侧色条；H4 强调色。阅读模式和编辑模式外观一致，长标题换行后仍是完整的胶囊，编辑时点击定位准确。
- **段落间距**：阅读模式按编辑模式的空行排版，块与块之间隔一个空行的高度，两种模式切换时内容基本不跳动。
- **正文**：粗体为强调色，引用块有浅色背景，行内代码为强调色，代码块左侧带色条，表格圆角并隔行变色，分割线为渐变。
- **文件列表**：沿用 Phycat 样式，圆角标题行、彩虹文件夹（顶层文件夹按 7 色轮换）、文件夹/文件/图片/Canvas/Base 图标、细层级线。
- **其他**：标签做成胶囊样式，外链不显示末尾箭头图标，Callout 左侧带色条，已完成的任务文字变淡。
- 尊重系统的「减少动态效果」设置。

## 安装

1. 在库的 `.obsidian/themes/` 下新建文件夹 `Hidontknow`。
2. 把 `theme.css` 和 `manifest.json` 复制进去（开发时可以用软链接）。
3. 打开 **设置 → 外观 → 主题**，选择 **Hidontknow**。

## 改色

强调色由 `--accent-h/s/l` 推导，主题为亮色和暗色分别设了默认值。想换颜色，可以新建一个 CSS 片段：

```css
.theme-light { --accent-h: 340; --accent-s: 75%; --accent-l: 55%; }
.theme-dark  { --accent-h: 340; --accent-s: 70%; --accent-l: 65%; }
```

暗色下 H2 胶囊用深色文字，所以暗色的 `--accent-l` 建议保持在 60% 以上。

## 配套插件：Pele Mermaid（试验）

插件 [Pele Mermaid](https://github.com/hidontknow/obsidian-pele-mermaid) 用 [Pele](https://github.com/obsidianmd/pele) 代替内置的 mermaid.js 渲染 Mermaid 图。主题已为 Pele 的图适配亮色 / 暗色配色；不装插件时，Mermaid 图照常由 mermaid.js 渲染。

## 开发

```bash
npm install
npm run lint
```

## 致谢

- [Blue Topaz](https://github.com/whyt-byte/Blue-Topaz_Obsidian-css)，MIT，© whyt-byte
- [Phycat](https://github.com/sumruler/obsidian-theme-phycat)，MIT，© XuJilong
