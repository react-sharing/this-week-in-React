This Week In React #99: Remix, Next.js, Redux, Memoization, Storybook, Ladle, Wix, Shopify, React-Native, CodeSandbox, Prettier, Deno...


## React


[**Ladle - A drop-in alternative to Storybook**](https://www.ladle.dev/blog/introducing-ladle/?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)

Ladle是一个来自Uber的工程师的项目，他喜欢Storybook，但在他的公司里仍然看到各种性能问题：构建时间、启动时间、交互时间......。因此，他创建了一个更快的替代方案，基于Vite和ES模块，并与[Component Story Format](https://storybook.js.org/docs/react/api/csf?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)兼容，使采用更容易([demo](https://baseweb.netlify.app/?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter))。

[**Preemptive Memoization In React Is Probably Not Evil**](https://www.zhenghao.io/posts/memo-or-not?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)

一篇关于对象和回调的稳定性的文章，非常有趣，而且有据可查。尽管使用`useMemo`看起来是一种过早的优化，但Zhenghao建议尽可能地稳定身份，至少对于lib和自定义钩子是这样。我们期待着 [React-Forget](https://www.youtube.com/watch?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter&v=lGEMwh32soc)和[Records & Tuples](https://sebastienlorber.com/records-and-tuples-for-react?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)的出现，它们可以大大简化我们的生活。

[**Remix Stacks**](https://remix.run/blog/remix-stacks?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)** & **[**Remix v1.3**](https://github.com/remix-run/remix/releases/tag/v1.3.0?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)

Remix CLI现在允许你用一个给定的堆栈初始化一个项目。Remix提供了3个内置栈，可以快速启动（DB、Auth、host、test...），也可以创建自己的栈（例如公司项目）。在这3个可用的堆栈中，差异主要是在主机或持久性方面，我们发现了一些共同的基础：Tailwind, TypeScript, Prettier, ESLint, Cypress, MSW, Docker, Vitest, Testing Library。

我觉得提供启动器以快速入门是件好事，但我对 "模板 "的做法褒贬不一，我更喜欢Kent之前倡导的 ["company-scripts"](https://kentcdodds.com/blog/tools-without-config?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)的做法（如CRA），以减少现有项目的长期维护。

[**Upgrading Next.js for instant performance improvements**](https://vercel.com/blog/upgrading-nextjs-for-instant-performance-improvements?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)

Vercel最近将一个演示应用程序（[Virtual Reality Store](https://serverless-vrs.vercel.app/?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)）从Next.js v8升级到v12。Lydia借此机会列举了最新版本的许多改进，你只需付出最小的升级努力就能得到这些改进。对你可能错过的新功能做了一个很好的概述。

[**How Wix Applied Multi-threading to Node.js and Cut Thousands of SSR Pods and Money**](https://openjsf.org/blog/2022/03/17/openjs-in-action-how-wix-applied-multi-threading-to-node-js/?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)

来自Wix的反馈，解释了他们如何优化运行React服务器端渲染的平台，以满足高CPU需求。他们使用了新的Node.js API 14 [worker_threads](https://nodejs.org/api/worker_threads.html?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)（与 [child_process](https://nodejs.org/api/child_process.html?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)不同，允许内存共享），得到了非常好的结果。这篇文章更多的是关于Node.js的，但对于那些运行自我托管的React SSR管道的人来说，仍然觉得很有意义。

[**Shopify: Creating a React Library for Consistent Data Visualization**](https://shopify.engineering/react-library-consistent-data-visualization?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)

来自Shopify的反馈，报告其数据可视化的一致性问题。解决方案：创建Polaris Viz库，该库将很快开源。他们特别解释了使用React上下文来创建默认主题，以及通过部分覆盖来创建变体的可能性。

[**Idiomatic Redux: Designing the Redux Toolkit Listener Middleware**](https://blog.isquaredsoftware.com/2022/03/designing-rtk-listener-middleware/?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)

Mark Erikson对新的Redux Toolkit 1.8 [Listener Middleware](https://redux-toolkit.js.org/api/createListenerMiddleware?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter) API的设计进行了回顾，该设计跨越了2年多的时间，进行了多次迭代。他们设法用一个相对简单的API覆盖了许多Redux-Saga/Observable的用例。我喜欢`await condition(predicate)` 的概念。

### **拓展阅读**

-   📜 [Nexus --- a Component Tree Visualizer for Next.js](https://levelup.gitconnected.com/introducing-nexus-a-component-tree-visualizer-for-next-js-1109f31e118e?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter): extension VSCode
-   📜 [Using SVG sprites in a React app](https://dev.to/mbarzeev/using-svg-sprites-in-a-react-app-477d?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)
-   📜 [Implementing advanced usePrevious hook with React useRef](https://www.developerway.com/posts/implementing-advanced-use-previous-hook?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)
-   📜 [Remix - Full Context Review](https://www.fullcontextdevelopment.com/blog/remix-full-context-review?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)
-   📜 [Remix vs Next.js](https://bejamas.io/blog/remix-vs-nextjs/?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)
-   📜 [Storybook Community Showcase #1](https://storybook.js.org/blog/community-showcase-1/?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)
-   📖 [Partydown + Gatsby](https://partytown.builder.io/gatsby?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter): integration doc
-   📖 Dan Abramov [annonced 3 new doc pages](https://twitter.com/dan_abramov/status/1504503103109926919?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter) on the beta site: [useReducer](https://beta.reactjs.org/apis/usereducer?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter), [useContext](https://beta.reactjs.org/apis/usecontext?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter), [createContext](https://beta.reactjs.org/apis/createcontext?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)
-   📦 [React-Runner v1](https://twitter.com/_neonie/status/1505880831092482052?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter): 这个现代的React-Live替代品的稳定发布，允许创建一个具有实时预览功能的代码编辑器。与CodeSandbox [Sandpack](https://codesandbox.io/post/sandpack-announcement?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)类似，但没有任何iframe，直接在浏览器中运行。
-   📦 [React-Spline](https://github.com/splinetool/react-spline?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter): 来运行用[Spline](https://spline.design/?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)工具创建的3D体验。不是100%确定这是什么，但它看起来像是Blender + React-Three-Fiber的一个可能的替代方案？
-   📦 [Remix-ETag](https://github.com/donavon/remix-etag?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)
-   📦 [MDX v2.1](https://github.com/mdx-js/mdx/releases/tag/2.1.0?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)

## React-Native

-   📦 [React-Native v0.68.0-rc.3](https://twitter.com/reactnative/status/1506327122771513345?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter):计划在下周推出稳定的0.68版，包括启用Fabric和新架构的开关🤯。
-   📜 [Using Storybook and MSW in React Native](https://phelipetls.github.io/posts/using-storybook-and-msw-in-react-native/?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)
-   🧑‍🎨 React-Native-Skia: [shadows](https://twitter.com/wcandillon/status/1505907265072738307?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)
-   🎙️ [RNR 229 - Building an Expo App for Mobile and Web with Josh Justice](https://reactnativeradio.com/episodes/rnr-229-building-an-expo-app-for-mobile-and-web-with-josh-justice?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)
-   😢 [React-Native Weekly - The End](https://andrei-calazans.com/posts/2022-03-22/react-native-weekly?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)
-   📦 [React-Native-Quick-SQLite](https://twitter.com/ospfranco/status/1504389581264896004?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter): async callbacks support
-   📦 [React-Native-Elements v4.0.0-rc.0](https://github.com/react-native-elements/react-native-elements/releases/tag/v4.0.0-rc.0?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)

## Other

[**CodeSandbox Projects**](https://codesandbox.io/post/announcing-codesandbox-projects?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)

CodeSandbox重写，为任何规模的项目提供新的云开发体验，与IDE集成（现在是VSCode，将来会有更多），甚至支持iPad。不错的贡献工作流程，对于快速合作或代码评审似乎很方便，而无需切换你的本地git分支。

### **拓展阅读**

-   [Prettier 2.6](https://prettier.io/blog/2022/03/16/2.6.0.html?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter): new `singleAttributePerLine` option, TS 4.6 support...
-   [Deno 1.20](https://deno.com/blog/v1.20?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter): significant perf improvements, TS 4.6 support, V8 upgrade...
-   [welcome2web3.com](https://welcome2web3.com/?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter): ironic site, demo the web3 UX 😂
-   [Lamina](https://twitter.com/0xca0a/status/1504140883167703044?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter): *"Tailwind for shaders"*
-   [Vercel Deploy](https://chrome.google.com/webstore/detail/vercel-deploy/nkignhibadhmcbiiilleogljodcaonjk?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter): Chrome Extension
-   [Boa v0.14](https://boa-dev.github.io/posts/2022-03-15-boa-release-14/?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)
-   [Parcel CSS v1.7](https://twitter.com/devongovett/status/1505327865553997824?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)
-   [Wave.js 2.0](https://github.com/foobar404/Wave.js?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)
-   [Your SSR is slow & your devtools are lying to you](https://dev.to/mlrawlings/your-ssr-is-slow-your-devtools-are-lying-to-you-3056?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)
-   [Debugging TypeScript using Replay Node](https://medium.com/replay-io/debugging-typescript-using-replay-node-646087b6712?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)
-   [OpenSSL security releases require Node.js security releases](https://nodejs.org/en/blog/vulnerability/mar-2022-security-releases/?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)
-   [Conquering JavaScript Hydration](https://dev.to/ryansolid/conquering-javascript-hydration-a9f?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)
-   [experiences. Web. frameworks. future. me.](https://igor.dev/posts/experiences-web-frameworks-future-me/?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)
-   [Motion Developer Tools](https://twitter.com/mattgperry/status/1505918782685921282?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)
-   [How to write fast code](https://twitter.com/devongovett/status/1504476131818237967?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)
-   [Vitest inline assertions](https://twitter.com/antfu7/status/1505299814069977088?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)? 🤔
-   [hidden="until-found"](https://twitter.com/cramforce/status/1504539803336929282?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)
-   [Alert: peacenotwar module sabotages npm developers in the node-ipc package to protest the invasion of Ukraine](https://snyk.io/blog/peacenotwar-malicious-npm-node-ipc-package-vulnerability/?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)
-   [Protestware is trending in open source: 4 different types and their impact](https://snyk.io/blog/protestware-open-source-types-impact/?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)
-   [Packages with high download numbers that nobody wanted to install](https://www.stefanjudis.com/notes/packages-with-high-download-numbers-that-nobody-wanted-to-install/?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)
-   [CSS-Tricks is joining DigitalOcean!](https://css-tricks.com/css-tricks-is-joining-digitalocean/?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)
-   [In Defense of Sass](https://thinkdobecreate.com/articles/in-defense-of-sass/?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)
-   [Gotchas with Git and the GitHub API](https://retool.com/blog/gotchas-git-github-api/?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)
-   [Retro-specifying fetch/performance](https://blog.whatwg.org/retro-specifying-fetch-performance?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)
-   [Making WebViews work for the Web](https://www.w3.org/blog/2022/03/making-webviews-work-for-the-web/?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)
-   [Why I Prefer Makefiles Over package.json Scripts](https://spin.atomicobject.com/2021/03/22/makefiles-vs-package-json-scripts/?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)

![image](https://user-images.githubusercontent.com/749374/159665898-2cf1c82b-55c8-4a74-8fd4-ebdc53f5db82.png)
 
