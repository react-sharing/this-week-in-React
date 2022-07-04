
## React

[**Lexical**](https://lexical.dev/?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)

Meta新开源库，用于创建可扩展的文本编辑器（有一个支持提及、哈希标签、协作编辑的插件系统...）。它似乎是[Draft.js的一个现代、轻量级的替代品](https://news.ycombinator.com/item?id=31022152&utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)（这次不需要使用ImmutableJS了😏）。不特别依赖React，但提供了一个官方绑定。可以被其他框架使用，甚至可以针对 [其他平台](https://news.ycombinator.com/item?id=31023832&utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter) ([计划支持iOS](https://twitter.com/trueadm/status/1514680423133196295?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter))。

[**A Quick Guide to Mitosis**](https://www.builder.io/blog/mitosis-a-quick-guide?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)

Mitosis是一个工具，它允许你用接近React/JSX的语法来创建一个设计系统（受Solid启发）。Mitosis能够将这些组件编译成各种框架（React、Angular、Svelte、React-Native...）。这对于长期使用多个框架的大公司来说是很方便的。这篇官方文章是一个很好的介绍。

[**Multiple forms per route in Remix**](https://sergiodxa.com/articles/multiple-forms-per-route-in-remix?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter#multiple-forms-per-route-in-remix)

解释了如何管理与同一Remix路由相关的两个表单。每个路由只能有一个`ActionFunction`，所以最好的解决办法似乎是在提交按钮上使用`action`属性。

[**Accessible React Forms**](https://www.carlrippon.com/accessible-react-forms/?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)

对React背景下的一些无障碍原则进行了很好的概述：描述`aria-*`属性及其对屏幕阅读器的影响，颜色，焦点...

[**Storybook Lazy Compilation for Webpack**](https://storybook.js.org/blog/storybook-lazy-compilation-for-webpack/?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)

在即将到来的storybook 6.5版本中，通过懒加载提升了本地dx加载的性能：启动速度提高3倍，再次构建速度提高2倍。对于较大的故事书来说，其影响似乎很显著。与[Ladle](https://www.ladle.dev/blog/introducing-ladle?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)比较，它是最近发布的Storybook的替代品，也试图提高性能。

**拓展阅读**

-   📜 [Static Full-Text Search in Next.js with WebAssembly, Rust, and Xor Filters](https://hackernoon.com/static-full-text-search-in-nextjs-with-webassembly-rust-and-xor-filters-tldr?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter): a part dedicated to integrating WebAssembly with Next.js (Webpack config). 的一部分，专门用于将WebAssembly与Next.js（Webpack配置）整合。
-   📜 [Introducing React-admin V4](https://marmelab.com/blog/2022/04/13/react-admin-v4.html?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter): already presented [last week](https://www.getrevue.co/profile/thisweekinreact/issues/this-week-in-react-101-astro-redwood-next-js-remix-react-admin-rust-reducers-webcomponents-gatsby-typescript-rome-1121624?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter), now v4 is officially released.
-   📜 [Why you should always Cleanup Side Effects in React useEffect and How to Cleanup](https://dillionmegida.com/p/why-you-should-cleanup-when-component-unmounts/?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)
-   📜 [The Duality of CLS with Lazy Loading Components](https://wicki.io/posts/2022-03-cls-with-lazy-loading-components/?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)
-   📜 [Migrating your React app from Webpack to Vite](https://dev.to/wojtekmaj/migrating-your-react-app-from-webpack-to-vite-inp?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)
-   📜 [React Higher-Order Components (HOCs)](https://www.robinwieruch.de/react-higher-order-components/?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)
-   📜 [What's New in React 18](https://blog.appsignal.com/2022/04/13/whats-new-in-react-18.html?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)
-   📖 [Why Redux Toolkit is How To Use Redux Today](https://redux.js.org/introduction/why-rtk-is-redux-today?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter): new doc nudging you to adopt Redux Toolkit.
-   🐦 React-Router v6.x: [preview 1](https://twitter.com/ryanflorence/status/1513957268898738179?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter), [preview 2](https://twitter.com/ryanflorence/status/1513968694291939328?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)
-   🐦 [Remotion: StackBlitz support](https://twitter.com/remotion_dev/status/1515273796726497289?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)
-   🐦 [Module Federation Support for Next.js](https://twitter.com/ScriptedAlchemy/status/1514793313278128131?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)
-   🐦 [Lighthouse + Next.js guidance](https://twitter.com/hdjirdeh/status/1514440320192110597?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)
-   📦 [Next-Markdown](https://github.com/frouo/next-markdown?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter): new lib to integrate Markdown content in Next.js. Supports MDX, Table of Contents, index...
-   📦 [Redux 4.2](https://github.com/reduxjs/redux/releases/tag/v4.2.0?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter): `createStore` deprecated with a warning
-   📦 [React-Redux v8](https://twitter.com/acemarke/status/1515383796237012998?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter): compat React 18, codebase in TypeScript.
-   📦 [Generouted](https://github.com/oedotme/generouted?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter): file-based routing, integration between React-Location and Vite. Modern features to compete with meta-frameworks: supports code-splitting, data loaders, nested layouts...
-   📦 [Zustand v4.0.0-rc.0](https://twitter.com/dai_shi/status/1515880958838571016?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter): JS backward compatible. Breaking changes TS.
-   📦 [Proxy-Memoize 1.0](https://twitter.com/dai_shi/status/1514216846232530944?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter): interesting alternative to Reselect to create memoized selectors, but can be used for other cases as well.
-   📦 [Create-React-App v5.0.1](https://twitter.com/iansu/status/1513935894859841536?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter): improves React 18 compat
-   📦 [React-Hooks-Testing-Library v8.0](https://github.com/testing-library/react-hooks-testing-library/releases/tag/v8.0.0?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)
-   🎥 [Ryan Carniato - A First Look at Next.js](https://www.youtube.com/watch?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter&v=m-Gl_Cc8xOg)
-   💸 [Intellij 2022.1](https://www.jetbrains.com/idea/whatsnew/?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter): improves IDE Next.js support
-   💸 [Official React-Query Course](https://twitter.com/tannerlinsley/status/1514987976773701632?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)

## React-Native

-   📜 [Create high-performance graphics with React Native Skia](https://blog.logrocket.com/create-high-performance-graphics-react-native-skia/?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)
-   🐦 React-Native-Skia: [drop-in React-Native-Svg replacement](https://twitter.com/wcandillon/status/1515731236861493258?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)?
-   💡 [PR: Add TypeScript support in New Architecture/Codegen](https://github.com/facebook/react-native-website/pull/3036?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter): it is possible to write [TurboModule spec](https://reactnative.dev/docs/next/new-architecture-library-intro?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter#turbomodules) in TypeScript (to describe your native module API)
-   📦 [React-Native-Turbo-Starter](https://github.com/talknagish/react-native-turbo-starter?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter): a boilerplate to create modern React-Native modules leveraging the new architecture.
-   📦 [React Native Turbo Secure Storage](https://github.com/ospfranco/turbo-secure-storage?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)
-   📦 [expo-github-action/command](https://github.com/expo/expo-github-action/tree/main/command?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter): can trigger an EAS build with a GitHub comment (experimental)
-   👥 [React-Native devs Twitter community](https://twitter.com/jamonholmgren/status/1515453608434708484?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)
-   🎥 [Creating a RN Turbo Secure Storage module from scratch](https://www.youtube.com/watch?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter&v=U0shm20ClkU)
-   🎥 [React Native Turbomodule + TypeScript Codegen Tutorial](https://www.youtube.com/watch?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter&v=c_AQSztIS6Y)


## 其它

[**CSS Parent Selector**](https://ishadeed.com/article/css-has-parent-selector/?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)

CSS有一个新的`:has()`选择器，通常被称为 "父选择器"，它允许根据子元素将CSS规则应用于父元素。例如，你可以改变一个卡片的父级布局，但只有当它包含一个图像元素时才生效：这就避免了必须在父级上应用一个变量来控制。这篇文章用许多使用案例说明了这个新功能。我发现根据`<select>`值在 `<html>` 上应用CSS变量的可能性很有趣（对于主题化或[黑暗模式支持](https://twitter.com/tomayac/status/1515376550048419848?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter))的[有用Demo](https://twitter.com/shadeed9/status/1514875999418208263?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)）。目前只在Safari和Chrome Canary中可用，但支持度可以快速提高。

注意不要滥用它：在React这样的组件模型中，最好将自己限制在针对本地类，以避免破坏组件的封装模型。

[**New 103 HTTP Status Code (Early Hints)**](https://twitter.com/sebastienlorber/status/1516087831134879747?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)

在HTML规范中正式加入了一个新的状态代码。它允许向浏览器发送 "early hints（早期提示）"，以便在收到服务器的200响应之前预取/预装资源。这对于CDN（阅读[Cloudflare的文章](https://blog.cloudflare.com/early-hints/?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)）似乎很有用，它能够在从源服务器获取新的同时，发送缓存的早期提示（甚至通过机器学习🤯预测）。

[**Building a dialog component**](https://web.dev/building-a-dialog-component/?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)

随着`<dialog>`在Safari 15.4中的加入和[越来越多的支持](https://caniuse.com/dialog?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)，是时候来看看这个新元素了。Adam Argyle为我们提供了一篇关于这个主题的相当完整的文章：基于最现代的网络API，他实现了一个具有动画、可访问性、响应性、轻型驳回、自定义事件的巨型/迷你模态。


**拓展阅读**

-   [Node.js 18](https://nodejs.org/en/blog/announcements/v18-release-announce/?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter): freshly released! With experimental support for `fetch()`, Web Streams, a test runner...
-   [navigation-api](https://github.com/WICG/navigation-api?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter): [intent to ship Blink/Chromium](https://twitter.com/intenttoship/status/1513914320056459274?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)
-   [The Front-End Developer's Guide to the Terminal](https://www.joshwcomeau.com/javascript/terminal-for-js-devs/?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)
-   [Innovating beyond libraries and frameworks](https://nilsnh.no/2022/04/09/innovating-beyond-libraries-and-frameworks/?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)
-   [Declarative design](https://adactio.com/journal/18982?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)
-   [WebAssembly 2.0 First Public Working Drafts](https://www.w3.org/blog/news/archives/9509?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)
-   [NodeJS packages don't deserve your trust](https://josephg.com/blog/node-sandbox/?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)
-   [Announcing Fastify v4 release candidate!](https://medium.com/@fastifyjs/announcing-fastify-v4-release-candidate-2b6be6edf196?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)
-   [Shopify/Javy: JS to WebAssembly toolchain](https://github.com/Shopify/javy?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)
-   [Deno Cheat Sheet](https://oscarotero.com/deno/?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)
-   [Netlify Edge Functions on Deno Deploy](https://deno.com/blog/netlify-edge-functions-on-deno-deploy?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)
-   [Will Tauri Be an Electron Killer?](https://betterprogramming.pub/will-tauri-be-an-electron-killer-38fd6478004?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)
-   [How Jotai Specifies Package Entry Points](https://blog.axlight.com/posts/how-jotai-specifies-package-entry-points/?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)
-   [The Ultimate Guide to Optimizing JavaScript for Quick Page Loads](https://www.builder.io/blog/the-ultimate-guide-to-optimizing-javascript-for-quick-page-loads?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)
-   [Exploring the new CSS color functions: CSS Color Module Level 5](https://blog.logrocket.com/exploring-css-color-module-level-5/?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)
-   [The Definitive Guide to Image Optimization](https://www.builder.io/blog/the-definitive-guide-to-image-optimization?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)
-   [JavaScript Function Composition: What's The Big Deal?](https://jrsinclair.com/articles/2022/javascript-function-composition-whats-the-big-deal/?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)
-   [Node.js 18 Introduces Prefix-Only Core Modules](https://fusebit.io/blog/node-18-prefix-only-modules/?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)
-   [Dependabot alerts now surface if your code is calling a vulnerability](https://github.blog/2022-04-14-dependabot-alerts-now-surface-if-code-is-calling-vulnerability/?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)
-   [Git security vulnerability announced](https://github.blog/2022-04-12-git-security-vulnerability-announced/?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)
-   [GitHub Discussions: Organization Discussions, polls, and more](https://github.blog/2022-04-12-whats-new-in-github-discussions-organization-discussions-polls-and-more/?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)
-   [Why is Builder.io creating Qwik and Partytown?](https://www.builder.io/blog/why-is-builderio-creating-qwik-and-partytown?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)
-   [Angular Developer Survey 2021 Results](https://blog.angular.io/developer-survey-2021-results-38e653cbb36b?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)
-   [DuckDuckGo for Mac: A Private, Fast, and Secure Browsing App](https://spreadprivacy.com/introducing-duckduckgo-for-mac/?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)
-   [HTTPie: how we lost 54k GitHub star](https://httpie.io/blog/stardust?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)

  
  <img width="524" alt="CleanShot 2022-04-20 at 09 39 20@2x" src="https://user-images.githubusercontent.com/749374/164176177-8d55866a-db39-4098-b25c-f9c24f97bd86.png">
  
  ---
  
  订阅原文:
-   🇬🇧 [ThisWeekInReact.com](https://thisweekinreact.com/)
-   🇫🇷 [ReactHebdo.fr](https://reacthebdo.fr/)
