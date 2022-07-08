## React


[**React useEvent() RFC**](https://github.com/reactjs/rfcs/blob/useevent/text/0000-useevent.md?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)

Dan Abramov的RFC建议在React核心中添加一个新的`useEvent(fn)`钩子，没有任何依赖数组。然后，作为参数传递的不稳定的函数/闭包被稳定化（它在一段时间内保持相同的身份）。这有助于避免陈旧的[闭包问题](https://tkdodo.eu/blog/hooks-dependencies-and-stale-closures?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)（当ESLint规则未配置或者不受重视时），同时通过`React.memo()`简化优化，并避免`useEffects`的重新执行。计划对ESLint规则进行修改：稳定的函数不需要传递到其他依赖数组中，可以采用 "onEvent"/"handleEvent "惯例。

我在[pull-request](https://github.com/reactjs/rfcs/pull/220?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)中给出了我的 [积极反馈](https://github.com/reactjs/rfcs/pull/220?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter#issuecomment-1135819463)（那里有很多评论，特别是关于该钩子的命名）。对我来说，这确实是最初钩子设计中缺少的一块，许多应用程序已经使用了[基于useLayoutEffect的变通方法](https://github.com/reactjs/rfcs/blob/useevent/text/0000-useevent.md?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter#internal-implementation)。

[useEvent - 缺失的React钩子](https://www.youtube.com/watch?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter&v=8BgLzG8kXmQ) 是一个很好的3分钟视频，可以了解大局。

[**Next.js Layouts RFC**](https://nextjs.org/blog/layouts-rfc?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)

Next.js将使其路由基础设施现代化。这将有助于利用React 18的功能，以及其他即将到来的功能。

他们计划逐步采用：`./pages` 文件夹继续像以前一样工作，你可以逐步把东西移到新的`./app`文件夹，这也会激活服务器组件🤯。

将支持基于`layout.js`命名惯例的嵌套路由/布局。请求将被并行执行（没有瀑布）。这篇文章只是一个巨大的RFC的第一部分：第二部分即将到来。

**拓展阅读**

-   📜 [Building a Design System from scratch](https://blog.maximeheckel.com/posts/building-a-design-system-from-scratch/?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter): Maxime sharing all the details behind his personal React [design system](https://github.com/MaximeHeckel/design-system?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter) , based on [Stitches](https://github.com/modulz/stitches?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)
-   📜 [Building a Mini Next.js](https://hire.jonasgalvez.com.br/2022/may/18/building-a-mini-next-js/?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter): Jonas shows how to replicate Next.js file-system routing and SSR with `getServerSideProps`, using Vite and Fastify.
-   📜 [Remix and "The Edge"](https://remix.run/blog/remix-and-the-edge?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter): Jim recently [joined the Remix team](https://blog.jim-nielsen.com/2022/joining-remix/?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter). This explains how Remix leverages the Edge (ie Deno and Cloudflare Workers 😏) to be both fast and dynamic.
-   📜 [Storybook Performance: Vite vs Webpack](https://storybook.js.org/blog/storybook-performance-from-webpack-to-vite/?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter): Storybook has pluggable builders, so which one to use? This benchmark shows that Vite does not always win against Webpack, on a large IBM Carbon 250 comps Storybook
-   📜 [What the useEvent React hook is (and isn't)](https://typeofnan.dev/what-the-useevent-react-hook-is-and-isnt/?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter): opinion of a Solid contributor
-   📜 [Getting started with Markdoc in Next.js](https://dev.to/stripe/getting-started-with-markdoc-in-nextjs-ioj?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter): Stripe just open-sourced their doc tool [Markdoc](https://markdoc.io/?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)
-   📜 [React key attribute: best practices for performant lists](https://www.developerway.com/posts/react-key-attribute?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter): good illustration on problems happening when you use index or random keys
-   📜 [(P)react vs Web Components: a Xoogler's perspective](https://whistlr.info/2022/react-preact-wc/?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)
-   📜 [Reading Source Code: React-Query](https://alexkondov.com/reading-source-code-react-query/?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)
-   📜 [You Don't Need A UI Framework](https://www.smashingmagazine.com/2022/05/you-dont-need-ui-framework/?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)
-   📜 [What You Need to Do to Improve Performance in Next.js](https://www.builder.io/blog/fast-to-faster-what-you-need-to-do-to-improve-performance-in-nextjs?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)
-   📜 [How to solve React useEffect infinite loops](https://blog.logrocket.com/solve-react-useeffect-hook-infinite-loop-patterns/?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)
-   📜 [What I learnt at Reactathon 2022](https://dev.to/shrutikapoor08/what-i-learnt-at-reactathon-2022-3e3a?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)
-   📜 [Using Next.js ISR with Serverless Cloud](https://www.serverless.com//blog/using-next-js-isr-with-serverless-cloud?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)
-   👥 [Remix Conf](https://remix.run/conf?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter): starts today!
-   👥 Reactathon 2022 livestreams: [day 1](https://www.youtube.com/watch?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter&v=V5hPAl1q7vo), [day 2](https://www.youtube.com/watch?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter&v=Ck-e3hd3pKw), [day 3](https://www.youtube.com/watch?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter&v=0qK2_wi4t3k)
-   🧑‍🎓 [Advanced-Remix](https://github.com/kentcdodds/advanced-remix?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter): workshop open-sourced by Kent
-   🧑‍🎓 [Complex State Management in React with Jotai and XState](https://egghead.io/courses/complex-state-management-in-react-with-jotai-and-xstate-3be0a740?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)
-   🐦 [TypeScript 4.8 + "as props"](https://twitter.com/diegohaz/status/1526618550105870337?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter): possible improvement?
-   🐦 [well-named function inside useEffect](https://twitter.com/housecor/status/1528707302483697666?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)
-   📦 [eslint-plugin-react v7.30](https://github.com/jsx-eslint/eslint-plugin-react/releases/tag/v7.30.0?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter): new [jsx-no-leaked-render](https://github.com/jsx-eslint/eslint-plugin-react/blob/v7.30.0/docs/rules/jsx-no-leaked-render.md?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter) rule very useful. Permits to avoid rendering a 0 with `{count && <div>{count}</div>}` (which makes React-Native crash 😅)
-   📦 [Remix 1.5](https://twitter.com/remix_run/status/1527288716837867526?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter): officiel Deno support
-   📦 [Reagraph](https://github.com/reaviz/reagraph?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter): WebGL Graph Visualizations
-   📦 [Playright 1.22](https://github.com/microsoft/playwright/releases/tag/v1.22.0?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter): possible to test React components


## React-Native

[**Announcing Reanimated 3**](https://blog.swmansion.com/announcing-reanimated-3-16167428c5f7?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)

新版本在RC中。支持新的Fabric架构，但也支持旧的架构，以帮助逐步采用。Reanimated v2代码继续在v3上工作，但旧的Reanimated v1 API被删除 [demo Reanimated 3 + RNGH + Screens](https://twitter.com/tomekzaw_/status/1526977496415092736?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)

[**Microsoft - React Native Developer Tools**](https://microsoft.github.io/rnx-kit/blog/react-native-developer-tools?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)

Adam宣布启动React Native开发者工具社区项目。这是一个repo([rnx-kit](https://github.com/microsoft/rnx-kit?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter))，里面有许多对React-Native项目[有用的工具](https://microsoft.github.io/rnx-kit/docs/tools/overview?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)，与Metro、TypeScript、Jest有关。微软已经在Office、Xbox和Teams等各种产品上使用它。

**拓展阅读**

-   📜 [Expo SDK 45](https://blog.expo.dev/expo-sdk-45-f4e332954a68?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter): using latest React-Native 0.68.2 version. New Expo Go UI with better EAS Updates integration. Modules upgraded to JSI and Sweet API. New CLI in beta.
-   📜 [Tamagui Beta](https://tamagui.dev/blog/tamagui-enters-beta-themes-and-animations?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter): promising cross-platform tool now available in beta. Starter available using Expo, Next.js and Solito.
-   📜 [React Native Accessibility - GAAD 2022 Update](https://reactnative.dev/blog/2022/05/19/GAAD-2022-update?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)
-   🎥 [It's Severance, but in React Native](https://www.youtube.com/watch?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter&v=fMMj9oWbWL8): latest William Candillon video with Skia, Perlin Noise and shaders. As good as the [TV show](https://www.imdb.com/title/tt11280740/?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter). Remotion intros/outros are back👌
-   🎙️ [The React Native Show - Coffee Talk #2 - Top Resources for Developers](https://www.callstack.com/podcasts/coffee-talk-2-top-resources-for-developers?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)
-   🎙️ [RNR 234 - React Native Tips and Tricks](https://reactnativeradio.com/episodes/rnr-234-react-native-tips-and-tricks?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)
-   🎙️ [RNR 235 - Dissecting React Native 0.68](https://reactnativeradio.com/episodes/rnr-235-dissecting-react-native-068?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)
-   🎙️ [RNR 236 - Reanimated 2 with Krzysztof Magiera](https://reactnativeradio.com/episodes/rnr-236-reanimated-2-with-krzysztof-magiera?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)
-   📦 [6 Expo 45 clones](https://github.com/calebnance?language=&q=clone&sort=stargazers&tab=repositories&type=source&utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter): Spotify, Uber, Netflix, Slack, Twitch, Disney+
-   🐦 [Tesla app using React-Native](https://twitter.com/aarongrider/status/1526963131821355008?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)
-   🐦 [React-Native 0.69: faster & ~5% less RAM usage](https://twitter.com/ReactNativeMSFT/status/1528788635692109824?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)

## 其它

-   [JavaScript Containers](https://tinyclouds.org/javascript_containers?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)
-   [A Community Group for Web-interoperable JavaScript runtimes](https://blog.cloudflare.com/introducing-the-wintercg/?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)
-   [Google I/O 2022 Recap](https://web.dev/googleio22-recap/?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)
-   [Interaction to Next Paint (INP)](https://web.dev/inp/?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)
-   [State of CSS 2022](https://web.dev/state-of-css-2022/?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)
-   [TypeScript 4.7 RC](https://devblogs.microsoft.com/typescript/announcing-typescript-4-7-rc/?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter) + [TypeScript 4.8 Iteration Plan](https://github.com/microsoft/TypeScript/issues/49074?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)
-   [Stripe: Migrating millions of lines of code to TypeScript](https://stripe.com/blog/migrating-to-typescript?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)
-   [Deno 1.22 Release Notes](https://deno.com/blog/v1.22?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)
-   [Lerna is dead --- Long Live Lerna](https://blog.nrwl.io/lerna-is-dead-long-live-lerna-61259f97dbd9?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)
-   [Transferring Jest to the OpenJS Foundation](https://engineering.fb.com/2022/05/11/open-source/jest-openjs-foundation/?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)
-   [Flutter 3](https://medium.com/flutter/introducing-flutter-3-5eb69151622f?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)


<img width="640" alt="CleanShot 2022-05-25 at 09 16 29@2x" src="https://user-images.githubusercontent.com/749374/170203328-b5d82a2f-fb91-46e1-98f1-e290d2e2119e.png">

  
  订阅原文:
-   🇬🇧 [ThisWeekInReact.com](https://thisweekinreact.com/)
-   🇫🇷 [ReactHebdo.fr](https://reacthebdo.fr/)
