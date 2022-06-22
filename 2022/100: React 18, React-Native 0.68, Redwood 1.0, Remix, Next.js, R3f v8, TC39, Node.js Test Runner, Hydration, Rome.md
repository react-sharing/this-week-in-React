This Week In React #100: React 18, React-Native 0.68, Redwood 1.0, Remix, Next.js, R3f v8, TC39, Node.js Test Runner, Hydration, Rome...

## 概览
- react 18 终于发布了，一些新特性方法值得学习和关注！（推荐）
- Remix和React-Router仓库将合并为Remix。
- React-Native 0.68版本发布，可以手动开启新的Fabric和TurboModules架构
- TC 39会议更新：Decorators、Type annotations等

## React

[**React v18.0**](https://reactjs.org/blog/2022/03/29/react-v18.html?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)

React 18新鲜出炉! 这个新版本提供了许多改进和API，相信很多人已经有所了解: automatic batching, SSR streaming, Suspense, selective hydration, new hooks (`useId`, `useDeferredValue`, `useTransition`...)

这个备受期待的版本也包括**Concurrent React**。新版本中不再是同步和原子渲染：它可以被中断、暂停和恢复。这允许将工作分割成不同优先级的小切片并且可以保持ui的持续响应。

这些并发功能目前可以使用，但主要是为了封装在一个库或一个框架内（计划在[Remix](https://twitter.com/mjackson/status/1508848619700600837?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter), [Next.js](https://twitter.com/timneutkens/status/1508846833304543233?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)中进行整合）

这个新的渲染器可以产生破坏性，只有在使用React 18的新并发功能时才会激活，这可以让我们顺利地增量采用。因此，将React升级到v18应该不会太复杂。如果你的应用程序在开发中出现问题， [建议禁用StrictMode](https://twitter.com/reactjs/status/1509729057541341184?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter).

React 18奠定了一个新的基础，大多数的创新还没有到来。Dan Abramov甚至把这个版本称为[MVP](https://twitter.com/dan_abramov/status/1509008072550846464?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)，其目标似乎基本上是促进并发式React的逐步采用。一些人如[Paul Henschel](https://twitter.com/0xca0a/status/1508850096447840256?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)（React-Three-Fiber）或 [James Ide](https://twitter.com/JI/status/1508849489305432066?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)已经预测到一些巨大的性能影响。

我认为我们正在进入一个新的时代。一些网络框架，如Svelte或Solid，由于其简单性和性能，正在变得流行。与React不同，它们是真正的响应式和无虚拟DOM。

[React的虚拟DOM是有代价的](https://svelte.dev/blog/virtual-dom-is-pure-overhead?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)，但我认为如果没有这个抽象，Concurrent React是很难实现的。随着React 18+，我们将最终知道这个代价是否值得付出。在未来的几年里，将React的用户体验、DX和性能与Svelte或Solid进行比较将是非常有趣的。

[**RedwoodJS v1.0**](https://community.redwoodjs.com/t/redwood-1-0-is-now-available/2958?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)

现在是Redwood的[Launch Week](https://v1launchweek.redwoodjs.com/?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)，V1.0刚刚发布，另一个重要的公告计划在周四发布。这个受Ruby on Rails启发的React元框架比它的竞争对手更有主见，并且可以通过与Prisma、GraphQL、Storybook、TypeScript、Jest的意见整合，帮助你更快地交付产品。它的创造者Tom Preston-Werner（也是GitHub、Jekyll的创造者......）正在以可持续的方式（没有风险投资） [在未来一年内用100万美元资助这个框架](https://tom.preston-werner.com/2022/04/04/redwood-v1-and-funding.html?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter).

[**Remixing React Router**](https://remix.run/blog/remixing-react-router?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)

Remix和React-Router仓库将合并为Remix，Remix中的许多功能将在React-Router中提供：数据加载、突变、中断、重新验证、竞赛条件...... 这些抽象被认为是与Suspense和  ["render-as-you-fetch"](https://17.reactjs.org/docs/concurrent-mode-suspense.html?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter#approach-3-render-as-you-fetch-using-suspense)模式的最佳结合。

### **拓展阅读**

-   📜 [Remix: The Yang to React's Yin](https://kentcdodds.com/blog/remix-the-yang-to-react-s-yin?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)
-   📜 [Improving Web Page Performance at DoorDash Through Server-Side Rendering with Next.JS](https://doordash.engineering/2022/03/29/improving-web-page-performance-at-doordash-throughserver-side-rendering-with-next-js/?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter): great feedback of a complex migration at scale
-   📜 [Hooks Considered Harmful](https://labs.factorialhr.com/posts/hooks-considered-harmful?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)
-   📜 [When Does React Render Your Component?](https://www.zhenghao.io/posts/react-rerender?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)
-   📜 [SSR Date Formatting in Remix using the User's Locale](https://donavon.com/blog/remix-locale?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)
-   📜 [How Does Shallow Comparison Work In React?](https://www.chakshunyu.com/blog/how-does-shallow-comparison-work-in-react/?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)
-   📜 [Trying out Ladle - A Storybook Alternative](https://dev.to/mbarzeev/trying-out-ladle-a-storybook-alternative-f68?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)
-   📜 [Why React 18 Broke Your App](https://dev.to/this-is-learning/why-react-18-broke-your-app-4730?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)
-   🐦 React core team: [Brian Vaughn leaves](https://twitter.com/brian_d_vaughn/status/1509558012956102663?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter), [Mengdi Chen enters](https://twitter.com/mengdi_en/status/1508845599340310533?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)
-   🐦 [useId() + React keys?](https://twitter.com/reactjs/status/1510334505252491267?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter) ❌
-   🐦 [useDeferredValue mental model: "like debounce but React decides when to bounce"](https://twitter.com/reactjs/status/1509458435586338821?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)
-   🐦 [JSX && conditionals](https://twitter.com/kadikraman/status/1507654900376875011?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter): pitfalls to know! There are ESLint plugins for that ([1](https://twitter.com/radexp/status/1508543569379958787?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter), [2](https://github.com/jeremy-deutsch/eslint-plugin-jsx-falsy?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter))
-   🐦 [Next.js + Partytown "worker"](https://twitter.com/adamdbradley/status/1506333446737739780?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)
-   🐦 [React + Qwik](https://twitter.com/Steve8708/status/1506729726420742145?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)
-   🎥 [The Story of Next.js](https://www.youtube.com/watch?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter&v=BILxV_vrZO0)
-   📦 React-Three-Fiber: [v8.0](https://twitter.com/0xca0a/status/1509179201080995843?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter) (with** React-Native support!**) + [Babel plugin](https://twitter.com/umariomaker/status/1509324799926943744?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)
-   📦 [React Router v6.3.0](https://remix.run/blog/react-router-v6.3.0?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter): compatibility v5
-   📦 [React Testing Library v13](https://twitter.com/matanbobi/status/1509421450305937411?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)
-   📦 [React-Query v4.0.0-beta.1](https://twitter.com/TkDodo/status/1510223448429277188?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)
-   📦 [Chicane v1.0](https://twitter.com/zoontek/status/1508434249577373696?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)
-   📦 [Gatsby v4.11](https://www.gatsbyjs.com/docs/reference/release-notes/v4.11/?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)

## React-Native

[**React Native v0.68**](https://reactnative.dev/blog/2022/03/30/version-068?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)

这个版本非常重要，因为它是React-Native的第一个可以通过一个标志轻松激活**新架构**（Fabric和TurboModules）的版本

Expo的下一个版本（SDK 45） [应该是基于v0.68的](https://twitter.com/Baconbrix/status/1509506872071663620?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)，但新架构 [不会立即在Expo Go中使用](https://twitter.com/Baconbrix/status/1506656896706568198?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)（但可能会在自定义开发客户端中启用）。

### **拓展阅读**

-   🐦 [TypeScript moduleSuffixes](https://twitter.com/sebastienlorber/status/1510995344422846470?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter): improves integration between TypeScript and React-Native extensions (`Comp.ios.tsx`)
-   🐦 [React Native for Web 0.18 preview](https://twitter.com/ReactWeb/status/1506716803975634945?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)
-   📜 [Deep dive into React Native JSI](https://engineering.teknasyon.com/deep-dive-into-react-native-jsi-5fbad4ea8f06?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)
-   📜 [Ionic vs. React Native: Performance Comparison](https://ionicframework.com/blog/ionic-vs-react-native-performance-comparison/?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)
-   📜 [How do you cache FlatList.renderItem?](https://andrei-calazans.com/posts/2022-03-31/memoization-mistake-flatlist-renderitem?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)
-   🎥 React-Native-Skia: [Neumorphism](https://www.youtube.com/watch?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter&v=0FC8O9mRUmg) + [Gen-Z mode](https://www.youtube.com/watch?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter&v=0FC8O9mRUmg)
-   🎙️ [React Native Radio 230 - We React to News](https://reactnativeradio.com/episodes/rnr-230-we-react-to-news?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)
-   🎙️ [React Native Show 12 - Mobile Payments in React Native](https://www.callstack.com/podcasts/mobile-payments-in-react-native?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)
-   📦 [Nx Expo Support](https://blog.nrwl.io/introducing-expo-support-for-nx-3fffb1849a6f?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)
-   📦 [OneSignal Expo Plugin](https://onesignal.com/blog/our-onesignal-expo-plugin-is-now-available/?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)
-   📦 [React-Native-Google-SignIn Expo Plugin](https://twitter.com/vonovak/status/1508735715605057541?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)

## 其它

[**Updates from the 89th TC39 meeting**](https://dev.to/hemanth/updates-from-the-89th-tc39-meeting-5bkf?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)

巨大的TC39更新! 我的关注:

-   Decorators stage 3, 最终回到正轨上了!
-   通过复制修改数组 in stage 3: JS数组的不可变方法! 也是[Records & Tuples](https://sebastienlorber.com/records-and-tuples-for-react?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)进步的一个[重要步骤](https://twitter.com/r_ricard/status/1509232839719632899?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter) 。
-   类型声明（Type annotations） stage 1 🤯
-   Intl.MessageFormat in stage 1: could reduce bundle size of apps using React-Intl.

### **拓展阅读**

-   [A Built-in Test Runner Is Coming to Node and Why You Should Care](https://fusebit.io/blog/node-testing-comes-to-core/?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter): new out-of-the-box test runner in Node.js 18! 🤯
-   [Release Notes for Safari Technology Preview 142](https://webkit.org/blog/12522/release-notes-for-safari-technology-preview-142/?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter): CSS Container Queries!
-   [From Static to Interactive: Why Resumability is the Best Alternative to Hydration](https://www.builder.io/blog/from-static-to-interactive-why-resumability-is-the-best-alternative-to-hydration?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter): interesting model used by Qwik
-   [Announcing Rome Formatter](https://rome.tools/blog/2022/04/05/rome_formatter_release?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)
-   [How to Write TypeScript Like a Haskeller](https://serokell.io/blog/typescript-for-haskellers?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)
-   [Conquering JavaScript Hydration](https://dev.to/this-is-learning/conquering-javascript-hydration-a9f?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)
-   [How return await can slow down your code](https://arthur.place/the-cost-of-return-await?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)
-   [Optimising Core Web Vitals on SPAs](https://simonhearne.com/2022/core-web-vitals-on-spas/?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)
-   [Cache and Prizes - Serious Platforms Don't Play Favourites](https://infrequently.org/2022/03/cache-and-prizes/?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)
-   [TypeScript Optional variance annotations](https://github.com/microsoft/TypeScript/pull/48240?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)
-   [TS Pattern v4.0](https://twitter.com/GabrielVergnaud/status/1508384947928764420?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)
-   [Boxed: Functional utility types and functions for TypeScript](https://swan-io.github.io/boxed/?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)
-   [Types as comments: Strong types, weakly held](https://blog.logrocket.com/types-as-comments-strong-types-weakly-held/?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)
-   [The Ultimate TypeScript Thread](https://twitter.com/mpocock1/status/1509964736275927042?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)
-   [WebContainers are out of beta in Chromium](https://blog.stackblitz.com/posts/webcontainers-out-of-beta/?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)
-   [Parcel v2.4.0](https://parceljs.org/blog/v2-4-0/?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)
-   [Vite 2.9](https://twitter.com/vite_js/status/1509165446595072001?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)
-   [Understanding CSS Layout Algorithms](https://www.joshwcomeau.com/css/understanding-layout-algorithms/?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)
-   [Picture perfect images with the modern img element](https://stackoverflow.blog/2022/03/28/picture-perfect-images-with-the-modern-element/?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)
-   [Those HTML Attributes You Never Use](https://www.smashingmagazine.com/2022/03/html-attributes-you-never-use/?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)
-   [Dum: npm script runner in Rust](https://github.com/egoist/dum?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)
-   [Storybook Figma plugin beta](https://storybook.js.org/blog/figma-plugin-beta/?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)
-   [What's new in Node.js core? March 2022 edition](https://simonplend.com/whats-new-in-node-js-core-march-2022-edition/?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)
-   [Astro 1.0 Beta Release](https://astro.build/blog/astro-1-beta-release/?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)
-   [14 Linting Rules To Help You Write Asynchronous Code in JavaScript](https://maximorlov.com/linting-rules-for-asynchronous-code-in-javascript/?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)
-   [Node.js community update](https://developers.redhat.com/articles/2022/03/18/nodejs-community-update?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)
-   [GraphQL Yoga 2.0](https://www.the-guild.dev/blog/announcing-graphql-yoga-2?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)
-   [Electron v18.0](https://www.electronjs.org/blog/electron-18-0?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)

<img width="686" alt="image" src="https://user-images.githubusercontent.com/749374/161927657-2ef832ae-28b9-422e-ac7f-9f0603215167.png">
