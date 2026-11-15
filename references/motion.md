# 动效、特效与源码

来源：用户提供的 resources.md。目录区分“参考实现”和“驱动动画的工具”；除下方核验记录外，具体版本、许可、下载与访问情况在使用时确认。

## 找现成效果与源码

| 资源 | 适合寻找 | 如何取得可用内容 |
|---|---|---|
| [Codrops](https://tympanus.net/codrops/) | 图片转场、排版动效、创意交互、WebGL 示例 | 进入具体文章，找 Demo / Source / GitHub，确认项目 LICENSE 与图片、字体依赖；本次抓取返回 403 |
| [CodePen](https://codepen.io/) | HTML / CSS / JS 交互实验 | 找具体 Pen，查看依赖及源码；区分代码和素材许可 |
| [CodyHouse](https://codyhouse.co/) | UI 组件与交互模式 | 查看具体组件是否开放源码、下载是否付费 |
| [CSS-Tricks](https://css-tricks.com/) | CSS 交互技巧与实现片段 | 按目标效果查文章和 demo，仅取任务相关实现，不用作课程路线 |
| [Motion.Lab](https://motionlab.uanx.online/) | 原清单中的动效参考入口 | 2026-11-14 当前工具无法访问；具体效果、源码和许可未核实 |
| [HyperFrames](https://hyperframes.io/) | 原清单的项目相关候选入口 | 2026-11-14 当前工具无法访问；用途、内容和许可未确认，不作为已验证动效库推荐 |

搜索词：`image transition`、`text reveal`、`scroll animation`、`magnetic button`。要求可复制代码时，优先交付具体示例链接、源文件入口和接入条件；只有站点首页时标为“源码查找入口”。

## 选择动画实现工具

| 资源 | 何时选 | 接入与限制 |
|---|---|---|
| [Web Animations API / MDN](https://developer.mozilla.org/en-US/docs/Web/API/Web_Animations_API) | 原生网页、需编程控制的简单动画 | 先考虑 CSS；滚动驱动能力按目标浏览器检查支持 |
| [Motion](https://motion.dev/) | 组件进出场、弹簧和布局动画 | 查看目标框架或原生 JS 的对应文档，不沿用旧包名猜 API |
| [GSAP](https://gsap.com/) | 多段时间轴、复杂滚动与动画编排 | 使用自有标准许可，不能标为 MIT；见下方 |
| [Anime.js](https://animejs.com/) | JS / SVG / DOM 动画编排 | 核对当前主版本 API 与所需模块 |
| [Three.js](https://threejs.org/) | 真实三维对象、相机与材质 | 需要渲染循环、清理及移动端性能预算 |
| [React Three Fiber](https://r3f.docs.pmnd.rs/) | 在 React 中组织 Three.js 场景 | 与 Three.js 配合；不用于无 React 依赖的项目 |
| [LottieFiles](https://lottiefiles.com/) | 导出动画素材与播放器生态 | 平台、具体动画文件、播放器分别看许可；不把整个图库视为免费 |
| [Rive](https://rive.app/) | 状态机、响应输入的交互动效 | 核对编辑器、运行时、素材与导出条件 |
| [Spline](https://spline.design/) | 可视化工具制作与嵌入 3D | 核对导出、嵌入、计划限制及加载成本 |
| [Theatre.js](https://www.theatrejs.com/) | 可视化时间轴与场景编排 | 查看当前维护、集成与许可情况 |
| [Lenis](https://lenis.dev/) | 平滑滚动与滚动同步 | 不是完整动画引擎；评估滚动体验后再引入 |

按需求选最小实现：简单反馈优先 CSS / WAAPI；组件状态可考虑 Motion；复杂时间轴考虑 GSAP；真实 3D、交互状态机、设计师导出动画分别考虑 Three.js、Rive、Lottie。它们解决不同问题，不是必须逐级升级的路线。

动画通常优先使用 transform / opacity；filter、布局变化和大面积重绘需实际评估，不能统称为低成本。适配 `prefers-reduced-motion`，为重型效果提供静态或轻量呈现。

## 已核验修正（2026-11-14）

- [GSAP 标准许可](https://gsap.com/community/standard-license/)允许商业网站等许可用途免费使用，包含对特定可视化动画构建工具用途的限制；并非原清单写的 MIT。
- [Lenis 官网](https://lenis.dev/)由原 `lenis.darkroom.engineering` 入口跳转而来，目录使用新地址。
- CodePen 首页可读取；Codrops 返回 403；Motion.Lab / HyperFrames 当前工具无法读取。后三项仅保留候选，不承诺可获取源码。
