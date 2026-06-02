# Awesome Design MD

> 一个精选的设计系统分析库，收集了 **Stripe**、**Linear**、**Figma**、**Ferrari** 等顶级品牌的 DESIGN.md 文档。将这些文件放入项目中，让 AI 编码助手可以生成符合品牌风格的 UI。

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![GitHub Stars](https://img.shields.io/github/stars/dahong2799/sjxg?style=social)](https://github.com/dahong2799/sjxg)

## 📚 概述

本仓库包含对世界一流品牌设计系统的深度分析，如 **Stripe**、**Linear**、**Figma**、**Ferrari**、**Airbnb**、**Apple**、**Airtable** 等。

每个品牌都有一个 `DESIGN.md` 文件，文档内容包括：

- **色彩系统** — 品牌调色板和语义 token
- **字体排版** — 字体族、字体规模和层级
- **布局与间距** — 栅格系统和节奏
- **组件规范** — 按钮、卡片、输入框及其完整规格
- **响应式行为** — 断点和折叠策略
- **设计哲学** — "应做事项"和"禁忌事项"原则

这些文件是 **AI 友好的** — AI 编码助手可以直接读取 DESIGN.md 并生成符合品牌语音的 UI 组件，无需查看任何线框图或设计稿。

## 🎨 品牌列表

| 品牌 | 状态 | 文件 | 描述 |
|------|------|------|------|
| Stripe | 🔄 进行中 | — | 现代支付平台，极简主义设计 |
| Linear | 🔄 进行中 | — | 高效工作工具，精简风格 |
| Figma | 🔄 进行中 | — | 协作设计平台，渐进式风格 |
| Ferrari | 🔄 进行中 | — | 超级跑车品牌，奢侈设计 |
| Airbnb | ✅ 完成 | [`design-md/airbnb/DESIGN.md`](./design-md/airbnb/DESIGN.md) | 摄影驱动的市场，温暖的 Rausch 强调色 |
| Apple | ✅ 完成 | [`design-md/apple/DESIGN.md`](./design-md/apple/DESIGN.md) | 产品至上的 UI，极简主义风格 |
| Airtable | ✅ 完成 | [`design-md/airtable/DESIGN.md`](./design-md/airtable/DESIGN.md) | 编辑工作软件，标志性表面卡片 |

## 📄 DESIGN.md 格式

每个 `DESIGN.md` 都是结构化的 YAML + Markdown 文档：

```yaml
---
version: alpha
name: Brand-Name-design-analysis
description: 品牌风格概述

colors:
  primary: "#0066cc"
  surface: "#ffffff"
  # ... 语义 token

typography:
  display:
    fontFamily: "SF Pro Display"
    fontSize: 56px
    fontWeight: 600
    lineHeight: 1.07

rounded:
  sm: 8px
  md: 12px
  lg: 16px

spacing:
  xs: 4px
  sm: 8px
  md: 16px

components:
  button-primary:
    backgroundColor: "{colors.primary}"
    textColor: "{colors.on-primary}"
    typography: "{typography.button}"
---

## 概述
[品牌设计理念]

## 色彩
[详细的色彩说明及语义含义]

## 字体排版
[字体层级和原则]

## 组件
[组件逐项细分]

## Do's and Don'ts
[品牌防护栏]
```

## 🚀 如何使用

### 给 AI 代理使用

```
加载: /design-md/{brand}/DESIGN.md
任务: 生成符合设计系统的 React 组件
结果: 组件遵循所有设计 token 和品牌原则
```

### 给设计师使用

- 参考任何 `DESIGN.md` 深入理解品牌系统
- 在竞争对手分析之前用作简报文档
- 复制格式来记录你自己的设计系统

### 给开发者使用

- 提取颜色/排版 token 来构建 CSS 设计 token
- 构建组件库时参考组件规格
- 用作响应式断点和间距的单一事实来源

## 🤝 贡献

我们欢迎贡献！要添加新品牌：

### 分析步骤

1. **Fork** 本仓库
2. **创建分支**: `git checkout -b design/your-brand`
3. **分析设计系统**：
   - 访问品牌网站（营销 + 产品）
   - 使用浏览器开发者工具检查颜色、字体、间距
   - 按 DESIGN.md 格式记录 token 和组件
4. **文件位置**: `design-md/{brand-slug}/DESIGN.md`
5. **更新 README** 添加你的新品牌
6. **提交 PR**，附带清晰的分析描述

### 分析检查清单

- [ ] 色彩已提取并进行语义命名
- [ ] 字体规模已记录，包含字体堆栈
- [ ] 间距/栅格系统已识别
- [ ] 已记录 5 个以上关键组件
- [ ] 已注记响应式行为
- [ ] 已编写 "Do's and Don'ts" 部分
- [ ] 文件通过 linter: `npx @google/design.md lint DESIGN.md`

参考 [CONTRIBUTING.md](./CONTRIBUTING.md) 获取详细的分析指南。

## 💡 示例

### 编程方式提取 Token

```javascript
const design = require('./design-md/apple/DESIGN.md');

const colors = design.colors;
const typography = design.typography;
const spacing = design.spacing;

// 在组件库中使用
export const colors = { ...colors };
export const typography = { ...typography };
```

### 在设计中参考

```markdown
查看 Stripe 的设计？检查 `stripe/DESIGN.md` 获取：
- 主品牌色: `{colors.primary}`
- 按钮规格: `{component.button-primary}`
- 响应式断点: 手机 < 768px，平板 < 1024px，桌面 ≥ 1024px
```

## 📋 项目结构

```
sjxg/
├── README.md                          # 本文件
├── CONTRIBUTING.md                    # 贡献指南
├── LICENSE                            # MIT 许可证
└── design-md/
    ├── airbnb/
    │   └── DESIGN.md
    ├── apple/
    │   └── DESIGN.md
    ├── airtable/
    │   └── DESIGN.md
    ├── stripe/                        # 待添加
    ├── linear/                        # 待添加
    ├── figma/                         # 待添加
    └── ferrari/                       # 待添加
```

## 📖 核心概念

### 什么是 DESIGN.md？

DESIGN.md 是一个**结构化的设计系统文档**，用 YAML frontmatter 定义设计 token（颜色、字体、间距），然后用 Markdown 提供语境性的解释和最佳实践。

### 为什么是 DESIGN.md？

- **AI 可读** — 清晰的 YAML 结构让 AI 代理可以解析和应用 token
- **人类友好** — Markdown 部分提供设计理念和使用指南
- **可版本控制** — 纯文本格式适合 Git 跟踪
- **可继承** — `{token.ref}` 语法允许组件引用其他 token

### Token 引用系统

```yaml
components:
  button-primary:
    backgroundColor: "{colors.primary}"         # 引用色彩 token
    textColor: "{colors.on-primary}"            # 引用色彩 token
    typography: "{typography.button}"           # 引用排版 token
    rounded: "{rounded.md}"                     # 引用圆角 token
    padding: "{spacing.md} {spacing.lg}"        # 引用间距 token
```

所有组件都是基础 token 的组合，确保系统的一致性。

## 🔗 相关资源

- [VoltAgent/awesome-design-md](https://github.com/VoltAgent/awesome-design-md) — 原始精选集
- [Google Design Tokens](https://github.com/google/design-tokens) — Token 标准化
- [Design System Checklist](https://www.designsystemchecklist.com/) — 设计系统最佳实践
- [Design.md Spec](https://github.com/google/design.md) — 官方规范

## 📝 许可证

MIT — 可自由用于商业和个人项目。参见 [LICENSE](./LICENSE)

## 👤 维护者

- [@dahong2799](https://github.com/dahong2799) — 创建者

---

**有问题？** 开启一个 [issue](https://github.com/dahong2799/sjxg/issues)。
**有品牌分析？** 提交 [PR](https://github.com/dahong2799/sjxg/pulls)。
**想合作？** 开启一个讨论。

**让我们一起建立一个开源设计系统库！** 🚀
