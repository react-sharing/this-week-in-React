This Week In React #101: Astro, Redwood, Next.js, Remix, React-Admin, Rust reducers, WebComponents, Gatsby, TypeScript, Rome...

订阅原文:
-   🇬🇧 [ThisWeekInReact.com](https://thisweekinreact.com/)
-   🇫🇷 [ReactHebdo.fr](https://reacthebdo.fr/)

---

## React

[**Astro Server-Side Rendering**](https://astro.build/blog/experimental-server-side-rendering/?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)

Astro是一个现代元框架，能够使用任何UI库（包括React）。它现在支持服务器端渲染，在[v1.0 beta](https://astro.build/blog/astro-1-beta-release/?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)测试版中可以实验。与Remix一样，该框架提供了一个 [adapters](https://github.com/withastro/astro/tree/main/packages/integrations?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)层，用于部署到多个目标。

[**React-admin V4: Build Your Own Framework**](https://marmelab.com/blog/2022/04/11/react-admin-v4-build-your-own-framework.html?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)

François以React中一个简单的管理界面为例，该界面基于MUI和React-Hook-Form。这段代码最初是相当冗长的，有90行。他通过抽象和复用，重构了这段代码，最终实现相同的效果只用了20行代码。

他解释说，这些抽象实际上是React-Admin的第四版（[v4.0.0-RC.1](https://github.com/marmelab/react-admin/releases/tag/v4.0.0-rc.1?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)）。这个新版本基于更现代的堆栈，并且更加模块化：它暴露了高级组件（默认基于MUI，可以交换），但也有低层单元来创建你自己的框架。[v4的全部系列文章](https://marmelab.com/en/blog/?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter#react-admin)。

[**An Overlooked Factor For Performance Optimization In React**](https://www.zhenghao.io/posts/top-level-perf?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)

Interesting reflection on the need (or not) to memoize the value of a React context according to the position of the provider in the tree. Personally, I still prefer to always memoize for safety, as you never know if the provider will not be moved somewhere else.

关于是否需要（或不需要）根据provider在树中的位置来记忆React上下文的值的有趣的思考。就个人而言，为了安全起见，我还是倾向于总是记忆化，因为你永远不知道提供者是否会被移到其他地方。

[**Writing Redux Reducers in Rust**](https://fiberplane.dev/blog/writing-redux-reducers-in-rust/?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)

通过WebAssembly将现有的Rust业务代码整合到React应用中，以及遇到的挑战：非理想的绑定，序列化WASM桥梁等场景的反馈。他们需要在两边（Rust和TypeScript）访问相同的状态。解决方案：在Rust中创建还原器，并向TypeScript返回一个状态差异。

[**How to Create and Export Web Components From a React Application**](https://spin.atomicobject.com/2022/04/11/export-web-components/?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)

展示了如何使用React来创建一个Web组件。它看起来比较简单，在一些特定的情况下🤔可能会很有用。不要与React的Web Components的使用相混淆（[以后将正式支持](https://twitter.com/reactjs/status/1508899112074231810?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)）。

[**React components composition: how to get it right**](https://www.developerway.com/posts/components-composition-how-to-get-it-right?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)

Gives some hints on when/how to split into smaller subcomponents. Also evokes an important Clean Code principle (without naming it): [Single Level of Abstraction](https://medium.com/trabe/coding-react-components-single-level-of-abstraction-e60f25676235?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter).

对何时/如何分割成更小的子组件给出了一些建议。也唤起了一个重要的清洁代码原则（没有命名它）。[单一层次的抽象](https://medium.com/trabe/coding-react-components-single-level-of-abstraction-e60f25676235?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)。

**拓展阅读:**

-   🧵 [React 18 + TypeScript](https://twitter.com/reactjs/status/1512453230504124420?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter): typings released with necessary breaking changes. In particular the [TypeScript type for `React.FC` does not include `children` anymore](https://twitter.com/dan_abramov/status/1512833611401150474?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter). Also check [Removal Of Implicit Children](https://solverfox.dev/writing/no-implicit-children/?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter), and this [codemod](https://github.com/eps1lon/types-react-codemod?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter) to migrate.
-   📜 [Test component interactions with Storybook](https://storybook.js.org/blog/test-component-interactions-with-storybook/?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter): complete guide to create and execute interaction tests in Storybook stories thanks to the `play()` function.
-   📜 [How to easily reduce your NextJS bundle size by 30%?](https://www.flavienbonvin.com/reduce-next-js-bundle/?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter) feedback, quantified impact of 4 actions relatively easy to implement. Using dynamic imports provides the best ROI.
-   📜 [React 18 Quick Guide & Core Concepts Explained](https://dev.to/shrutikapoor08/react-18-quick-guide-core-concepts-explained-519p?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter): good React 18 major changes summary.
-   📜 [Redwood Startup Fund](https://tom.preston-werner.com/2022/04/07/the-redwood-startup-fund.html?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter): follow-up of last week's [Redwood 1.0 Launch Week](https://v1launchweek.redwoodjs.com/?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)
-   📜 [Bad Habits of Mid-Level React Developers](https://dev.to/srmagura/bad-habits-of-mid-level-react-developers-b41?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)
-   📜 [Improving Web Performance with React Hydration Strategies](https://medium.com/cdiscount-engineering/improving-web-performance-with-react-hydration-strategies-3117f71a1695?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)
-   💡 [Gatsby RFC: New Bundler in Gatsby](https://github.com/gatsbyjs/gatsby/discussions/35357?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter): may incrementally adopt esbuild according to current benchmarks?
-   💡 [Gatsby RFC: Script component](https://github.com/gatsbyjs/gatsby/discussions/35404?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter): similar component to the Next.js one, with a possible Partytown integration?
-   💡 [Redux deprecate createStore?](https://twitter.com/acemarke/status/1513714595764051972?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)
-   💡 [Remix deferred API?](https://twitter.com/ebey_jacob/status/1512921424972767236?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)
-   🐦 React + TypeScript: [no need to import React event handler types](https://twitter.com/sebastienlorber/status/1512420374201446405?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)
-   🐦 React 18 + `React.lazy()` + Suspense + SSR: [only works with new APIs SSR](https://twitter.com/reactjs/status/1511755578716028928?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter), not `renderToString`.
-   🎥 [RedwoodJS Intro](https://www.youtube.com/watch?t=1s&utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter&v=m_3I9mufZfs) by Tom Preston Werner
-   🎥 [React Jargon Explained: What is Concurrent React?](https://www.youtube.com/watch?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter&v=bZRqmobuJvM)
-   📦 [React-Native-Storybook-Starter](https://twitter.com/Danny_H_W/status/1512985528249028610?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter): with mobile + React-Native-Web support
-   📦 [Capacitor-Remix-Templates](https://github.com/ionic-team/capacitor-remix-templates?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)
-   📦 [Remix + Crystallize eCommerce Starter](https://crystallize.com/blog/remix-run-ecommerce-starter?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)
-   🎙️ [StackOverflow #430: The new version of React](https://stackoverflow.blog/2022/04/05/episode-430-the-new-version-of-react-great-tools-for-learning-css-and-the-double-standard-for-female-engineers/?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)...


## React-Native

-   🐦 [Expo: Evan Bacon automating Android app deployment](https://twitter.com/Baconbrix/status/1511892021321121793?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter): want to go further than Fastlane and allow deploying a new app without any manual step on the Play Store UI (first submission).
-   🐦 React-Native-{Bootsplash,Localize,Permissions}: [looking for sponsors to support Fabric](https://twitter.com/zoontek/status/1512823843206967300?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)
-   📦 [React-Native-Bignumber](https://github.com/margelo/react-native-bignumber?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter): performant Fabric/JSI big number lib
-   📦 [React-Native-Purchase](https://github.com/RevenueCat/react-native-purchases?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter): claims to work with all [Expo workflows](https://docs.revenuecat.com/docs/reactnative?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter#expo-special-instructions)
-   🎙️ [React Native Radio 231 - Using Flipper's Flamegraph Tool](https://reactnativeradio.com/episodes/rnr-231-using-flippers-flamegraph-tool?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)


## 其它

[**Announcing TypeScript 4.7 Beta**](https://devblogs.microsoft.com/typescript/announcing-typescript-4-7-beta/?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)

Another great TypeScript release! The long-awaited ES Modules support and [package.json "exports"](https://devblogs.microsoft.com/typescript/announcing-typescript-4-7-beta/?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter#package-json-exports-imports-and-self-referencing) which allows to create several entry points for the same Node.js package. Many other improvements and new features, including ["moduleSuffixes"](https://devblogs.microsoft.com/typescript/announcing-typescript-4-7-beta/?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter#resolution-customization-with-modulesuffixes) useful for React-Native.

又一个伟大的TypeScript版本! 期待已久的ES模块支持和[package.json "exports"](https://devblogs.microsoft.com/typescript/announcing-typescript-4-7-beta/?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter#package-json-exports-imports-and-self-referencing)，允许为同一个Node.js包创建多个入口点。许多其他改进和新功能，包括对React-Native有用的  ["moduleSuffixes"](https://devblogs.microsoft.com/typescript/announcing-typescript-4-7-beta/?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter#resolution-customization-with-modulesuffixes)。

**拓展阅读:**

-   [Announcing Rome Formatter](https://rome.tools/blog/2022/04/05/rome-formatter-release?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter): broken link in last edition 😅 Rome offers a code formatter written in Rust. Mostly compatible with Prettier, but 9-12x faster, and able to format invalid code!
-   [Node v12.22.12](https://nodejs.org/en/blog/release/v12.22.12/?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter): last v12 LTS
-   [JavaScript Testing Best Practices](https://twitter.com/nodepractices/status/1511633760114069507?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter): updated and translated
-   [Prevent the introduction of known vulnerabilities into your code](https://github.blog/2022-04-06-prevent-introduction-known-vulnerabilities-into-your-code/?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter): new action GitHub to review PR dependency changes and prevent supply-chain attacks. Seems easy to setup.
-   [New to the web platform in March](https://web.dev/web-platform-03-2022/?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter): good overview
-   [Devs For Ukraine](https://www.devsforukraine.io/?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter): conf 25-26 April
-   [TypeScript / How the compiler compiles](https://www.huy.rocks/everyday/04-01-2022-typescript-how-the-compiler-compiles?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)
-   [TypeScript type-level parser](https://twitter.com/anuraghazru/status/1512092136841543682?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)
-   [Make the TypeScript interface partially optional/required](https://pawelgrzybek.com/make-the-typescript-interface-partially-optional-required/?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)
-   [Principles of Object-oriented Programming in TypeScript](https://blog.appsignal.com/2022/04/06/principles-of-object-oriented-programming-in-typescript.html?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)
-   [TypeScript things I wish I knew earlier](https://alvar.dev/blog/typescript-things-i-wish-i-knew-earlier?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)
-   [ECMAScript proposal "Change Array by copy": four new non-destructive Array methods](https://2ality.com/2022/04/change-array-by-copy.html?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)
-   [Safari Technology Preview 143](https://webkit.org/blog/12563/release-notes-for-safari-technology-preview-143/?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)
-   [Safari 15.5 Beta Release Notes](https://developer.apple.com/documentation/safari-release-notes/safari-15_5-release-notes?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)
-   [The "inert" attribute is finally coming to the web](https://www.stefanjudis.com/blog/the-inert-attribute-is-finally-coming-to-the-web/?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)
-   [CSS :has( ) A Parent Selector Now](https://matthiasott.com/notes/css-has-a-parent-selector-now?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)
-   [ShadowRealms -- an ECMAScript proposal for a better `eval`](https://2ality.com/2022/04/shadow-realms.html?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)
-   [What's new in ECMAScript 2022](https://pawelgrzybek.com/whats-new-in-ecmascript-2022/?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)
-   [AST Explorer SWC support](https://twitter.com/jantimon/status/1513451535916838914?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)
-   [How Tailwind CSS came to be feat](https://www.youtube.com/watch?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter&v=1x7HlvSfW6s)
-   [Nx 13.10](https://twitter.com/NxDevTools/status/1512430082349957126?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter) + [Nx 15 Roadmap](https://github.com/nrwl/nx/discussions/9716?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)
-   [Turborepo 1.2](https://twitter.com/turborepo/status/1512454415931879424?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)
-   [Parcel CSS 1.8](https://twitter.com/devongovett/status/1512102628024532996?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)
-   [ESLint v8.13](https://eslint.org/blog/2022/04/eslint-v8.13.0-released?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)
-   [StackBlitz $7.9M Seed Round](https://blog.stackblitz.com/posts/seed-funding/?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)
-   [Prisma Adds Support for MongoDB](https://www.prisma.io/blog/mongodb-general-availability-pixnun6mffmu?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)
-   [4 ways we use GitHub Actions to build GitHub](https://github.blog/2022-04-05-4-ways-we-use-github-actions-to-build-github/?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)
-   [The Next Google](https://dkb.io/post/the-next-google?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)
-   [With 3 months left before IE retirement, new enhancements arrive in Microsoft Edge for IE mode](https://blogs.windows.com/windowsexperience/2022/03/29/with-3-months-left-before-ie-retirement-new-enhancements-arrive-in-microsoft-edge-for-ie-mode/?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)

 <img width="683" alt="CleanShot 2022-04-13 at 10 24 54@2x" src="https://user-images.githubusercontent.com/749374/163133351-b2b94270-79c5-4a9b-9178-255c97db1ed7.png">
