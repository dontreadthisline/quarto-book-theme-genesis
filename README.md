# quarto-book-theme-genesis

中文教材风格的 [Quarto](https://quarto.org) 主题：litera 底座、无衬线正文 + 衬线标题、三栏布局（目录贴左缘、TOC 贴右缘）、阅读模式（收起两侧目录，右侧留白安置本章小节导航）。

## 安装与使用

```bash
quarto add dontreadthisline/quarto-book-theme-genesis
```

```yaml
---
title: 我的文档
format: genesis-book-html    # -html 后缀是 Quarto 定位扩展的约定，必须完整书写
---
```

## 主题包含

- **中文长文排版**：系统字体栈（PingFang SC / Noto Sans SC）、行高 1.85、衬线标题、教材风表格（上下粗边框去竖线）、块级公式横向滚动、行内公式基线修正
- **三栏布局**（≥992px）：目录面板贴视口左缘（无 Quarto 默认 70px inset）、右侧页内目录贴右缘、正文居中保 46rem 行长；窄屏回退 Quarto 原生抽屉
- **阅读模式**：目录面板右缘抽屉把手或按 `[` 键，收起两侧目录，正文 58rem 容器 + 右侧小节导航（scroll-spy 滚动高亮），localStorage 记忆

## 已知边界

- 数学公式走 Quarto 默认 MathJax CDN（联网正常）；完全离线需自行替换为本地自托管
- 开发与测试于 Quarto 1.8.27（`quarto-required: ">=1.4"`）

## 许可

MIT
