原文地址：https://www.getrevue.co/profile/thisweekinreact/issues/this-week-in-react-90-jsx-tinybase-dioxus-owl-useworkerizedreducer-perf-typescript-css-982513

一周的各种内容，从有趣的 React 文章到导致一些健康的 FOMO 的新工具 😇
Parcel CSS 重用了最初为 Firefox 创建的 Rust css 解析器，这真的很酷！
我也很高兴地注意到 Node.js 显然支持 Error Cause！
🙏 支持时事通讯 🙏 ： 
😘 推荐给你的朋友：真的很有帮助！
💸 本周在 React中赞助
😍 在 Twitter 上写推荐信
🧵 转发最新的 Twitter 帖子
📨 回复此邮件： 随时欢迎反馈
反应
关于 JSX 条件的好建议
我们喜欢 React，因为它只是 JavaScript，我们不需要学习另一种模板语言。但是让我们管理它并不总是那么容易，并且有一些陷阱需要避免😅这篇文章给出了一个很好的概述。
使用WorkerizedReducer
Surma (Google) 引入了一个库来使用 Service Worker 来创建 React reducer（可能是异步的）。由于 ImmerJS 和使用postMessage. 浏览器支持很好，只有 Firefox 需要 polyfill。现在让我们为这个🤷‍♂️找到一个好的用例，有人吗？
一个不一致的事实：Next.js 和类型安全
关于 Next.js 中 end-2-end 类型的当前限制的有趣想法，重点是getServerSideProps页面道具。要么有太多的手动样板文件（出错的风险），要么有一个类型助手InferGetServerSidePropsType可能会给出令人惊讶的不安全结果。唤起所有框架期待已久的 TypeScript 功能：类型模块导出的能力。展示其他解决方案，如 Blitz、服务器组件或tRPC。最后一个看起来很有趣（另见使用它的zart样板）。
小基地
用于结构化数据的新反应式存储（在表中，如 SQL 或 Normalizr），带有 React 集成包，包括useCell用于高效、细粒度订阅的钩子。体积小，但很有特色：索引、关系、撤消/重做……
附加功能：
我们如何以零错误将 541 个组件从 Styled Components 迁移到 Emotion：将 Storybook 代码库从一个 CSS-in-JS 库迁移到另一个库的反馈，将他们自己的视觉回归工具（Chromatic）作为安全网进行测试
阅读源代码 - Redux：Alex 研究了 Redux 代码库并利用这个机会讨论了 TypeScript 重载的合法用法createStore
Three.js Web Animations 的性能优化：有效集成和延迟加载繁重的 React 组件的有用技术。在这种情况下，一个可选的 Three.js 背景。
如何编写高性能的 React 代码：规则、模式、注意事项和注意事项：好的建议和 4 条值得借鉴的规则
Gatsby 4.5：也在尝试打字getServerData😏
🎥如何与 Lee Robinson 一起为开源 (Next.js) 做贡献
Remix-GraphQL
Next.js RFC：更改默认 JS/CSS 输出以针对现代浏览器
💸赞助商
Stream：用于 React 和 React-Native 的强大聊天和提要
Stream 是企业级API和SDK的制造商，可帮助产品和工程团队大规模解决两个常见问题：应用内聊天和社交活动源。
借助 Stream，开发人员可以将任何类型的消息传递或提要体验集成到他们的应用程序中，所需时间只是从头开始构建这些功能所需时间的一小部分。Stream Chat 使开发人员可以轻松地将丰富的实时消息传递到他们的应用程序中。
Stream 为React、React-Native、Flutter、Android、Angular、Compose、Unreal 和 iOS等流行框架提供强大的客户端 SDK 。它还支持Expo 管理的工作流程。
使用Maker Account为您的启动或副项目完全免费解锁企业级特性、功能和 UI 组件。
反应原生
React-Native-Owl：React-Native 的视觉回归测试
这个新的解决方案以原生方式运行您的 React-Native 屏幕，截取屏幕截图，并将它们与之前存储的屏幕截图进行比较./owl以生成报告。所有这些都与 Jest 很好地集成在一起（如快照）。
很高兴看到 React-Native 的视觉回归测试进展：这非常有用，与 web 相比，React-Native 已经落后了一点。另请参阅Storybook React-Native-Web允许使用Chromatic做类似的事情，但需要进行网络转换。
附加功能：
React-Native 0.67 应该在本周发布（更新日志可用）
为 React Native 构建风格/方案：允许在设备上多次安装同一个应用程序：对管理多个环境很有用。
试图理解 Reanimated 2 的内部结构：很好的概述，很多图表
expo-auto-navigation-webpack：Evan Bacon 正在进行的工作，以在 React-Native 中启用基于文件系统的导航（之前的演示）。现在使用 Webpack 而不是 Metro。
Expo Modules + JSI：Expo 确认了简化我们生活的目标，即基于 JSI 在 Swift 或 Kotlin 中创建高性能的原生模块。这应该首先出现在 iOS 上。
Demo React-Native-Gesture-Handler 按钮：展示了优于 React-Native Touchables 的优势
在 React Native 中绘图（使用 Skia）：创建进度指示器
React-Native-Skia 绘图应用演示：用手指在画布上绘图
谁将支持您的下一个移动应用项目？提示：不是 React Native 或 Flutter：从哪里获得对 RN 应用程序的支持？🤷‍♂️
React Native Facebook 登录：The Hard Way + The Expo Way
伙伴
开始 React Native：与 William Candillon 一起学习有关手势和动画的一切
React-Native Weekly：保持最新的 React-Native 核心更新
TypeScript Weekly：每周最好的 TypeScript 链接，就在您的收件箱中。
ES.next 新闻：了解最新的 JavaScript 和跨平台工具
Tailwind Weekly : 所有东西 Tailwind CSS，每周六新一期
G2i：经过预先审查的远程 React 和 React-Native 开发人员，您可以在合同或全职基础上信任
Infinite Red：美国 React-Native 专家让您的想法成为现实
软件大厦：React Native 的共同创造者，众多科技公司的技术核心
其他
包裹 CSS
一个新的解析器，编译器，用 Rust 编写的压缩器 un CSS，重用Firefox的 rust-cssparser。在速度和输出大小（甚至 esbuild）方面优于竞争对手。集成在 Parcel 中，但也可以在 Rust 或 JavaScript（Webpack？）甚至Deno 或 Web（WASM）中独立使用
狄奥克斯
新的 Rust 框架很大程度上受 React（钩子、VDOM、RSX ……）的启发，强类型、高性能、跨平台（Web、移动、桌面、SSR）。旨在易于被 React/TypeScript 开发人员采用。
我看了一点跨平台支持，但我不确定它是如何工作的。它说本机性能，但似乎在桌面和移动设备上使用Tauri，afaik 使用 WebViews？🤔
附加功能：
TypeScript 备忘单：4 个官方备忘单：类型、接口、类和控制流分析
🎥 CSS Cascade 层：更好地控制 CSS 规则的特异性。这可能会产生有趣的影响：不必再关心 CSS 插入顺序。另请参阅级联层解释器。
🧵如何优化我的前端以获得最快的页面加载时间？
宣布 Astro 技术公司：筹集 700 万美元
将 Vite 添加到您现有的 Web 应用程序：对从 Webpack 迁移很有用
制作美丽的渐变：Josh Comeau 解释了如何设计渐变并介绍渐变生成器
JavaScript 调查状态：调查已开放
DevTools 中的新功能 (Chrome 98)
通过包发布和使用 ECMAScript 模块
加速 Svelte 的发展
Safari 15 IndexedDB 泄漏+利用 Safari 15 中的 IndexedDB API 信息泄漏
停止对 AngularJS 的长期支持
我们如何将 nodejs monorepo 构建时间减少 70%
2022 年的伐木成本
WebAssembly 的状态——2021 年和 2022 年
我们如何使用 Rust、WebAssembly 和 TypeScript 构建 VS Code 扩展
