# Ob_Theme — NXL Obsidian 模板仓库

本仓库是一个自用的 **Obsidian 模板配置仓库**，集成了常用插件和自建主题 NXL，开箱即用。

---

## 🎨 主题

| 主题 | 说明 |
|------|------|
| **NXL** | 自建主题，支持双配色方案 + Style Settings 全面调节 + bloom-stone 装饰特性 |
| Blue Topaz | 社区热门主题，配色丰富，作为 NXL 的设计参考 |
| Composer | 简洁风格主题 |
| MyTheme | 旧版试验主题（保留） |

当前默认启用主题：**NXL**

### NXL 主题特性

- **双配色方案**：通过 Style Settings 切换
- **Ink**（Blue Topaz 风格，白底蓝强调）
- **Orange Heart**（橙红暖色 + 衬线字体 + 特殊 H2 标签样式）
- **Style Settings 全面支持**：无需手写 CSS，在设置面板即可切换配色、调整字体、开关装饰、覆盖颜色
- **字体架构**：参照 Blue Topaz 的设计，正文字体直接作用于内容容器，不干预 UI 组件字体，兼容性更好
- **bloom-stone 装饰风格**：背景渐变、页面卡片、标题下划线（H1 虚线 / H2-H4 实线）、代码块 Mac 圆点
- **H1 对齐**：左对齐 / 居中 / 右对齐
- **颜色覆盖**：可单独自定义强调色、内联代码色、加粗/斜体颜色

---

## 🔌 已集成插件

| 插件 | 说明 |
|------|------|
| **Style Settings** | 主题样式可视化调节面板（NXL 的核心依赖） |
| **Dataview** | 将仓库视为数据库，支持类 SQL 查询和动态列表 |
| **Editing Toolbar** | 编辑模式下提供浮动格式工具栏 |
| **cmdr** | 自定义 Obsidian 界面中的命令按钮 |
| **Easy Typing** | 优化中文输入体验，自动加空格、修正标点 |
| **Table Editor** | 增强的表格编辑功能 |
| **OZ Clear Unused Images** | 清理未使用的图片附件 |
| **Recent Files** | 显示最近打开的文件列表 |
| **Cycle Through Panes** | 使用快捷键循环切换面板 |
| **Obsidian Linter** | Markdown 文件格式化与 lint 检查 |
| **Open Tab Settings** | 在新标签页中打开设置面板 |

---

## 🚀 使用方式

1. 克隆本仓库到本地
2. 在 Obsidian 中「打开本地仓库」选择此文件夹
3. 进入 `设置 → 外观 → 主题`，选择 **NXL**
4. 安装并启用 **Style Settings** 插件（已内置）
5. 在 `Style Settings` 面板中：
   - **配色方案**：切换 Ink / Orange Heart
   - **排版设置**：调整字体、字号、行高、H1 对齐
   - **装饰样式**：开关背景渐变、页面卡片、标题下划线、代码圆点
   - **颜色覆盖**：自定义强调色、内联代码色等

---

## 📁 目录结构

```
.obsidian/
├── themes/
│   ├── NXL/              # 自建主题（主力）
│   ├── Blue Topaz/       # Blue Topaz 主题（设计参考）
│   ├── Composer/         # Composer 主题
│   └── MyTheme/          # 旧版试验主题
├── plugins/              # 已安装的社区插件
└── appearance.json       # 外观配置（默认主题: NXL）

Css/                      # 额外样式源文件（空，备用）
```

---

---

## 📝 更新日志

| 日期 | 版本 | 内容 |
|------|------|------|
| 2025-06 | — | 重构字体架构：参照 Blue Topaz，`--font-text` 直接设置、`--font-interface` 不再覆盖、内容容器 `font-family: var(--font-text)`；修复 tooltip 矩形框问题（颜色改用 `--text-normal`，移除全局 `*` 过渡规则） |

*个人配置仓库，持续更新中。*
