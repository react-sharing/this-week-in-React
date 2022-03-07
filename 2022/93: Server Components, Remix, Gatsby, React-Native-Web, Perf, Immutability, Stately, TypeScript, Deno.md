# React 

[**Shopify: React Server Components best practices**](https://shopify.engineering/react-server-components-best-practices-hydrogen?utm_campaign=thisweekinreact&utm_medium=email&utm_source=Revue%20newsletter)

Cathryn对Shopify公司使用Servers Components的反馈，她通过新的[Hydrogen](https://hydrogen.shopify.dev/?utm_campaign=thisweekinreact&utm_medium=email&utm_source=Revue%20newsletter)框架学会了使用Servers Components。如果没有最佳实践指导，你可能无法正确地使用这个新的React功能，导致最终会产生一个比它大的包。她建议默认使用Shared Components，而不是Client Components（我们现在使用的）。对于交互性，提取一些最细粒度的Client Components，然后把剩余的尽可能转化为Server Components。我们[有时用来优化](https://twitter.com/sebmarkbage/status/1096115287781400576?utm_campaign=thisweekinreact&utm_medium=email&utm_source=Revue%20newsletter)的composition patterns（使用`children`用）也可以用来搭配使用不同类型的组件。她提供了一个真实的案例，用了2个例子来说明：通讯注册和产品FAQ。一个Shopify使用服务器组件的教程也已经出版了：[Rapid Development with Hydrogen: Building a Product Page](https://shopify.engineering/rapid-development-hydrogen-building-product-page?utm_campaign=thisweekinreact&utm_medium=email&utm_source=Revue%20newsletter)

[**How to write performant React apps with Context**](https://www.developerway.com/posts/how-to-write-performant-react-apps-with-context?utm_campaign=thisweekinreact&utm_medium=email&utm_source=Revue%20newsletter)

Nadia解释了如何使用React上下文来优化复杂的React表单的渲染。首先，你必须分离成2个上下文和hooks`useFormData()`和`useFormAPI()`。不要忘记正确memo`api`对象。我们最终可以把状态分成几个小的上下文。这些技术可能无法像真正的状态管理器那样扩展，但在你无法使用状态管理器的情况下，了解这些技术还是很有用的。

[**The “best” way to manage icons in React.js**](https://benadam.me/thoughts/react-svg-sprites/?utm_campaign=thisweekinreact&utm_medium=email&utm_source=Revue%20newsletter)

在React中使用图标有很多方法，每种方法都有不同的权衡。`.svg`文件不能在CSS中写样式。渲染SVG的React组件（也适用于SVGR）很方便，但它们在HTML输出中内联SVG标签会使页面更重。根据我的经验，在多次使用相同图标的静态页面（或SSR）上，我们很快就会看到这个问题。Ben提供了一个伟大的、鲜为人知的替代方案：使用SVG sprites。

## **拓展阅读:**
-   📜 [How to Setup React Native Web in a Remix project](https://horus.dev/blog/react-native-web-remix-setup?utm_campaign=thisweekinreact&utm_medium=email&utm_source=Revue%20newsletter): React-Native-Web可以与Remix很好地整合，就像使用任何的CSS-in-JS库一样。
-   📜 [Offline React Query](https://tkdodo.eu/blog/offline-react-query?utm_campaign=thisweekinreact&utm_medium=email&utm_source=Revue%20newsletter): Dominik介绍了React-Query 3在处理离线或网络问题上的局限性，并介绍了新的v4（[目前在Beta版本](https://github.com/tannerlinsley/react-query/releases?utm_campaign=thisweekinreact&utm_medium=email&utm_source=Revue%20newsletter)），可能会帮助你更好的处理离线优先场景的应用程序。
-   📜 [Rendering 3D in React made easy with react-three-fiber](https://tsh.io/blog/react-three-fiber/?utm_campaign=thisweekinreact&utm_medium=email&utm_source=Revue%20newsletter): 一个对Three.js 和 R3f不错的介绍。
-   📖 Partytown: [new doc site](https://partytown.builder.io/?utm_campaign=thisweekinreact&utm_medium=email&utm_source=Revue%20newsletter) + pages to integrate with [Next.js](https://partytown.builder.io/nextjs?utm_campaign=thisweekinreact&utm_medium=email&utm_source=Revue%20newsletter) and [Remix](https://partytown.builder.io/remix?utm_campaign=thisweekinreact&utm_medium=email&utm_source=Revue%20newsletter)
-   🐦 [ *“A simple composition trick to avoid re-rendering a component”* ](https://twitter.com/asidorenko_/status/1490017216942780418?utm_campaign=thisweekinreact&utm_medium=email&utm_source=Revue%20newsletter): 与服务器组件使用的技术相同😏（第一条）。
-   📦 [Gatsby 4.7](https://www.gatsbyjs.com/docs/reference/release-notes/v4.7/?utm_campaign=thisweekinreact&utm_medium=email&utm_source=Revue%20newsletter): with new option: `trailingSlash`
-   📦 [Yerba](https://github.com/TheoBr/yerba?utm_campaign=thisweekinreact&utm_medium=email&utm_source=Revue%20newsletter): Electron Turborepo monorepo with Next.js, Typescript, Vite…
-   📦 [Lamina](https://github.com/pmndrs/lamina?utm_campaign=thisweekinreact&utm_medium=email&utm_source=Revue%20newsletter): layer-based shader material for Three.js + React-Three-Fiber
-   🔗 [Remix Routing Demo](https://remix-routing-demo.netlify.app/?utm_campaign=thisweekinreact&utm_medium=email&utm_source=Revue%20newsletter)
-   🔗 [Remix Bug Report Test](https://twitter.com/remix_run/status/1488999703354085380?utm_campaign=thisweekinreact&utm_medium=email&utm_source=Revue%20newsletter): Remix建议通过创建失败的测试来报告框架的错误😏
-   🔗 [remix.guide](https://remix.guide/?utm_campaign=thisweekinreact&utm_medium=email&utm_source=Revue%20newsletter): 有点像HackerNews的Remix content 

# React-Native 
-   🧵 *Andrew Clark:* [*“I can’t prove this but I suspect if someone built a Next.js/Remix/etc for React Native (i.e. single codebase for client and server) they would make a trillion dollars”* ](https://twitter.com/acdlite/status/1489755769876754434?s=20&t=oOXVNH5yTvK-4xcWrJM7Ig&utm_campaign=thisweekinreact&utm_medium=email&utm_source=Revue%20newsletter): 我不知道Andrew到底在想什么，但这是一个非常有趣的讨论话题!我对服务器组件在React-Native中的使用特别感兴趣（或者至少是一些服务器驱动的UI），以及将数据需求与屏幕放在一起（想想Remix/`loader`，Next.js/`getServerProps`，但它们用于React-Navigation）。
-   🧵 Satyajit Sahoo: [ *“Seeing many people compare React Navigation to React Router…”*](https://twitter.com/satya164/status/1490279552882511878?utm_campaign=thisweekinreact&utm_medium=email&utm_source=Revue%20newsletter)
-   📜 [Displaying a List in React Native: Map Method or FlatList Component](https://blog.expo.dev/react-native-flatlist-made-easy-20fca51e0327?utm_campaign=thisweekinreact&utm_medium=email&utm_source=Revue%20newsletter)
-   📜 [Expo EAS + LogRocket: Unlimited Possibilities for Your Expo Apps](https://blog.expo.dev/eas-logrocket-unlimited-possibilities-for-your-expo-apps-d74cf1fbf1b5?utm_campaign=thisweekinreact&utm_medium=email&utm_source=Revue%20newsletter)
-   📖 [React-Navigation - Organizing Types](https://reactnavigation.org/docs/typescript/?utm_campaign=thisweekinreact&utm_medium=email&utm_source=Revue%20newsletter#organizing-types): new doc
-   📦 [React-Native 0.68.0-rc.1](https://github.com/facebook/react-native/releases/tag/v0.68.0-rc.1?utm_campaign=thisweekinreact&utm_medium=email&utm_source=Revue%20newsletter): 已经有了新的分支和RC，因为发布周期越来越快。
-   📦 [expo-e2e-demo](https://github.com/calitb/expo-e2e-demo?utm_campaign=thisweekinreact&utm_medium=email&utm_source=Revue%20newsletter): 通过GitHub actions在Expo应用上试用Detox e2e测试
-   📦 [React Location on React Native POC](https://github.com/tom-sherman/ReactLocationNative?utm_campaign=thisweekinreact&utm_medium=email&utm_source=Revue%20newsletter): 将React-Location库与React-Native集成，以实现 "边取边用 "模式。
-   🐦 [ *“We rebuilt the docs of NativeBase using Nativebase”*](https://twitter.com/sanketsahu/status/1489588106194202627?utm_campaign=thisweekinreact&utm_medium=email&utm_source=Revue%20newsletter)
-   [👥](https://emojikeyboard.org/copy/Busts_in_Silhouette_Emoji_%F0%9F%91%A5?utm_campaign=thisweekinreact&utm_medium=email&utm_source=Revue%20newsletter) [App.js Conf 2022](https://blog.swmansion.com/app-js-conf-2022-4ad792c0a566?utm_campaign=thisweekinreact&utm_medium=email&utm_source=Revue%20newsletter): 6月8-10日克拉科夫（[CFP](https://docs.google.com/forms/d/e/1FAIpQLScyrpH1Htd1A6oEKL6RDDMckjP7L_FmWljsAvVpu-pbLhQiJw/viewform?utm_campaign=thisweekinreact&utm_medium=email&utm_source=Revue%20newsletter)）。我还有2020年的票，所以希望你能在那里见到我。
-   [👥](https://emojikeyboard.org/copy/Busts_in_Silhouette_Emoji_%F0%9F%91%A5?utm_campaign=thisweekinreact&utm_medium=email&utm_source=Revue%20newsletter) [React Native London February 2022](https://www.meetup.com/React-Native-London/events/283794909/?utm_campaign=thisweekinreact&utm_medium=email&utm_source=Revue%20newsletter): 与Quin Jung（Expo）会面（直播），谈论全新的EAS更新。
-   🎥 [Limitless App Development with Expo and React Native](https://www.youtube.com/watch?utm_campaign=thisweekinreact&utm_medium=email&utm_source=Revue%20newsletter&v=b5ZHPJU_FLQ) 

# 其它
[**A list of every web API in Deno**](https://deno.com/blog/every-web-api-in-deno?utm_campaign=thisweekinreact&utm_medium=email&utm_source=Revue%20newsletter)

Luca（Deno贡献者）详尽地提到了Deno支持的所有网络API。毫不奇怪，它是一个部署Remix应用的好平台。这可能是[上周宣布的Node.js 18的新网络API](https://twitter.com/MylesBorins/status/1489024782205173760?utm_campaign=thisweekinreact&utm_medium=email&utm_source=Revue%20newsletter)的回应。另请阅读：[Node.js核心中的fetch()：为什么你应该关心](https://fusebit.io/blog/node-fetch/?utm_campaign=thisweekinreact&utm_medium=email&utm_source=Revue%20newsletter)

[**Immutability isn’t free**](https://swizec.com/blog/immutability-isnt-free/?utm_campaign=thisweekinreact&utm_medium=email&utm_source=Revue%20newsletter)

有趣的故事，在后端背景下，但基本上适用于React应用程序。FP和不可变性的使用导致了与数组复制和`O(n2)`算法有关的糟糕性能。注意：通过使用[ImmutableJS](https://immutable-js.com/?utm_campaign=thisweekinreact&utm_medium=email&utm_source=Revue%20newsletter)等lib内部使用的[向量尝试和结构共享](https://hypirion.com/musings/understanding-persistent-vector-pt-1?utm_campaign=thisweekinreact&utm_medium=email&utm_source=Revue%20newsletter)，也有可能获得更好的不变性性能。

[**Netlify Scheduled Functions**](https://www.netlify.com/blog/quirrel-joins-netlify-and-scheduled-functions-launches-in-beta?utm_campaign=thisweekinreact&utm_medium=email&utm_source=Revue%20newsletter)

[Quirrel](https://quirrel.dev/?utm_campaign=thisweekinreact&utm_medium=email&utm_source=Revue%20newsletter)（serverless cron jobs SaaS）及其创建者Simon（见他的[帖子](https://simonknott.de/articles/netlify-acquires-quirrel?utm_campaign=thisweekinreact&utm_medium=email&utm_source=Revue%20newsletter)）都加入了Netlify，Netlify在测试版中引入了新的Scheduled Functions功能。这种功能在目前的无服务器领域显然是缺乏的。请注意，Blitz（Simon是贡献者之一）[转向Blitz Toolkit](https://github.com/blitz-js/blitz/discussions/3075?utm_campaign=thisweekinreact&utm_medium=email&utm_source=Revue%20newsletter)，以提供类似的服务。我们对Vercel提出的建议不会感到惊讶😏

## **拓展阅读:**
-   [Why Efficient Hydration in JavaScript Frameworks is so Challenging](https://dev.to/this-is-learning/why-efficient-hydration-in-javascript-frameworks-is-so-challenging-1ca3?utm_campaign=thisweekinreact&utm_medium=email&utm_source=Revue%20newsletter): Ryan Carniato（Solid）介绍了各种前端应用程序化策略的权衡，包括Remix、服务器组件、Astro、Qwik...
-   [Stately Editor public beta](https://stately.ai/blog/stately-editor-public-beta?utm_campaign=thisweekinreact&utm_medium=email&utm_source=Revue%20newsletter): 低代码工具，基于状态机和状态图可视化地创建应用逻辑。作者是XState的创造者。
-   [Babel 7.17.0](https://babeljs.io/blog/2022/02/02/7.17.0?utm_campaign=thisweekinreact&utm_medium=email&utm_source=Revue%20newsletter): includes new decorators proposal (stage 2)
-   [@tsconfig/strictest](https://www.npmjs.com/package/@tsconfig/strictest?utm_campaign=thisweekinreact&utm_medium=email&utm_source=Revue%20newsletter): because [strict mode is not strict enough](https://twitter.com/orta/status/1489489857198051328?utm_campaign=thisweekinreact&utm_medium=email&utm_source=Revue%20newsletter)
-   [Wordle with TypeScript types](https://twitter.com/orta/status/1490631626828746753?utm_campaign=thisweekinreact&utm_medium=email&utm_source=Revue%20newsletter) 😝
-   [Monitor Exports from Packages in Monorepos](https://kamranicus.com/monitor-exports-from-node-js-packages-in-monorepos/?utm_campaign=thisweekinreact&utm_medium=email&utm_source=Revue%20newsletter): 使用Jest快照+`codeowners`来监控libs公共API表面的变化 🤔
-   [Structuring your Storybook](https://storybook.js.org/blog/structuring-your-storybook/?utm_campaign=thisweekinreact&utm_medium=email&utm_source=Revue%20newsletter)
-   GitHub: [New sponsors-only repositories, custom amounts, and more](https://github.blog/2022-02-02-new-sponsors-only-repositories-custom-amounts-and-more/?utm_campaign=thisweekinreact&utm_medium=email&utm_source=Revue%20newsletter)
-   New option `curl --json`
-   [*“Nobody at Facebook has worked on Jest for years”* ](https://news.ycombinator.com/item?id=30168241&utm_campaign=thisweekinreact&utm_medium=email&utm_source=Revue%20newsletter): some Hacker News drama
-   [Vercel - The evolution of the Web](https://vercel.com/blog/how-the-web-evolves?utm_campaign=thisweekinreact&utm_medium=email&utm_source=Revue%20newsletter): 2021 retrospective
-   [Flutter 2.10](https://medium.com/flutter/whats-new-in-flutter-2-10-5aafb0314b12?utm_campaign=thisweekinreact&utm_medium=email&utm_source=Revue%20newsletter)
-   [Announcing Flutter for Windows](https://medium.com/flutter/announcing-flutter-for-windows-6979d0d01fed?utm_campaign=thisweekinreact&utm_medium=email&utm_source=Revue%20newsletter)
-   [Push Notifications, WebXR, and better PWA support coming to iOS](https://firt.dev/ios-15.4b/?utm_campaign=thisweekinreact&utm_medium=email&utm_source=Revue%20newsletter)
-   [A TypeScript Perspective on Go: the 2021 Advent of Code](https://effectivetypescript.com/2022/02/06/advent-of-code-2021-golang/?utm_campaign=thisweekinreact&utm_medium=email&utm_source=Revue%20newsletter)
-   [DesignSystem.tools](https://www.designsystem.tools/?utm_campaign=thisweekinreact&utm_medium=email&utm_source=Revue%20newsletter)
-   [Vue 3 as the New Default](https://twitter.com/vuejs/status/1490592213184573441?utm_campaign=thisweekinreact&utm_medium=email&utm_source=Revue%20newsletter)
-   [Chrome 99: CSS Cascade Layers, a New Picker for Input Elements, and More](https://blog.chromium.org/2022/02/chrome-99-css-cascade-layers-new-picker.html?utm_campaign=thisweekinreact&utm_medium=email&utm_source=Revue%20newsletter)
-   [Electron 17](https://www.electronjs.org/blog/electron-17-0?utm_campaign=thisweekinreact&utm_medium=email&utm_source=Revue%20newsletter)
-   [*“Did ya know you probably should be using `interface` rather than `type` where possible?”*](https://twitter.com/alexdotjs/status/1489766836912668672?utm_campaign=thisweekinreact&utm_medium=email&utm_source=Revue%20newsletter)
-   [Stackshare: Top 100+ Developer Tools 2021](https://stackshare.io/posts/top-developer-tools-2021?utm_campaign=thisweekinreact&utm_medium=email&utm_source=Revue%20newsletter)
-   [Use Streams to Build High-Performing Node.js Applications](https://blog.appsignal.com/2022/02/02/use-streams-to-build-high-performing-nodejs-applications.html?utm_campaign=thisweekinreact&utm_medium=email&utm_source=Revue%20newsletter)
-   [Using fetch(), AbortSignal, And setTimeout() To Apply Retry Mechanics In JavaScript](https://www.bennadel.com/blog/4200-using-fetch-abortsignal-and-settimeout-to-apply-retry-mechanics-in-javascript.htm?utm_campaign=thisweekinreact&utm_medium=email&utm_source=Revue%20newsletter)
-   [Yes, I can connect to a DB in CSS](https://www.leemeichin.com/posts/yes-i-can-connect-to-a-db-in-css.html?utm_campaign=thisweekinreact&utm_medium=email&utm_source=Revue%20newsletter)
-   [Custom Highlight API](https://twitter.com/patrickbrosset/status/1484197202461401090?utm_campaign=thisweekinreact&utm_medium=email&utm_source=Revue%20newsletter)
-   [Wolvic: AR/VR browser](https://twitter.com/tomayac/status/1489256709163929606?utm_campaign=thisweekinreact&utm_medium=email&utm_source=Revue%20newsletter)
-   [When should you leverage Module Federation, and how?](https://scriptedalchemy.medium.com/when-should-you-leverage-module-federation-and-how-2998b132c840?utm_campaign=thisweekinreact&utm_medium=email&utm_source=Revue%20newsletter)

订阅原文：https://www.getrevue.co/profile/thisweekinreact
