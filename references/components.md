# 设计系统与组件

来源：用户提供的 resources.md。表中为检索入口和用途判断，未标注核验日期的版本、框架支持、价格及许可需在入选时查看官网。设计系统、Figma kit、代码组件库与 CSS 框架分别选择，不要求同时引入。

## 设计规范与 Figma

| 资源 | 适用任务 | 注意事项 |
|---|---|---|
| [Untitled UI](https://www.untitledui.com/) | SaaS 设计基础、Figma kit、成套界面 | 按具体产品判断免费范围、付费内容和团队许可 |
| [shadcn/ui 的 Figma 入口](https://ui.shadcn.com/docs/figma) | 找与 shadcn 对应的 Figma kit | 社区维护，含免费与付费条目；核对所选文件与代码版本 |
| [Ant Design](https://ant.design/) | 企业应用规范、复杂表单与表格 | 官方 React 组件与其他框架实现分别核验 |
| [Material 3](https://m3.material.io/) | Material 风格、设计 token、交互规范 | 规范可参考；代码实现需匹配目标平台 |
| [Adobe Spectrum](https://spectrum.adobe.com/) | 专业工具、复杂产品 UI 的规范 | 设计规范与具体实现库分开看 |
| [Carbon](https://carbondesignsystem.com/) | 企业应用、数据密集界面 | 找组件规范、状态及可访问性说明 |
| [GitHub Primer](https://primer.style/) | 开发者工具、信息密集产品 | 区分设计规范与不同实现包 |
| [GOV.UK Design System](https://design-system.service.gov.uk/) | 公共服务、清晰表单与内容流程 | 借鉴可用性模式，适配本地语言和品牌 |
| [Figma Community](https://www.figma.com/community) | UI kit、模板与设计素材 | 搜索具体框架 + UI kit；按发布者、维护情况及许可筛选 |

## 可接入的代码

| 资源 | 类别 / 框架入口 | 适合什么 | 接入时确认 |
|---|---|---|---|
| [shadcn/ui](https://ui.shadcn.com/) | 将组件源码引入项目的体系，以 React 生态为入口 | 高定制产品 UI、可编辑组件 | 查看当前样式及底层实现，不假定全部固定为某一原语库 |
| [Radix UI](https://www.radix-ui.com/) | React 无样式交互原语 | 自建风格的 Dialog、Menu、Popover 等 | 仍需样式和应用测试 |
| [Headless UI](https://headlessui.com/) | React / Vue 无样式组件 | 自定义弹窗、列表选择、菜单 | 进入对应框架文档；不是现成后台模板 |
| [MUI](https://mui.com/) | React 组件体系 | Material 产品、数据 UI | 核查所需组件是否属于不同授权层级 |
| [Chakra UI](https://chakra-ui.com/) | React 组件体系 | 需要主题化的应用 | 按项目版本确认 API 与主题方式 |
| [Ant Design](https://ant.design/) | React 企业级组件 | 表格、表单、后台管理 | Vue 项目需要另外核实对应实现，不能直接 import React 包 |
| [Tailwind Plus（原 Tailwind UI）](https://tailwindcss.com/plus) | 官方组件 / 模板产品入口 | 已有使用权时查找成品区块 | 2026-11-14 入口跳转登录页；未证实新用户可购买或获取，不作为无账号用户默认选项 |

项目使用 Vue、Svelte 或原生 HTML 时，优先查目录中明确兼容的实现；不足以覆盖需求时可补充该生态官方资源，标明目录外补充。不能为了套用某个 React 库改换项目框架。

## CSS 框架

| 资源 | 用途 | 选择条件 |
|---|---|---|
| [Tailwind CSS](https://tailwindcss.com/) | 工具类与设计 token 的实现 | 项目已采用或明确选择时用，按现有主版本接入 |
| [Bootstrap](https://getbootstrap.com/) | 通用布局与组件 | 已有 Bootstrap 项目或快速原型；检查 JS 行为与项目集成方式 |

## 已核验修正（2026-11-14）

- [shadcn Figma 文档](https://ui.shadcn.com/docs/figma)区分社区提供的免费和付费文件，不能把所有 kit 描述为“官方、免费、与代码严格一一对应”。
- [Headless UI 官网](https://headlessui.com/)提供 React 与 Vue 入口，适合需要自定义样式的交互组件。
- [Tailwind Plus 入口](https://tailwindcss.com/plus)本次仅能读到登录页；这只说明当前访问结果，不据此断言产品停运。
