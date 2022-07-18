This Week In React #110: Fresh, Hydrogen, Next.js, Remix, Storybook, useEffect, MJML, MDX, React-Native, ES2022...
===

Hi everyone!

Another busy week with lots of releases 🤪 Hydrogen 1.0, Fresh 1.0, Next.js 12.2, React-Native 0.69...

大家好!

又是一个忙碌的一周，发布了很多🤪Hydrogen1.0、Fresh 1.0、Next.js 12.2、React-Native 0.69...

React官方下场，不支持通过useEffect来获取数据。

---

## React

[Fresh 1.0](https://deno.com/blog/fresh-is-stable?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)

Deno正式支持的Preact框架现在是v1版，被认为是可以投入生产的。Fresh让我想起了Remix和Astro之间的混合体：默认没有JS，渐进式增强，多页面应用程序与islands architecture。没有构建步骤：你可以在几秒钟内直接将你的TypeScript/Deno应用部署到Edge上。

[How We Built Hydrogen](https://shopify.engineering/how-we-built-hydrogen?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)

Hydrogen是Shopify用于构建电子商务商店的React元框架，刚刚发布了v1.0版本，是第一批依靠React服务器组件的框架之一。这篇文章是对该框架创建的一个有趣的反馈，详细介绍了随着时间推移所做的各种选择。React服务器组件、Vite、Tailwind、预加载/瀑布、GraphQL片段......

[Next.js 12.2](https://nextjs.org/blog/next-12-2?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)


最新版本的Next.js。主要的主题是逐步采用Edge和标准化的网络API：middleware，但也有API路由和SSR。在图像方面也有改进，在WebAssembly中还有一个SWC插件系统。

[My Wonderful HTML Email Workflow](https://www.joshwcomeau.com/react/wonderful-emails-with-mjml-and-mdx/?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)

Josh Comeau解释了他是如何用MDX编写邮件的，然后使用MJML、React和Next.js来创建最终的HTML输出，这些输出可以在所有的邮件客户端中使用，通过ConvertKit发送，也可以在网上使用。

[Data Flow in Remix](https://remix.run/blog/remix-data-flow?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)

React的初始模型可以概括为`ui = f(state)`。问题是，这个模型并没有真正考虑到网络同步（即API调用）。Jim解释了Remix如何采用React模型并包括网络，从而减少对本地状态管理的需求。

[You Might Not Need an Effect](https://beta.reactjs.org/learn/you-might-not-need-an-effect?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)

由Dan Abramov编写的新文档页，刚刚合并到测试版网站。存在与外部系统同步的效果。提出了许多反模式的具体例子，甚至是挑战。即使是有经验的开发者也应该阅读它。有些东西可能会让人吃惊：比如 [在渲染时使用setState](https://twitter.com/sebastienlorber/status/1541793224561463297?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter) 😱。我特别喜欢useSyncExternalStore的例子。

[What is the recommended way to load data for React 18?](https://www.reddit.com/r/reactjs/comments/vi6q6f/what_is_the_recommended_way_to_load_data_for/?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)

Dan Abramov在Reddit上解释了为什么通过useEffect获取数据并不理想。然而，如果你的应用程序没有任何用户体验问题，就没有必要当场重写：这些问题在React 18中并不新鲜，只是有更好的记录。也请看关于React-Native数据获取的评论。

**Extras:**

-   📜 [How to add a theme switcher to Storybook](https://storybook.js.org/blog/how-to-add-a-theme-switcher-to-storybook/?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter): shows how to leverage Storybook toolbar to add a theme switch. Convenient tip: displays component in both light/dark mode.
-   📜 [React Query FAQs](https://tkdodo.eu/blog/react-query-fa-qs?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter): Dominik from React-Query answers the 3 most common questions.
-   📜 [The React core team finally have opinions about CSS](https://dev.to/hypeddev/the-react-core-team-finally-have-opinions-about-css-16f0?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter): good summary of current trends: increasing use of no-runtime CSS-in-JS.
-   📜 [Cut build times with Gatsby Runner](https://www.netlify.com/blog/cut-build-times-with-gatsby-runner/?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter): new experimental Netlify plugin to reduce Gatsby build time by delaying image processing.
-   📜 [State Machines on the Edge](https://erikras.com/blog/remixconf-2022?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter) + [Modeling React in XState](https://erikras.com/blog/modeling-react-in-xstate?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)
-   📜 [Demystifying The New Gatsby Framework](https://www.smashingmagazine.com/2022/06/demystifying-gatsby4-framework/?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)
-   📜 [Should we use Lexical to edit our legal graph?](https://medium.com/doctrine/should-we-use-lexical-to-edit-our-legal-graph-61aa9cfab096?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)
-   🎥 [Storybook in 100 Seconds](https://www.youtube.com/watch?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter&v=gdlTFPebzAU)
-   📈 [Front-end frameworks popularity (React, Vue, Angular and Svelte)](https://gist.github.com/tkrotoff/b1caa4c3a185629299ec234d2314e190?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)
-  📜 [Verbum](https://github.com/ozanyurtsever/verbum?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter): text editor based on React and Lexical (new Facebook project to replace Draft.js)
-  📦 [Storybook Variants Addon](https://twitter.com/winkerVSbecks/status/1541078873949048838?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter): convenient addon: add toolbar dropdown to display all variants of a story at once. No extra code needed: based on Controls.
-  📦 [Create-T3-App](https://github.com/nexxeln/create-t3-app?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter): modern stack to start a project: Next.js, Prisma, TypeScript, tRPC, Tailwind...
-   📦 [Gatsby 4.17](https://www.gatsbyjs.com/docs/reference/release-notes/v4.17/?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter): perf improvements
-  📦 [Recoil Sync 0.1](https://recoiljs.org/blog/2022/06/21/recoil-sync-0.1.0-release?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter) + [Refine 0.1](https://recoiljs.org/blog/2022/06/21/refine-0.1.0-release?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)
- 📦[Vavite: Develop server-side applications with Vite](https://github.com/cyco130/vavite?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)
- 🐦 [Preact will compile out unused class components](https://twitter.com/_developit/status/1541516098939543552?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)
- 🐦 [Qwik-React is coming](https://twitter.com/QwikDev/status/1540667422402920448?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)


## React-Native

[**Announcing React Native 0.69**](https://reactnative.dev/blog/2022/06/21/version-069?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)

第一个支持React 18的React-Native版本。要使用Concurrent React的新功能，你必须先迁移到新的架构。Hermes的发布模式也发生了变化：React-Native的每个版本都将与Hermes版本保证兼容。

**Extras:**

-   📦 [react-native-zephyr](https://github.com/FormidableLabs/react-native-zephyr?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter): Formidable Labs published a new React-Native type-safe styling solution inspired by Tailwind. Focusing on mobile usage, not [cross-platform](https://twitter.com/sebastienlorber/status/1541820495603064832?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter) for now.
-   📦 [react-native-app-clip](https://github.com/bndkt/react-native-app-clip?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter): Expo config plugin to create an iOS App Clip, permitting to users to test your app without even installing it ([demo](https://twitter.com/bndkt/status/1539606675291639808?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)).
-   📦 [react-native-safari-extension](https://github.com/andrew-levy/react-native-safari-extension?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)
-   📦 [link-native-assets-expo-config-plugin](https://twitter.com/Baconbrix/status/1539885820622110720?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)
-   🎙️ [RNR 240 - What's New in Expo SDK 45](https://reactnativeradio.com/episodes/rnr-240-whats-new-in-expo-sdk-45?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)
-   📈 [React-Native vs Flutter popularity](https://gist.github.com/tkrotoff/93f5278a4e8df7e5f6928eff98684979?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)
-   🐦 [Reanimated useAnimatedSensor() demo](https://twitter.com/swmansion/status/1541433419107733505?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)
-   🎉 [Reanimated PR: reduce bundle size on Web by 80%](https://github.com/software-mansion/react-native-reanimated/pull/3278?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)

## Other

-   [ES2022 Features](https://h3manth.com/ES2022/?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter): Ecma International just validated the ES2022 spec. Overview of all the features included: `.at()`, Error Cause, top-level await...
-   [Defensive CSS](https://defensivecss.dev/?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter): CSS tips to make your CSS more robust.
-   [Style Queries](https://una.im/style-queries/?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter): CSS Container Queries is not just about layouts.
-   [StackOverflow Developer Survey 2022](https://survey.stackoverflow.co/2022/?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter): React remains very used and liked. Svelte and Phoenix are good challengers.
-   [Histoire: A new way to write stories](https://histoire.dev/?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter): Storybook challenger coming from the Vue ecosystem.
-   [FnApi](https://twitter.com/kdy1dev/status/1540673590282326018?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter): new project from Donny (swc creator) to reduce API calls boilerplate
-   [Prisma 4.0](https://twitter.com/prisma/status/1541866761552908289?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)
-   [Turborepo 1.3](https://turborepo.org/blog/turbo-1-3-0?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)
-   [SPAs: theory versus practice](https://nolanlawson.com/2022/06/27/spas-theory-versus-practice/?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)

---

<img width="725" alt="CleanShot 2022-06-29 at 11 27 17@2x" src="https://user-images.githubusercontent.com/749374/176402711-1255046e-fa8b-4de4-9cbe-0632d356cef0.png">


  订阅原文:
-   🇬🇧 [ThisWeekInReact.com](https://thisweekinreact.com/)
-   🇫🇷 [ReactHebdo.fr](https://reacthebdo.fr/)
