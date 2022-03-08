# React

[**Using global memoization in React**](https://thoughtspile.github.io/2022/02/09/react-global-memo/?utm_campaign=thisweekinreact&utm_medium=email&utm_source=Revue%20newsletter)

Vladimir解释说，有时候仅仅使用useMemo是不够的，我们需要在多个组件之间共享缓存数据。他提出了5种在React组件外以全局方式缓存数据的方法，从单个常量到LRU缓存。我的观点：使用[WeakMap](https://javascript.info/weakmap-weakset?utm_campaign=thisweekinreact&utm_medium=email&utm_source=Revue%20newsletter)也可以是一个不错的解决方案，为什么不在React上下文中提供缓存呢？

[**React component as prop: the right way™️**](https://www.developerway.com/posts/react-component-as-prop-the-right-way?utm_campaign=thisweekinreact&utm_medium=email&utm_source=Revue%20newsletter)

Nadia给出了使用React composition的充分理由。她以一个带有文本+图标的按钮为例，提出了3个备选方案，并在不同的更新场景下对它们进行了比较。
-   `icon={<MyIcon/>}`
-   `Icon={MyIcon}`
-   `renderIcon={(...settings) <Icon {...settings}/>}` 

我不太喜欢第一种情况，并尽量避免使用`cloneElement`。

## **拓展阅读:**
-   📜 [Remix upload to S3](https://www.canrau.com/en/remix-upload-to-s3?utm_campaign=thisweekinreact&utm_medium=email&utm_source=Revue%20newsletter): 使用Remix API将上传流直接转发至S3
-   📦 [Remix Electron](https://github.com/itsMapleLeaf/remix-electron?utm_campaign=thisweekinreact&utm_medium=email&utm_source=Revue%20newsletter): Remix和Electron的整合🤔似乎很有趣，可以减少Electron的模板，并提供更好的网络+本地代码的共同定位。
-   📦 [Griffel](https://github.com/microsoft/griffel?utm_campaign=thisweekinreact&utm_medium=email&utm_source=Revue%20newsletter): 微软对[原子式CSS-in-JS](https://sebastienlorber.com/atomic-css-in-js?utm_campaign=thisweekinreact&utm_medium=email&utm_source=Revue%20newsletter)、零运行时间、类型安全的看法。提醒我们，我们仍在等待StyleX😏。
-   📦 [Jotai 1.6](https://twitter.com/dai_shi/status/1492132198375657474?utm_campaign=thisweekinreact&utm_medium=email&utm_source=Revue%20newsletter): 暴露存储接口，原子与localStorage同步…
-   🗳 [Next.js Developer Survey](http://vercel.link/nextjs-survey?utm_campaign=thisweekinreact&utm_medium=email&utm_source=Revue%20newsletter): Vercel官方调查
-   💡 [Next.js RFC: Switchable Runtime](https://github.com/vercel/next.js/discussions/34179?utm_campaign=thisweekinreact&utm_medium=email&utm_source=Revue%20newsletter): Next.js中的SSR在历史上是基于Node.js的运行时。他们计划引入全局和每条线路的配置来启用Edge运行时。这在很多方面都很有趣：启用流式SSR，降低延迟......请注意，Remix由于其适配器层，已经在某种程度上具备了这种能力。
-   💡 [Gatsby RFC: Ahead of Time Compilation for config files](https://github.com/gatsbyjs/gatsby/discussions/34613?utm_campaign=thisweekinreact&utm_medium=email&utm_source=Revue%20newsletter): 来支持TypeScript中的配置文件。顺便说一下，我发现了一个有趣的包，用于这个用途：[bundle-require](https://github.com/egoist/bundle-require?utm_campaign=thisweekinreact&utm_medium=email&utm_source=Revue%20newsletter)
-   💡 [Flat file system for file-based routing](https://gist.github.com/jamiebuilds/86d467ee4353cb316edce8e69ad19237?utm_campaign=thisweekinreact&utm_medium=email&utm_source=Revue%20newsletter): 杰米-凯尔关于文件系统路由约定的强烈和原创的意见 🤔
-   📖 [Partytown + Hydrogen](https://partytown.builder.io/shopify-hydrogen?utm_campaign=thisweekinreact&utm_medium=email&utm_source=Revue%20newsletter): 新的整合文档
-   🐦 [Remix: animated page transitions with useOutlet()](https://twitter.com/buildsghost/status/1492201302423605252?utm_campaign=thisweekinreact&utm_medium=email&utm_source=Revue%20newsletter): Outlet是一个很好的解决方案，可以避免布局的卸载/重载，使其更容易实现页面的转换。
-   🎥 [Remotion Update - February 2022](https://www.youtube.com/watch?utm_campaign=thisweekinreact&utm_medium=email&utm_source=Revue%20newsletter&v=fF_ABGkrKmg)
-   📜 [Hydrogen & Tailwind: The Perfect Match](https://shopify.engineering/hydrogen-tailwind-building-beautiful-storefronts?utm_campaign=thisweekinreact&utm_medium=email&utm_source=Revue%20newsletter): 来自Shopify，有一点像React，更像是Tailwind。
-   📜 [Svelte vs. React in 2022: Choosing the Best Match for You](https://prismic.io/blog/compare-svelte-vs-react-2022?utm_campaign=thisweekinreact&utm_medium=email&utm_source=Revue%20newsletter) 

# React-Native 
[**Measuring and improving performance on a React Native app**](https://blog.bam.tech/developer-news/measuring-and-improving-performance-on-a-react-native-app?utm_campaign=thisweekinreact&utm_medium=email&utm_source=Revue%20newsletter)

Alexandre介绍了他的Flipper插件，可以持续测量React-Native的性能（UI和JS线程FPS），并像Lighthouse一样计算得分。他还分享了4个技巧，帮助你测量你的应用程序的性能。TIL关于用`adb`自动滚动。所有这些都被应用在一个具体的案例中：他的团队将TF1应用的分数从40分提高到90分。

## **拓展阅读:**
-   📜 [4 years as a React Native OSS maintainer: a retrospective](https://gist.github.com/kelset/05ae2f4a861c2252fc592ebadd7e0f25?utm_campaign=thisweekinreact&utm_medium=email&utm_source=Revue%20newsletter): 做一个维护者并不容易 😅
-   📜 [Calling Windows APIs from React Native just got easier](https://microsoft.github.io/react-native-windows/blog/2022/02/11/rnwinrt?utm_campaign=thisweekinreact&utm_medium=email&utm_source=Revue%20newsletter): 微软推出了一个新的React-Native包，以一种非常灵活的方式直接从JS中调用任何WinRT API，而不需要任何额外的模板。请注意，iOS也有类似的举措（[react-native-native-runtime](https://github.com/shirakaba/react-native-native-runtime?utm_campaign=thisweekinreact&utm_medium=email&utm_source=Revue%20newsletter)），但不确定苹果是否会批准。😝
-   📜 [React Native for Windows is helping Settings improve more quickly](https://microsoft.github.io/react-native-windows/blog/2022/02/11/settings?utm_campaign=thisweekinreact&utm_medium=email&utm_source=Revue%20newsletter): M微软对一个具体的跨平台用例的反馈，他们在桌面（使用上述WinRT包）和网络之间共享代码。
-   🎥 [Orta Dev Diary 2 - React Native Web](https://www.youtube.com/watch?utm_campaign=thisweekinreact&utm_medium=email&utm_source=Revue%20newsletter&v=2NItowAgfNA)
-   🎙️ [RNR 226 - GraphQL in React Native](https://reactnativeradio.com/episodes/rnr-226-graphql-in-react-native?utm_campaign=thisweekinreact&utm_medium=email&utm_source=Revue%20newsletter)

# Other 
[**Hello, CSS Cascade Layers**](https://ishadeed.com/article/cascade-layers/?utm_campaign=thisweekinreact&utm_medium=email&utm_source=Revue%20newsletter)

对CSS Cascade layers的一个很好的介绍，这是一个值得期待的CSS新功能。看起来它在我们的浏览器中[很快会被支持](https://twitter.com/stefanjudis/status/1492655597459808258?utm_campaign=thisweekinreact&utm_medium=email&utm_source=Revue%20newsletter)，即使你今天不能使用它（没有polyfill），那也值得看一看。CSS Cascade Laters对CSS级联给予额外的控制以及应用CSS规则的顺序。这可以帮助修复与特异性、插入顺序有关的问题，或者减少使用！`!important`。如果你只有1分钟时间，[可以看一眼这个动画](https://twitter.com/bramus/status/1493330153681920001?utm_campaign=thisweekinreact&utm_medium=email&utm_source=Revue%20newsletter)。

这就像浏览器重新排列了你的样式，而不是使用CSS文件中定义的顺序。[这让我想起了React](https://twitter.com/threepointone/status/1056594421079261185?utm_campaign=thisweekinreact&utm_medium=email&utm_source=Revue%20newsletter) 😅.为什么这很重要？因为捆绑器和前端工具没有任何明确的规则，以正确的可预测的顺序发出捆绑的CSS。例如，使用Webpack、CSS加载器、JS/CSS代码分割、动态导入、CJS/ESM，你真的知道你的CSS规则在最终页面中的顺序是什么？我绝对不知道! 🤷♂️有了这个新功能，你的CSS可能会变得更加便携。如果有一天你决定使用另一个捆绑器/工具，你不希望不得不重写一切，并修复一大堆与CSS插入顺序变化有关的小CSS问题：Cascade layers,可以防止这种情况。

这些天在CSS方面有很多活动。还可以看看[Interop 2022](https://www.bram.us/2022/02/13/interop-2022/?utm_campaign=thisweekinreact&utm_medium=email&utm_source=Revue%20newsletter)项目：浏览器计划在今年关注的有关浏览器兼容性的功能，包括cascade layers

## **拓展阅读:**
-   [Announcing TypeScript 4.6 RC](https://devblogs.microsoft.com/typescript/announcing-typescript-4-6-rc/?utm_campaign=thisweekinreact&utm_medium=email&utm_source=Revue%20newsletter): great [improvements on Control Flow Analysis](https://twitter.com/sebastienlorber/status/1488096041299816453?utm_campaign=thisweekinreact&utm_medium=email&utm_source=Revue%20newsletter), very nice for React
-   [Typescript - (ReadOnly) NotEmptyArray](https://dev.to/this-is-learning/typescript-readonlynotemptyarray-2id7?utm_campaign=thisweekinreact&utm_medium=email&utm_source=Revue%20newsletter): 需要了解的有用元组技术: `[T, ...T[]];`
-   [Assertion Functions in TypeScript](https://mariusschulz.com/blog/assertion-functions-in-typescript?utm_campaign=thisweekinreact&utm_medium=email&utm_source=Revue%20newsletter): useful feature for type-narrowing
-   [*“Extract in TS can be used to query a member of a union type.”*](https://twitter.com/farzad_yz/status/1492127144423694338?utm_campaign=thisweekinreact&utm_medium=email&utm_source=Revue%20newsletter)
-   [SWC v1.2.139](https://twitter.com/swc_rs/status/1492454606118752257?utm_campaign=thisweekinreact&utm_medium=email&utm_source=Revue%20newsletter): 介绍新的Rust插件系统
-   [Why I prefer JS for front-end build automation](https://thoughtspile.github.io/2022/02/14/js-automation/?utm_campaign=thisweekinreact&utm_medium=email&utm_source=Revue%20newsletter): 可以肯定的是，它比bash要好 😅
-   [npm RFC **:** Package Distributions](https://github.com/npm/rfcs/pull/519?utm_campaign=thisweekinreact&utm_medium=email&utm_source=Revue%20newsletter): 为需要发布特定平台二进制文件的lib作者提出新的解决方案。看起来对Rust和Go的现代工具很有用。
-   [Node.js 17.5.0](https://twitter.com/ruyadorno/status/1491847226662043649?utm_campaign=thisweekinreact&utm_medium=email&utm_source=Revue%20newsletter): fetch (behind flag), JSON modules
-   [Jest v28.0 alpha](https://twitter.com/thymikee/status/1492065154258935823?utm_campaign=thisweekinreact&utm_medium=email&utm_source=Revue%20newsletter): ligher, remove deps JSDOM, Jasmine
-   [AbortController -> TaskController](https://twitter.com/sebmarkbage/status/1492142346867286018?utm_campaign=thisweekinreact&utm_medium=email&utm_source=Revue%20newsletter): assign priority to JS tasks?
-   [Parcel 2.3](https://twitter.com/parceljs/status/1491465162456502274?utm_campaign=thisweekinreact&utm_medium=email&utm_source=Revue%20newsletter) + [Parcel CSS 1.3](https://twitter.com/devongovett/status/1493256831879237632?utm_campaign=thisweekinreact&utm_medium=email&utm_source=Revue%20newsletter) + [Webpack integration example](https://twitter.com/devongovett/status/1491818780418318336?utm_campaign=thisweekinreact&utm_medium=email&utm_source=Revue%20newsletter)
-   [EdgeDB 1.0](https://www.edgedb.com/blog/edgedb-1-0?utm_campaign=thisweekinreact&utm_medium=email&utm_source=Revue%20newsletter) with a [query builder TypeScript](https://twitter.com/edgedatabase/status/1491534099042897923?utm_campaign=thisweekinreact&utm_medium=email&utm_source=Revue%20newsletter)
-   [Rome Formatter and Rust Update](https://rome.tools/blog/2022/02/08/rome-formatter-and-rust-update?utm_campaign=thisweekinreact&utm_medium=email&utm_source=Revue%20newsletter): initial focus seems to be on a code formatter that will try to [sync with Prettier](https://twitter.com/Vjeux/status/1491180045905567744?utm_campaign=thisweekinreact&utm_medium=email&utm_source=Revue%20newsletter).
-   [Flutter in 2022: strategy and roadmap](https://medium.com/flutter/flutter-in-2022-strategy-and-roadmap-8c5eaf7c4275?utm_campaign=thisweekinreact&utm_medium=email&utm_source=Revue%20newsletter): improvements planned on web support
-   [Vite 2.8](https://twitter.com/vite_js/status/1491407504336879617?utm_campaign=thisweekinreact&utm_medium=email&utm_source=Revue%20newsletter)
-   [ESLint 8.9](https://eslint.org/blog/2022/02/eslint-v8.9.0-released?utm_campaign=thisweekinreact&utm_medium=email&utm_source=Revue%20newsletter)
-   [Is Turborepo overhyped?](https://tolgee.io/blog/turborepo-overhyped?utm_campaign=thisweekinreact&utm_medium=email&utm_source=Revue%20newsletter)
-   [Move over JavaScript: Back-end languages are coming to the front-end](https://github.com/readme/featured/server-side-languages-for-front-end?utm_campaign=thisweekinreact&utm_medium=email&utm_source=Revue%20newsletter)
-   [Storybook: Component Encyclopedia beta](https://storybook.js.org/blog/component-encyclopedia-beta/?utm_campaign=thisweekinreact&utm_medium=email&utm_source=Revue%20newsletter)
-   [Static Files on Deno Deploy](https://deno.com/blog/deploy-static-files?utm_campaign=thisweekinreact&utm_medium=email&utm_source=Revue%20newsletter)
-   [Debugging JavaScript](https://flaviocopes.com/debugging/?utm_campaign=thisweekinreact&utm_medium=email&utm_source=Revue%20newsletter)
-   [Inside the JavaScript Engine](https://blog.devgenius.io/inside-the-javascript-engine-bb7b9f26e84b?utm_campaign=thisweekinreact&utm_medium=email&utm_source=Revue%20newsletter)
-   [Design system versioning: single library or individual components?](https://bradfrost.com/blog/post/design-system-versioning-single-library-or-individual-components/?utm_campaign=thisweekinreact&utm_medium=email&utm_source=Revue%20newsletter)
-   [How not to learn GraphQL](https://www.the-guild.dev/blog/how-not-to-learn-graphql?utm_campaign=thisweekinreact&utm_medium=email&utm_source=Revue%20newsletter)
-   [Implementing A Svelte Store In Rust](https://daveceddia.com/svelte-store-in-rust/?utm_campaign=thisweekinreact&utm_medium=email&utm_source=Revue%20newsletter)
-   [The first developer preview of Android 13](https://android-developers.googleblog.com/2022/02/first-preview-android-13.html?utm_campaign=thisweekinreact&utm_medium=email&utm_source=Revue%20newsletter)
-   [Server-Sent Events: the alternative to WebSockets you should be using](https://germano.dev/sse-websockets/?utm_campaign=thisweekinreact&utm_medium)

订阅原文：https://www.getrevue.co/profile/thisweekinreact
