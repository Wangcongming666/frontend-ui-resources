# 🎨 Frontend UI Resources

> 让 AI 在做界面时，快速找到用得上的设计参考、组件和素材。
>
> **73 个资源入口 · 按场景检索 · npx 安装 · 中文说明**

[![Resources](https://img.shields.io/badge/resources-73-2563eb)](#resources)
[![Skill](https://img.shields.io/badge/Agent_Skill-frontend--ui--resources-0f766e)](SKILL.md)
[![Install](https://img.shields.io/badge/install-npx-334155)](#install)

**frontend-ui-resources** 是一个面向 AI 编程助手的前端 UI 资源导航 Skill。它根据页面需求、现有技术栈和预算，从分类目录中筛选合适的资源，并说明用在哪里、如何获取、怎么接入，以及费用和授权条件。

适合正在做落地页、作品集、SaaS 或后台界面的开发者，也适合想让 AI 帮忙查找组件、动效和视觉素材的设计师。

<a id="quick-start"></a>
## ⚡ 一条命令开始使用

在项目目录运行，按提示选择目标助手：

```bash
npx skills add Wangcongming666/frontend-ui-resources
```

安装后，在助手中输入：

```text
使用 frontend-ui-resources，为我的 SaaS 落地页找极简风格参考、
适合现有技术栈的组件，以及免费可商用的插画。给我 5 项以内，说明用途和使用条件。
```

默认安装到当前项目；跨项目使用的安装方式见下方。运行 CLI 前需安装 Node.js，当前版本要求见 [Skills CLI 官方说明](https://github.com/vercel-labs/skills#install-a-skill)。

## 🧭 快捷导航

| 想做什么 | 从这里开始 |
|---|---|
| 安装给 Codex、Claude Code 或当前项目 | [安装方式](#install) |
| 看这个 Skill 能解决哪些问题 | [适用场景](#scenarios) |
| 浏览收录的资源类型 | [资源分类](#resources) |
| 复制提示词开始查资源 | [使用示例](#examples) |
| 了解 AI 会返回什么 | [工作方式与输出](#workflow) |
| 查看文件结构、来源与维护方式 | [目录与维护](#maintenance) |
| 确认离线、许可与下载行为 | [使用说明](#notes) |

<a id="scenarios"></a>
## 🎯 什么时候用

| 你的需求 | Skill 会重点查找 |
|---|---|
| 新做一个品牌站或作品集，先确定视觉方向 | 整站案例、版式、排版和交互参考 |
| 只想改好首屏、导航或页脚 | 对应区块的参考图库 |
| 给 SaaS 或后台补齐表单、弹窗、数据界面 | 与现有框架匹配的组件及真实产品流程 |
| 找到一个效果，希望有代码可以接入 | 具体动效示例、源码入口、依赖与许可 |
| 页面缺图标、插画、字体或背景视频 | 匹配视觉方向和格式的素材来源 |
| 资源必须免费、可商用，或无需署名 | 分别核查费用、商用范围和署名要求 |

**先看项目再选资源。** 已有设计系统和依赖优先复用；Vue 项目会检查 Vue 兼容性，要求源码时会继续寻找具体示例，而不只给截图或站点首页。

<a id="install"></a>
## 📦 安装方式

### 使用 npx 安装

[Skills CLI](https://github.com/vercel-labs/skills) 可直接从 GitHub 仓库发现技能，无需将本仓库发布为 npm 包。

```bash
# 安装到当前项目，交互选择目标助手
npx skills add Wangcongming666/frontend-ui-resources

# 全局安装给 Codex，跨项目使用
npx skills add Wangcongming666/frontend-ui-resources -a codex -g

# 全局安装给 Claude Code，跨项目使用
npx skills add Wangcongming666/frontend-ui-resources -a claude-code -g

# 只查看仓库中的技能，不安装
npx skills add Wangcongming666/frontend-ui-resources --list
```

本仓库默认分支为 `master`。`-a` 指定目标助手，`-g` 指定全局安装；省略 `-g` 时安装到当前项目。其他助手和参数见 [CLI 安装文档](https://github.com/vercel-labs/skills/blob/main/docs/commands.md#skills-add)。

<details>
<summary>手动下载或使用 Git 安装</summary>

可直接[下载 master 分支 ZIP](https://github.com/Wangcongming666/frontend-ui-resources/archive/refs/heads/master.zip)，解压后将文件夹命名为 `frontend-ui-resources`，放入目标助手的技能目录，并保留 `SKILL.md`、`agents/` 和 `references/` 的相对位置。

也可以使用 Git。例如，下载到个人 Codex 技能目录：

```bash
git clone --branch master https://github.com/Wangcongming666/frontend-ui-resources.git ~/.codex/skills/frontend-ui-resources
```

目标目录已有同名技能时，先检查已有内容，避免覆盖本地修改。

</details>

<a id="resources"></a>
## 🗂️ 资源分类

目录包含 **73 个不重复的资源入口**。下面列出各类代表资源，完整条目、检索提示和核验记录见分类索引。

| 分类 | 覆盖内容 | 代表资源 | 完整索引 |
|---|---|---|---|
| 页面与区块灵感 | 整站、Hero、导航、页脚、后台及产品流程 | Godly、Land-book、Mobbin、Refero | [页面灵感](references/inspiration.md) |
| 设计系统与组件 | Figma kit、设计规范、代码组件、交互原语、CSS 框架 | shadcn/ui、Headless UI、Ant Design、Carbon | [组件与规范](references/components.md) |
| 动效与特效 | 源码示例、时间轴、滚动叙事、状态机及 3D | Codrops、CodePen、Motion、GSAP、Three.js | [动效资源](references/motion.md) |
| 配色与视觉素材 | 配色、渐变、图标、字体、插画、图片及视频 | Coolors、Lucide、Fontsource、unDraw、Pexels | [视觉素材](references/assets.md) |

部分资源会出现在多个使用场景中，资源总数按入口 URL 去重。内容聚焦 UI 设计与实现，不包含学习路线、课程和后端工具链。

<a id="examples"></a>
## 💬 复制这些提示词开始用

### 给落地页找方向

```text
使用 frontend-ui-resources，为一个独立开发者工具找落地页参考。
风格克制、以排版为主，重点看 Hero、功能介绍和定价区块。
给 3 个合适的参考，并指出各自值得借鉴的布局与信息层级。
```

### 给现有项目找组件和插画

```text
使用 frontend-ui-resources，给 Vue 3 后台找表单、弹窗和空状态资源。
保留当前技术栈，组件需要支持 Vue；插画必须免费可商用且无需署名。
分别说明哪些条件已核实，哪些仍待确认。
```

### 找可接入的动效源码

```text
使用 frontend-ui-resources，找 3 个有源码的图片转场示例，用于作品集。
项目是原生 HTML/CSS/JS，需要兼顾移动端和减少动态效果偏好。
请给具体 demo 和源码入口，说明依赖、许可及接入成本。
```

### 让 AI 在实现前先选资源

```text
使用 frontend-ui-resources，先检查当前项目的技术栈与设计系统，
再为产品介绍页选择合适的图标、字体和背景素材，并继续完成页面实现。
优先复用已有依赖，说明新增资源的选择理由。
```

<a id="workflow"></a>
## 工作方式与输出

技能按需求读取相关分类，通常给出 3–5 项匹配资源；指定数量时遵从你的要求。需要最新信息时核查入选项，只有要求具体示例或素材时才继续定位到详情页。

| 输出内容 | 你能得到什么 |
|---|---|
| 资源链接 | 官网、具体案例、组件、demo、源码或素材详情入口 |
| 适用位置 | 资源如何服务于当前页面，而不只是一个名称 |
| 获取与接入 | 内容类型、框架兼容性、格式、依赖及使用方式 |
| 核验与条件 | 已确认的范围，以及费用、署名和许可等待确认项 |
| 推荐组合 | 适合当前任务的搭配及选择理由 |

找资源时会区分**灵感截图、Figma 文件、可复制源码、运行时库和素材文件**。要求“可直接复制”时，会定位代码或下载入口；仅能提供站点首页时，会注明它是查找入口。

<a id="maintenance"></a>
## 目录与维护

```text
frontend-ui-resources/
├── README.md                 # 安装、场景与使用说明
├── SKILL.md                  # AI 读取的技能入口
├── agents/
│   └── openai.yaml           # 技能展示信息
└── references/
    ├── inspiration.md       # 页面与区块灵感
    ├── components.md        # 设计系统与组件
    ├── motion.md            # 动效与源码
    └── assets.md            # 配色与视觉素材
```

资源基于前端设计资源清单筛选整理。部分许可、产品名称和访问状态于 **2026-11-14** 核验并修正，具体记录见分类索引；其余条目作为候选入口，在实际入选时确认当前状态。

欢迎通过 [Issue](https://github.com/Wangcongming666/frontend-ui-resources/issues) 或 Pull Request 补充资源、修正链接。新增条目请附上官方地址、适用场景、可获取的内容类型，以及已确认的费用或授权条件；更正状态时请注明核验日期与来源。

<a id="notes"></a>
## 使用说明

- **离线也能查目录。** 无法联网时，返回候选入口和搜索词，并明确标注当前未联网核验；不会把候选当成已满足全部条件的资源。
- **按任务获取素材。** 安装此 Skill 获得的是检索与选型指引，不会自动下载目录中的所有素材或安装所有组件库。
- **具体内容分别看许可。** 免费浏览、免费下载、可商用、无需署名和可再分发是不同条件，以官方页面及具体资源文件的许可为准。
- **访问失败如实说明。** 遇到登录墙、403 或抓取失败，会说明当前读取受限，并寻找可访问的替代来源。

README 的信息编排参考了 [Claude Code Skills 中文精选集](https://github.com/laolaoshiren/claude-code-skills-zh) 的快速上手与场景导航方式；技能内容和资源索引以本仓库文件为准。
