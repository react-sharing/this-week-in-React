原文地址：https://www.getrevue.co/profile/thisweekinreact/issues/this-week-in-react-90-jsx-tinybase-dioxus-owl-useworkerizedreducer-perf-typescript-css-982513

## React

### [JSX条件写法的好建议](https://thoughtspile.github.io/2022/01/17/jsx-conditionals/?utm_campaign=thisweekinreact&utm_medium=email&utm_source=Revue%20newsletter) 

我们喜欢 React，因为它还是 JavaScript，我们不需要学习另一种模板语言。但是让我们管理它并不总是那么容易，并且有一些陷阱需要避免😅这篇文章给出了一个很好的描述。

> 笔者备注：通过简单的图文，让人们很容易理解正确的写法和需要注意的坑。

### [使用WorkerizedReducer](https://github.com/surma/use-workerized-reducer?utm_campaign=thisweekinreact&utm_medium=email&utm_source=Revue%20newsletter)

Surma (Google) 介绍了一个库使用 Service Worker 来创建 React reducer（可能是异步的）的库。由于使用 Immer JS 和使用 post Message 传输补丁，通信效率很高。 浏览器兼容性很好，只有 Firefox 需要 polyfill。现在让我们为这个🤷‍♂️找到一个好的用例，有人自荐么？

### [不一致的事实：Next.js 和类型安全](https://t3.gg/blog/posts/types-and-nextjs?utm_campaign=thisweekinreact&utm_medium=email&utm_source=Revue%20newsletter)

关于Next.js中当前end-2-end类型限制的有趣想法，重点放在`getServerSideProps`和page props。要么有太多的手动样板文件（出错的风险），要么是类型帮助器`InferGetServerSidePropsType`可能会产生出人意料的不安全结果。唤起所有框架期待已久的 TypeScript 功能：[类型模块导出的能力](https://github.com/microsoft/TypeScript/issues/38511?utm_campaign=thisweekinreact&utm_medium=email&utm_source=Revue%20newsletter)。绍其他解决方案，如 Blitz、服务器组件或[tRPC](https://trpc.io/?utm_campaign=thisweekinreact&utm_medium=email&utm_source=Revue%20newsletter)。最后一个看起来非常有趣（另请参阅使用它的[zart](https://github.com/KATT/zart?utm_campaign=thisweekinreact&utm_medium=email&utm_source=Revue%20newsletter)样板）。

### [TinyBase](https://github.com/tinyplex/tinybase?utm_campaign=thisweekinreact&utm_medium=email&utm_source=Revue%20newsletter)
新的结构化数据的反应式存储(在表中，如SQL或Normalizr)，带有 React 集成包，包括用于高效、细粒度订阅的诸如`useCell`之类的hooks。体积小，但很有特色：索引、关系、撤消/重做……

-   [我们如何以零错误将 541 个组件从 Styled Components 迁移到 Emotion](https://storybook.js.org/blog/541-components-from-styled-components-to-emotion/?utm_campaign=thisweekinreact&utm_medium=email&utm_source=Revue%20newsletter)：将 Storybook 代码库从一个 CSS-in-JS 库迁移到另一个库的反馈，将他们自己的视觉回归工具（Chromatic）作为安全网进行测试
-   [阅读源代码 - Redux](https://alexkondov.com/reading-source-code-redux/?utm_campaign=thisweekinreact&utm_medium=email&utm_source=Revue%20newsletter)：Alex 研究了 Redux 代码库并利用这个机会讨论了在`createStore`中 TypeScript 重载的合法用法
-   [Three.js Web 动画的性能优化](https://www.gatsbyjs.com/blog/performance-optimization-for-three-js-web-animations/?utm_campaign=thisweekinreact&utm_medium=email&utm_source=Revue%20newsletter)：有效集成和延迟加载复杂React 组件的有用技术。在这种情况下，Three.js作为一个可选的前提。
-   [如何编写高性能的 React 代码：规则、模式、注意事项和注意事项](https://www.developerway.com/posts/how-to-write-performant-react-code?utm_campaign=thisweekinreact&utm_medium=email&utm_source=Revue%20newsletter)：好的建议和 4 条值得借鉴的规则
-   [Gatsby 4.5](https://www.gatsbyjs.com/docs/reference/release-notes/v4.5/?utm_campaign=thisweekinreact&utm_medium=email&utm_source=Revue%20newsletter)：也在尝试支持`getServerData` type😏
-   🎥如何与 Lee Robinson 一起[为开源 (Next.js) 做贡献](https://www.youtube.com/watch?utm_campaign=thisweekinreact&utm_medium=email&utm_source=Revue%20newsletter&v=cuoNzXFLitc)
-   [Remix-GraphQL](https://github.com/thomasheyenbrock/remix-graphql?utm_campaign=thisweekinreact&utm_medium=email&utm_source=Revue%20newsletter)
-   [Next.js RFC：更改默认 JS/CSS 输出以针对现代浏览器](https://github.com/vercel/next.js/discussions/33227?utm_campaign=thisweekinreact&utm_medium=email&utm_source=Revue%20newsletter)

## 💸赞助商

### [**Stream：用于 React 和 React-Native 的强大聊天和提要**](https://getstream.io/?utm_campaign=thisweekinreact&utm_content=Developer&utm_medium=email&utm_source=Revue%20newsletter) 

Stream 是企业级**API**和**SDK**的制造商，可帮助产品和工程团队大规模解决两个常见问题：**应用内聊天**和**社交活动反馈**。

借助 Stream，开发人员可以将任何类型的消息传递或各种反馈集成到他们的应用程序中，所需时间只是从头开始构建这些功能所需时间的一小部分。Stream Chat 使开发人员可以轻松地将丰富的实时消息传递到他们的应用程序中。

[Stream 为React](https://getstream.io/chat/sdk/react/?utm_campaign=thisweekinreact&utm_content=Developer&utm_medium=email&utm_source=Revue%20newsletter)、[React-Native](https://getstream.io/chat/sdk/react-native/?utm_campaign=thisweekinreact&utm_content=Developer&utm_medium=email&utm_source=Revue%20newsletter)、Flutter、Android、Angular、Compose、Unreal 和 iOS等流行框架提供强大的客户端 SDK 。它还支持[Expo 管理的工作流程](https://github.com/GetStream/stream-chat-react-native/tree/develop/examples/ExpoMessaging?utm_campaign=thisweekinreact&utm_medium=email&utm_source=Revue%20newsletter)。

[使用Maker Account](https://getstream.io/blog/maker-account/?utm_campaign=thisweekinreact&utm_content=Developer&utm_medium=email&utm_source=Revue%20newsletter)为您的启动或副项目**完全免费**解锁企业级特性、功能和 UI 组件。

## React Native
### [React-Native-Owl：React-Native 的视觉回归测试](https://formidable.com/blog/2022/react-native-owl/?utm_campaign=thisweekinreact&utm_medium=email&utm_source=Revue%20newsletter)

这个新的解决方案以原生方式运行您的 React-Native 屏幕，截取屏幕截图，并将它们与`./owl`中以前存储的屏幕截图进行比较，以生成报告。所有这些都与 Jest 很好地集成在一起（如快照）。

很高兴看到 React-Native 的可视化回归测试进展：这非常有用，与 web 相比，React-Native 已经落后了一点。另请参阅[Storybook React-Native-Web允许使用](https://www.dannyhwilliams.co.uk/introducing-react-native-web-storybook?utm_campaign=thisweekinreact&utm_medium=email&utm_source=Revue%20newsletter)[Chromatic](https://www.chromatic.com/?utm_campaign=thisweekinreact&utm_medium=email&utm_source=Revue%20newsletter)执行类似的操作，但但需要进行Web转换。

**附加功能：**

-   React-Native 0.67 应该在本周发布（[更新日志](https://github.com/facebook/react-native/blob/main/CHANGELOG.md?utm_campaign=thisweekinreact&utm_medium=email&utm_source=Revue%20newsletter#v0670)可用）
-   [为 React Native 构建风格/方案](https://medium.com/@ujjwalsayami/build-flavor-scheme-for-react-native-c58e764d4ecf?utm_campaign=thisweekinreact&utm_medium=email&utm_source=Revue%20newsletter)：允许在设备上多次安装同一个应用程序：对管理多个环境很有用。
-   [试图理解 Reanimated 2 的内部结构](https://aditya01.hashnode.dev/trying-to-understand-the-internals-of-reanimated-2?utm_campaign=thisweekinreact&utm_medium=email&utm_source=Revue%20newsletter)：很好的概述，很多图表
-   [expo-auto-navigation-webpack](https://github.com/EvanBacon/expo-auto-navigation-webpack?utm_campaign=thisweekinreact&utm_medium=email&utm_source=Revue%20newsletter)：Evan Bacon 正在进行的工作，以在 React-Native 中启用基于文件系统的导航（[之前的演示](https://twitter.com/Baconbrix/status/1384355891772739584?utm_campaign=thisweekinreact&utm_medium=email&utm_source=Revue%20newsletter)）。现在使用 Webpack 而不是 Metro。
-   [Expo Modules + JSI](https://twitter.com/tsapeta/status/1480932920462389255?utm_campaign=thisweekinreact&utm_medium=email&utm_source=Revue%20newsletter)：Expo 确认了简化我们生活的目标，即基于 JSI 在 Swift 或 Kotlin 中创建高性能的原生模块。这应该首先出现在 iOS 上。
-   [Demo React-Native-Gesture-Handler 按钮](https://twitter.com/swmansion/status/1480919926097518596?utm_campaign=thisweekinreact&utm_medium=email&utm_source=Revue%20newsletter)：展示了优于 React-Native Touchables 的优势
-   [在 React Native 中绘图（使用 Skia）](https://tonyowen.medium.com/drawing-with-skia-in-react-native-bffa816f4aa3?utm_campaign=thisweekinreact&utm_medium=email&utm_source=Revue%20newsletter)：创建进度指示器
-   [React-Native-Skia 绘图应用演示](https://twitter.com/chrfalch/status/1481969262575169538?utm_campaign=thisweekinreact&utm_medium=email&utm_source=Revue%20newsletter)：用手指在画布上绘图
-   [谁将支持您的下一个移动应用项目？提示：不是 React Native 或 Flutter](https://ionicframework.com/blog/who-is-going-to-support-your-next-mobile-app-project-hint-not-react-native-or-flutter/?utm_campaign=thisweekinreact&utm_medium=email&utm_source=Revue%20newsletter)：从哪里获得对 RN 应用程序的支持？🤷‍♂️
-   [React Native Facebook 登录：The Hard Way + The Expo Way](https://blog.expo.dev/react-native-facebook-login-the-hard-way-the-expo-way-d8eb978f82ee?utm_campaign=thisweekinreact&utm_medium=email&utm_source=Revue%20newsletter)


## 伙伴

-   [**开始 React Native**](https://start-react-native.dev/?utm_campaign=thisweekinreact&utm_medium=email&utm_source=Revue%20newsletter)：与 William Candillon 一起学习有关手势和动画的一切
-   [**React-Native Weekly**](https://andrei-calazans.com/?utm_campaign=thisweekinreact&utm_medium=email&utm_source=Revue%20newsletter)：保持最新的 React-Native 核心更新
-   [**TypeScript Weekly**](https://www.typescript-weekly.com/?utm_campaign=thisweekinreact&utm_medium=email&utm_source=Revue%20newsletter)：每周最好的 TypeScript 链接，应该在你的邮箱里面。
-   [**ES.next 新闻**](http://esnextnews.com/?utm_campaign=thisweekinreact&utm_medium=email&utm_source=Revue%20newsletter)：了解最新的 JavaScript 和跨平台工具
-   [**Tailwind Weekly**](https://tailwindweekly.com/?utm_campaign=thisweekinreact&utm_medium=email&utm_source=Revue%20newsletter) : 所有关于Tailwind CSS的东西，每周六新一期
-   [**G2i**](https://www.g2i.co/?utm_campaign=thisweekinreact&utm_medium=email&utm_source=Revue%20newsletter)：经过预先审查的远程 React 和 React-Native 开发人员，您可以按合同或完全信任本地开发人员
-   [**Infinite Red**](https://infinite.red/?utm_campaign=thisweekinreact&utm_medium=email&utm_source=Revue%20newsletter)：美国 React-Native 专家让您的想法成为现实
-   [**软件大厦**](https://swmansion.com/?utm_campaign=thisweekinreact&utm_medium=email&utm_source=Revue%20newsletter)：React Native 的共同创造者，众多科技公司的技术核心

## 其它
### [Parcel CSS](https://parceljs.org/blog/parcel-css/?utm_campaign=thisweekinreact&utm_medium=email&utm_source=Revue%20newsletter)

用Rust编写的一种新的解析器、编译器、压缩器，复用Firefox[的 rust-cssparser](https://github.com/servo/rust-cssparser?utm_campaign=thisweekinreact&utm_medium=email&utm_source=Revue%20newsletter)。在速度和输出规模方面优于竞争对手(甚至是esbuild)。集成在 Parcel 中，但也可以在 Rust 或 JavaScript（Webpack？）甚至[Deno 或 Web（WASM）中独立使用](https://twitter.com/devongovett/status/1482040430615318528?utm_campaign=thisweekinreact&utm_medium=email&utm_source=Revue%20newsletter)

### [Dioxus](https://dioxuslabs.com/blog/introducing-dioxus/?utm_campaign=thisweekinreact&utm_medium=email&utm_source=Revue%20newsletter)

新的 Rust 框架灵感主要来自于 React（钩子、VDOM、RSX ……），强类型、高性能、跨平台（Web、移动、桌面、SSR）。旨在易于被 React/TypeScript 开发人员采用。

我看了一点跨平台支持，但我不确定它是如何工作的。它说原生性能，但似乎在桌面和移动设备上使用[Tauri](https://tauri.studio/?utm_campaign=thisweekinreact&utm_medium=email&utm_source=Revue%20newsletter)，afaik 使用 WebViews？🤔

**附加功能：**

-   [TypeScript 备忘单](https://www.typescriptlang.org/cheatsheets?utm_campaign=thisweekinreact&utm_medium=email&utm_source=Revue%20newsletter)：4 个官方备忘单：类型、接口、类和控制流分析
-   🎥 [CSS Cascade 层](https://twitter.com/Una/status/1482096170843480068?utm_campaign=thisweekinreact&utm_medium=email&utm_source=Revue%20newsletter)：更好地控制 CSS 规则的特异性。这可能会产生有趣的影响：[不必再关心 CSS 插入顺序](https://twitter.com/sebastienlorber/status/1483155894288494593?utm_campaign=thisweekinreact&utm_medium=email&utm_source=Revue%20newsletter)。另请参阅[级联层解释器](https://css.oddbird.net/layers/explainer/?utm_campaign=thisweekinreact&utm_medium=email&utm_source=Revue%20newsletter)。
-   🧵[如何优化我的前端以获得最快的页面加载时间？](https://twitter.com/leeerob/status/1481693352059973632?utm_campaign=thisweekinreact&utm_medium=email&utm_source=Revue%20newsletter)
-   [宣布 Astro 技术公司](https://astro.build/blog/the-astro-technology-company/?utm_campaign=thisweekinreact&utm_medium=email&utm_source=Revue%20newsletter)：筹集 700 万美元
-   [将 Vite 添加到您现有的 Web 应用程序](https://css-tricks.com/adding-vite-to-your-existing-web-app/?utm_campaign=thisweekinreact&utm_medium=email&utm_source=Revue%20newsletter)：对从 Webpack 迁移很有用
-   [制作美丽的渐变](https://www.joshwcomeau.com/css/make-beautiful-gradients/?utm_campaign=thisweekinreact&utm_medium=email&utm_source=Revue%20newsletter)：Josh Comeau 解释了如何设计渐变并介绍[渐变生成器](https://www.joshwcomeau.com/gradient-generator/?utm_campaign=thisweekinreact&utm_medium=email&utm_source=Revue%20newsletter)
-   [JavaScript 调查状态](https://stateofjs.com/?utm_campaign=thisweekinreact&utm_medium=email&utm_source=Revue%20newsletter)：调查已开放
-   [DevTools 中的新功能 (Chrome 98)](https://developer.chrome.com/blog/new-in-devtools-98/?utm_campaign=thisweekinreact&utm_medium=email&utm_source=Revue%20newsletter)
-   [通过包发布和使用 ECMAScript 模块](https://2ality.com/2022/01/esm-specifiers.html?utm_campaign=thisweekinreact&utm_medium=email&utm_source=Revue%20newsletter)
-   [加速 Svelte 的发展](https://svelte.dev/blog/accelerating-sveltes-development?utm_campaign=thisweekinreact&utm_medium=email&utm_source=Revue%20newsletter)
-   [Safari 15 IndexedDB 泄漏](https://safarileaks.com/?utm_campaign=thisweekinreact&utm_medium=email&utm_source=Revue%20newsletter)+[利用 Safari 15 中的 IndexedDB API 信息泄漏](https://fingerprintjs.com/blog/indexeddb-api-browser-vulnerability-safari-15/?utm_campaign=thisweekinreact&utm_medium=email&utm_source=Revue%20newsletter)
-   [停止对 AngularJS 的长期支持](https://blog.angular.io/discontinued-long-term-support-for-angularjs-cc066b82e65a?utm_campaign=thisweekinreact&utm_medium=email&utm_source=Revue%20newsletter)
-   [我们如何将 nodejs monorepo 构建时间减少 70%](https://dev.to/scopsy/how-we-reduced-our-nodejs-monorepo-build-time-by-70-3oma?utm_campaign=thisweekinreact&utm_medium=email&utm_source=Revue%20newsletter)
-   [2022 年的伐木成本](https://www.nearform.com/blog/the-cost-of-logging-in-2022/?utm_campaign=thisweekinreact&utm_medium=email&utm_source=Revue%20newsletter)
-   [WebAssembly 的状态——2021 年和 2022 年](https://platform.uno/blog/the-state-of-webassembly-2021-and-2022/?utm_campaign=thisweekinreact&utm_medium=email&utm_source=Revue%20newsletter)
-   [我们如何使用 Rust、WebAssembly 和 TypeScript 构建 VS Code 扩展](https://www.osohq.com/post/building-vs-code-extension-with-rust-wasm-typescript?utm_campaign=thisweekinreact&utm_medium=email&utm_source=Revue%20newsletter)
