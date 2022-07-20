This Week In React #112: JSX Expressions, Storybook, Remix, Actionless reducers, Atomic Forms, NPM trends, Expo, RN Keyboard, Bun...
===

大家好!

看起来很多开发者都已经在度假了😎。在我这边，我也会在这个夏天跳过一些版本来休息。

这周，我们有很多React和React-Native的内容。很多来自社区的关于[Bun](https://bun.sh/?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)的非常积极的反馈!

(译者注：羡慕法国人假期多，这应该是今年的第三次休假了！由于上海疫情耽搁近3个月的周刊终于赶上Sébastien的进度了，下次将会开始同步最新周刊回复每周一次的更新频率以及拖了N久的react 18系列文章终于要提上章程了！)



---

## React

[**Statements Vs Expressions**](https://www.joshwcomeau.com/javascript/statements-vs-expressions/?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)

Josh Comeau正在准备他关于React的下一个课程。他提议回到JavaScript的基础知识，从而让人们更好地理解JJSX的工作原理，而JJSX只在表达式中起作用。在同一个话题上，我很想看到[do-expressions](https://github.com/tc39/proposal-do-expressions?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)提案的进展😇。

[**How to build connected components in Storybook**](https://storybook.js.org/blog/how-to-build-connected-components-in-storybook/?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)

一篇关于Storybook的官方文章，很好地解释了你可以用装饰器（decorators）做的所有事情：添加布局、全局提供者、模拟Redux商店或请求...... 它可以帮助在你的Storybook中添加 "connected "组件，否则由于上下文的依赖性而无法呈现。

[**How I Estimate NPM Package Market Share (and how Redux usage compares to other libraries)**](https://blog.isquaredsoftware.com/2022/07/npm-package-market-share-estimates/?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)


Mark Erikson（Redux）解释了他如何根据各种或多或少可靠的工具来分析npm包的使用趋势。下载统计数字通常与CI构建有关。他以React状态管理器为例。他现在估计Redux/React的使用率为33%（之前为45-50%）

[**Actionless and Stateless Reducers in React**](https://julesblom.com/writing/actionless-and-stateless-reducers?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)

useReducer()并不是为复杂的情况保留的：它也可以用于非常简单的状态机，比如把一个布尔值从假变成真。

**拓展阅读**

-   📜 [Next.js: open external links in a New Tab](https://www.seancdavis.com/posts/open-external-nextlink-links-in-a-new-tab/?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter): it can be interesting to create your own Link abstraction on top of the underlying framework to add extra behavior
-   📜 [The Unlocked Possibilities of the :has() Selector](https://blog.jim-nielsen.com/2022/unlocked-possibilities-of-has-selector/?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter): CSS feature. Interesting comparison with React rendering at the end.
-   📜 [Atomic Forms in React](https://reaper.is/writing/20220709-atomic-forms?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter): presents a bit Jotai-Form and the difference with more traditional approaches like Formik.
-   📜 [Create a simple cookie with Remix](https://jonmeyers.io/blog/create-a-simple-cookie-with-remix?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter): shows that the use of cookie in Remix is relatively simple, and close to the HTTP protocol
-   📜 [Yelp - Migrating from Styleguidist to Storybook](https://engineeringblog.yelp.com/2022/07/migrating-from-styleguidist-to-storybook.html?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)
-   📜 [Fresh: The Next-Gen JavaScript Web Framework](https://hxrsh.in/blog/fresh?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)
-   📜 [Rendering long lists using virtualization with React](https://wanago.io/2022/06/27/long-lists-react-virtualization/?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)
-   📜 [Component Code Coverage in Cypress v10](https://glebbahmutov.com/blog/component-code-coverage/?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)
-   🧑‍🎨 [Remix + Bun demo](https://twitter.com/ebey_jacob/status/1544608334736592896?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)
-   🧑‍🎨 [React-on-the-edge](https://github.com/vercel-labs/react-on-the-edge?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter): Vercel demo that shows how to use React SSR (without Next.js) with the Edge Runtime. With or without streaming.
-   🐦 [Remix loader type inference](https://twitter.com/kentcdodds/status/1545048020663750661?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter): PR merged to facilitate typesafe usage of the useLoaderData() hook 👌
-   🐦 [Bun + React SSR](https://twitter.com/jarredsumner/status/1544580094328418304?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter): significant performance gains
-   📦 [RemixBlocks](https://javascript.plainenglish.io/remixblocks-ready-to-use-remix-tailwind-css-routes-and-ui-blocks-470a6db70915?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter): I find the idea interesting: nested routes Remix are full-stack which makes them a good candidate for copy/paste, quite similar to Tailwind.
-   📦 [react-obsidian](https://github.com/wix-incubator/react-obsidian?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter): dependency injection for React
-   📦 [remix-bossa-nova-stack](https://github.com/clerkinc/remix-bossa-nova-stack?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)
-   📦 [Preact 10.9](https://github.com/preactjs/preact/releases/tag/10.9.0?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)
-   📦 [Next.js 12.2.1](https://github.com/vercel/next.js/releases/tag/v12.2.1?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)
-   📣 [Vercel: Hydrogen can now be deployed with 0 config](https://vercel.com/changelog/hydrogen-projects-can-now-be-deployed-with-zero-configuration?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)


## React-Native

-   📜 [Expo: sunsetting the CLI Web UI](https://blog.expo.dev/sunsetting-the-web-ui-for-expo-cli-ab12936d2206?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter): the CLI web UI will disappear. Not a big deal, it was limited anyway compared to the CLI features.
-   🧑‍🎨 [useAnimatedSentor travel cards parallax](https://twitter.com/lima_lucas3/status/1545956814650499072?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter): demo with a very nice visual result 😎
-   📦 [react-native-keyboard-controller 1.0](https://github.com/kirillzyusko/react-native-keyboard-controller?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter): synchronizes keyboard visibility with animated values 👌
-   📦 [vision-camera-plugin-builder](https://twitter.com/mrousavy/status/1544982270997852160?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter): reduces the boilerplate for the creation of a vision camera plugin.
-   📦 [React-Native MacOS 0.68](https://twitter.com/ReactNativeMSFT/status/1545289039187611650?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)
-   🎥 [It's After Effects, but in Remotion](https://www.youtube.com/watch?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter&v=-7MOoWN2_nk): William Candillon shows how React-Native-Skia runs on the web with Remotion. You can follow and apply the After Effect tutorials, not written for us at first.
-   📊 [FlatList vs FlashList profiling](https://twitter.com/almouro/status/1544669919479996416?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)
-   🐦 [Reanimated now supports V8](https://twitter.com/swmansion/status/1546872761045229568?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)
-   🐦 [Expo EAS + App Store Connect v2](https://twitter.com/Baconbrix/status/1546760343405330434?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)
-   🐦 [BottomSheet + FlashList integration](https://twitter.com/gorhom/status/1546256656639614977?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)

---

## Other

-   [Agenda for the 91st meeting of Ecma TC39](https://github.com/tc39/agendas/blob/main/2022/07.md?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)
-   [New Node.js security releases](https://nodejs.org/en/blog/vulnerability/july-2022-security-releases/?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)
-   [Simplify your full-stack applications with XState](https://blog.theodo.com/2022/07/simplify-your-applications-with-xstate/?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)
-   [The many faces of themeable design systems](https://bradfrost.com/blog/post/the-many-faces-of-themeable-design-systems/?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)
-   [Avoiding <img> layout shifts: aspect-ratio vs width & height attributes](https://jakearchibald.com/2022/img-aspect-ratio/?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)
-   [Fireship + Bun: JavaScript just got way faster](https://www.youtube.com/watch?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter&v=FMhScnY0dME)
-   [Bao.js: A fast, minimalist web framework for the Bun JavaScript runtime.](https://github.com/mattreid1/baojs?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)
-   [The Future of CSS: Variable Units, powered by Custom Properties](https://www.bram.us/2022/07/08/the-future-of-css-variable-units-powered-by-custom-properties/?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)
-   [Parcel CSS 1.11](https://twitter.com/devongovett/status/1545142100483719168?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)
-   [Announcing support for WASI on Cloudflare Workers](https://blog.cloudflare.com/announcing-wasi-on-workers/?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)
-   [Why Your Cached JavaScript Is Still Slow and Incurs Performance Overhead](https://www.webperf.tips/tip/cached-js-misconceptions/?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)

<img width="682" alt="CleanShot 2022-07-13 at 10 40 41@2x" src="https://user-images.githubusercontent.com/749374/178690238-2de46b69-5b32-4037-97d1-5a1c7bd23f97.png">

  订阅原文:
-   🇬🇧 [ThisWeekInReact.com](https://thisweekinreact.com/)
-   🇫🇷 [ReactHebdo.fr](https://reacthebdo.fr/)

 
