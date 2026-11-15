# Frontend UI Resources

面向 AI 编程助手的前端 UI 资源导航 Skill，精选 73 个不重复的设计与开发资源入口，按页面需求、技术栈和预算快速筛选。

## 资源范围

| 分类 | 内容 | 索引 |
|---|---|---|
| 页面与区块灵感 | 落地页、作品集、后台、产品流程、Hero、导航和页脚 | [inspiration.md](references/inspiration.md) |
| 设计系统与组件 | Figma kit、设计规范、组件库、交互原语和 CSS 框架 | [components.md](references/components.md) |
| 动效与特效 | 源码示例、时间轴、滚动叙事、交互动效和 3D 工具 | [motion.md](references/motion.md) |
| 配色与视觉素材 | 配色、图标、字体、插画、图片和背景视频 | [assets.md](references/assets.md) |

仅保留服务于 UI 设计与实现的内容，不包含学习路线、课程和后端工具链。

## 安装

将此仓库下载到支持 Skill 的 AI 助手的技能目录，保留整个文件夹结构。例如，安装到个人 Codex 技能目录：

```bash
git clone --branch master https://github.com/Wangcongming666/frontend-ui-resources.git ~/.codex/skills/frontend-ui-resources
```

如果目标目录已有同名技能，先检查已有内容，避免覆盖本地修改。也可以下载仓库 ZIP，解压为 `frontend-ui-resources` 文件夹后放入技能目录。

## 使用示例

```text
使用 $frontend-ui-resources，为我的 SaaS 落地页找极简风格参考、组件和免费素材。
```

```text
使用 $frontend-ui-resources，为 Vue 后台找兼容的表单组件和无需署名的空状态插画。
```

```text
使用 $frontend-ui-resources，找 3 个有源码的图片转场示例，并说明依赖和接入方式。
```

技能会按需读取分类索引，优先复用项目已有技术栈，输出资源链接、适用位置、获取与接入方式，以及费用、署名和许可条件。

## 文件结构

```text
frontend-ui-resources/
├── SKILL.md
├── agents/
│   └── openai.yaml
└── references/
    ├── inspiration.md
    ├── components.md
    ├── motion.md
    └── assets.md
```

[SKILL.md](SKILL.md) 为技能入口，四份参考文件按需加载。

## 核验与来源

资源基于用户提供的前端设计资源清单整理。部分许可、名称与访问状态于 2026-11-14 核验并修正，具体记录见分类索引；其余条目是候选入口，使用时需确认当前状态。

技能区分视觉参考、Figma 文件、可复制源码、运行时库和素材文件。离线或页面受限时会说明核验范围，不把首页入口当成已经取得的代码或素材。各资源的内容及授权以其官方页面、具体文件和许可为准。
