This Week In React #111: Reassure, Multiplayer Cursors, Next.js, Meteor, Storybook, TanStack, FlashList, Bun...
===

Hello everyone!

Another week with a lot of cool releases, like Reassure, FlashList or Bun 🤯

---

## React

[**Reassure**](https://github.com/callstack/reassure?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)


Reassure是一个新的React性能测试库。之前已经介绍过了，现在已经由Callstack开源了。它允许在检测到性能退步时在pull-request中发布一个报告。例如：一个组件的重现速度较慢，或比以前更频繁。目前只支持React-Native，但web端很快也会支持。


[**How to animate multiplayer cursors**](https://liveblocks.io/blog/how-to-animate-multiplayer-cursors?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)

一篇很好的互动文章，建议在几个浏览器上实时地对鼠标光标进行动画处理。这是个比看起来更复杂的问题。每种方法都用React实现来说明，并使用了不同的策略：CSS过渡、弹簧、样条......

[**How to Use Next.js Middleware**](https://www.ctnicholas.dev/articles/how-to-use-nextjs-middleware?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)

来自同一作者的互动文章，介绍了许多中间件的使用案例。这篇文章已经发表在这里，刚刚在Next.js 12.2正式发布后进行了更新，其中包括一些突破性的变化。

[**10 Years Of Meteor**](https://meteor10.sachagreif.com/?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)

Sacha Grief（《Discover Meteor》的合著者，也是《JS状态》、《CSS调查》......的作者）回顾了他个人与这个框架的10年历史。Meteor已经失去了知名度，但仍然被使用，并且极大地影响了我们的前端生态系统。

[**The mystery of React Element, children, parents and re-renders**](https://www.developerway.com/posts/react-elements-children-parents?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)


Nadia强调了一些可能令人惊讶甚至反直觉的React行为，并解释了在哪些情况下，父方的重新渲染会触发子方在各种边缘情况下的重新渲染。

[**Storybook Community Showcase #2**](https://storybook.js.org/blog/community-showcase-2/?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)

来自Storybook社区的最新消息摘要。组件百科全书、Figma插件、Story Explorer和各种附加组件。变体、CSS变量、Recoil...

[**The new wave of React state management**](https://frontendmastery.com/posts/the-new-wave-of-react-state-management/?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)

介绍了状态管理库需要解决的不同问题，并对其中一些问题进行了比较。前/后Redux的回顾。完整的文章，但相当长：不容易阅读。

**拓展阅读**

-   📜 [Deploy Next.js 12.2 on Netlify today](https://www.netlify.com/blog/deploy-nextjs-12-2/?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter): Next.js latest edge features can run on Netlify too
-   📜 [Use Next.js 12.2 On-Demand ISR to automatically refresh stale data](https://jonmeyers.io/blog/use-next-js-12-2-on-demand-isr-and-supabase-function-hooks-to-automatically-refresh-stale-data?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)
-   📖 [Thinking in Efffects](https://twitter.com/dan_abramov/status/1544090471655415810?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter): new doc page, work-in-progress
-   🐦 [Remix + Svelte](https://twitter.com/crim_codes/status/1542684471195045889?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)
-   🐦 [Astro Preact compat option](https://twitter.com/astrodotbuild/status/1542511038230237185?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)
-   🎥 [A Fresh new web framework is out](https://www.youtube.com/watch?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter&v=4boXExbbGCk)
-   📦 [FramerMotion 6.4](https://twitter.com/mattgperry/status/1544323698211045376?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter): new hook useInView()
-   📦 [TanStack Table v8](https://twitter.com/tannerlinsley/status/1542925072502968320?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter): new React-Table version is now framework-agnostic and also supports Svelte, Solid, Vue
-   📦 [storybook-addon-docusaurus](https://storybook.js.org/addons/storybook-addon-docusaurus?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)

## React-Native

[**FlashList - Fast & Performant React Native List**](https://shopify.github.io/flash-list/?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)

Shopify刚刚发布了FlashList，它是FlatList的替代品，以解决滚动时的性能问题，避免显示空单元格。目标是即使在低端Android设备上也能保持60fps，而不使实现复杂化。该库重用了已经渲染好的单元格：你必须调整你对React `key`的使用，让它来接管。

[**React-Native-Compat-Table**](https://retyui.github.io/react-native-compat-table/?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)

全面列出了每个React-Native运行时（JSC、V8、Android...）的API支持。作者还解释了 [为什么React Native推荐TS配置库。"es2017" ](https://dev.to/retyui/why-react-native-typescript-config-recommends-to-use-a-five-years-old-standard-lib-es2017-3bjk?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)

**拓展阅读**

-   📜 [What's New in React Native 0.69 --- How to Upgrade and Why it Matters](https://blog.devgenius.io/whats-new-in-react-native-0-69-how-to-upgrade-and-why-it-matters-59f0841c08fc?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)
-   🧵 [Expo 46 + web](https://twitter.com/Baconbrix/status/1542431795903451136?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter): Evan Bacon gives details about changes in web support and also confirms the ambition to replace Webpack by Metro.
-   🧵 [React-Native vs mobile native trends](https://twitter.com/GergelyOrosz/status/1542020036587667457?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter): the development of native apps seems to decrease.
-   🐦 [FlatList vs FlashList perf comparison](https://twitter.com/almouro/status/1542848782693449728?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)
-   🐦 [React-Native vs Flutter diagram](https://twitter.com/t3dotgg/status/1544168855412428801?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)
-   🐦 [Webpack Module Federation + React Native](https://twitter.com/ScriptedAlchemy/status/1542311673964273664?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)
-   🎙️ [RNR 241 - Redux Toolkit vs MobX-State-Tree Showdown](https://reactnativeradio.com/episodes/rnr-241-redux-toolkit-vs-mobx-state-tree-showdown?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)
-   🎥 [The React Native Avengers: GestureHandler, Reanimated, and Skia](https://www.youtube.com/watch?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter&v=yBuhnVDXekQ)

---

## Other

[**Bun - an incredibly fast all-in-one JavaScript runtime.**](https://bun.sh/?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)

一个新的JavaScript运行时，在性能上直接与Node.js和Deno竞争，基于JSC（不是V8），用Zig编写。一个完整的工具链，包括捆绑器、转译器、包管理器，甚至测试运行器。我们去年已经谈到了Bun捆绑器，但范围已经扩大到更大的东西，0.1版本刚刚发布。

**拓展阅读**

-   [Safari Technology Preview 148](https://webkit.org/blog/12992/release-notes-for-safari-technology-preview-148/?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter): :has(), Container Queries, inert...
-   [New to the web platform in June](https://web.dev/web-platform-06-2022/?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)
-   [Color.js: A library that takes color seriously](https://lea.verou.me/2022/06/releasing-colorjs/?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)
-   [Faster page loads using server think-time with Early Hints](https://developer.chrome.com/blog/early-hints/?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)
-   [The end of Internet Explorer](https://web.dev/the-end-of-ie/?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)
-   [TransformStream is now supported cross-browser](https://web.dev/transformstream/?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)
-   [wasmbuild - Using Rust in Deno and Web Apps](https://deno.com/blog/wasmbuild?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)
-   [CSS Cascade Layers -- There's a Polyfill for That!](https://www.oddbird.net/2022/06/21/cascade-layers-polyfill/?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)
-   [CSS - Breaking Out of a Central Wrapper](https://css-irl.info/breaking-out-of-a-central-wrapper/?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)
-   [Vue 2.7 "Naruto"](https://blog.vuejs.org/posts/vue-2-7-naruto.html?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)

<img width="687" alt="CleanShot 2022-07-06 at 12 16 27@2x" src="https://user-images.githubusercontent.com/749374/177528236-692a4831-67d0-48d7-926c-f7e2d57a836e.png">



  订阅原文:
-   🇬🇧 [ThisWeekInReact.com](https://thisweekinreact.com/)
-   🇫🇷 [ReactHebdo.fr](https://reacthebdo.fr/)
