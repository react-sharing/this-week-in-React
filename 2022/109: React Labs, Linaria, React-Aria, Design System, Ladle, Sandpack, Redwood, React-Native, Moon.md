This Week In React #109: React Labs, Linaria, React-Aria, Design System, Ladle, Sandpack, Redwood, React-Native, Moon...
===

## React

[**React Labs: What We've Been Working On -- June 2022**](https://reactjs.org/blog/2022/06/15/react-labs-what-we-have-been-working-on-june-2022.html?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)

React Labs是一个新的系列文章：React团队希望更经常地分享其进展。阅读整篇文章：它包含了很多非常有趣的信息，特别是。

- 服务器组件：async/await模型，不再有`.server.js`扩展，Webpack/Vite统一
- React优化编译器（React Forget）的重写，似乎进展顺利。
- Offscreen API提供了新的非常有趣的功能（即时转换 ❤️️）。

可以看[Dan Abramov 的评论](http://reddit.com/r/reactjs/comments/vd0w6g/react_labs_what_weve_been_working_on_june_2022/ickr47j/?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)

[**Airbnb's Trip to Linaria**](https://medium.com/airbnb-engineering/airbnbs-trip-to-linaria-dc169230bd12?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)

Airbnb解释了他们如何从Sass到react-with-styles，然后是Linaria。这是一个没有运行时间的CSS-in-JS框架，具有静态CSS提取功能。他们解释了他们的选择，迁移策略，并对他们所贡献的工具给予了积极的反馈。

[**React Aria - Date and Time Pickers for All**](https://react-spectrum.adobe.com/blog/date-and-time-pickers-for-all.html?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)

React Aria刚刚宣布发布了日期和时间选择器组件和钩子。正如你所期望的那样，它真正关注的是可访问性、灵活性和国际化。我们可以感觉到，这些组件的背后有Adobe团队的大量工作。

[**Notes on maintaining an internal React component library**](https://www.gabe.pizza/notes-on-component-libraries/?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)

Gabe在Walrus工作，这是Digital Ocean内部的React设计系统。他对React设计系统的长期维护提供了非常详细的反馈。他分享了关于人类方面以及道具设计、组件封装或版本升级管理方面的有趣经验。

[**Capture Phase Event Handling in React**](https://kyleshevlin.com/capture-phase-event-handling-in-react?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)

我们经常使用DOM事件的 "冒泡 "阶段，但有时使用 "捕获 "阶段也是很有用的，这个阶段并不为人所知。我们可以使用例如`onClickCapture`与React。

**拓展阅读**

-   📜 [5 Big Takeaways from Remix Conf](https://www.simplethread.com/5-big-takeaways-from-remix-conf/?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)
-   📜 [What is XState used for?](https://stately.ai/blog/what-is-xstate-used-for?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)
-   📜 [The Case for Use.GPU](https://acko.net/blog/the-case-for-use-gpu/?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)
-   📜 [Why Use useReducer?](https://kyleshevlin.com/why-use-use-reducer?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)
-   📜 [React Element vs Component](https://www.robinwieruch.de/react-element-component/?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)
-   📜 [Inversion of Control and JSX Injection via Context API](https://theroadtoenterprise.com/blog/react-inversion-of-control-and-jsx-injection-via-context-api?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)
-   📖 [You Might Not Need an Effect](https://twitter.com/dan_abramov/status/1539034955094933504?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter): new doc page in beta
-   📦 [Sandpack 1.0](https://codesandbox.io/post/announcing-sandpack-v1?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter): React components to build interactive code playground, from CodeSandbox. New design, theming, SSR support, React 18, file explorer...
-   📦 [Ladle 1.0](https://ladle.dev/blog/ladle-v1?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter): Storybook alternative based on Vite, built for Uber. Can now customize Vite config + addons for accessibility and accessing story source.
-   📦 [uipkg](https://uipkg.com/?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter): new plugin to export Figma designs to React.
-   📦 [Remix-routers](https://github.com/brophdawg11/remix-routers?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter): adapt Remix router to other frameworks (for now only Vue)
-   📦 [React-Teleporter 3.0](https://github.com/gregberge/react-teleporter/releases/tag/v3.0.0?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter): React 18 support
-   📦 [SWR 2.0 Beta 4](https://twitter.com/shuding_/status/1538165993448652800?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter): resource preloading API
-   📦 [React-cmdk](https://github.com/albingroen/react-cmdk?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter): A command palette for React
-   📦 [Redwood 2.0](https://twitter.com/RedwoodJS/status/1537798365609615363?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter): 3 months after v1.0? Don't panic! It's just a few breaking changes, Redwood respects semantic versioning.
-   📦 [React 18.2](https://twitter.com/dan_abramov/status/1536822549245575168?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter): SSR bugfixes
-   📦 [Vitext](https://github.com/aslemammad/vitext?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter): Next.js alternative based on Vite?
-   🐦 [React-Three-Fiber + Html embed](https://twitter.com/sebastienlorber/status/1539235102143795200?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)
-   👥 [React-conferences](https://github.com/nvh95/react-conferences?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)
-   🧵 [React Summit Sketches](https://twitter.com/flexbox_/status/1538874305596928005?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)

## React-Native

[**Helping migrate React Native libraries to the New Architecture**](https://reactnative.dev/blog/2022/06/16/resources-migrating-your-react-native-library-to-the-new-architecture?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)

React-Native团队解释了他们将如何帮助我们采用新的架构。将会有文档，通过工作组提供支持，但也有GitHub仓库，其中有许多应用和迁移分支的例子。请注意，React-Native 0.69（含React 18）应该很快就会推出：Concurrent React的功能将只对新架构的用户开放。

[**@shopify/react-native-performance**](https://github.com/Shopify/react-native-performance?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)

由Shopify创建的包，以剖析你的应用程序的性能。一流的React-Navigation和FlatList支持。

⚠️警告：3个流行的软件包现在有相同的名字 😅。

**拓展阅读**

-   📜 [Writing fastlane scripts in Javascript](https://reaper.is/writing/20220616-fastlane-in-javascript?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)
-   🧵 [Metro + web](https://twitter.com/sebastienlorber/status/1538925340193595395?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter): Metro web usage is increasing: Airbnb, Stripe, Expo...
-   📦 [React-Native-Owl 1.0](https://twitter.com/kadikraman/status/1537040838424944640?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter): visual regression testing lib for React-Native reaching v1 milestone
-   📦 [React-Native-Performance Config Plugin](https://twitter.com/almouro/status/1539260205162176513?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter) (not the same 😅)
-   📦 [Siri Shortcuts Config Plugin](https://twitter.com/Baconbrix/status/1537102639586021378?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)
-   📦 [React-Native-Firebase v15](https://twitter.com/fastsquatch/status/1538715138236235776?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)
-   🎙️ [RNR 239 - Shrink your app with ProGuard](https://reactnativeradio.com/episodes/rnr-239-shrink-your-app-with-proguard-james-hamilton?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)
-   🎙️ [The React Native Show Coffee Talk #3 - Open Source](https://www.callstack.com/podcasts/coffee-talk-3-open-source?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)
-   🎙️ [The React Native Show #13 - Migration to React Native](https://www.callstack.com/podcasts/migration-to-react-native?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)

---

## 其它

[**The cost of convenience**](https://surma.dev/things/cost-of-convenience/?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)

对前端抽象及其成本的有趣思考... 提出了一个有趣的心理模型来区分框架和库（IoC--好莱坞原则--"不要叫我们，我们会叫你"）。所有这些都用一些React的例子来说明。

[**Moon - A build system for the JavaScript ecosystem**](https://moonrepo.dev/?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)

似乎是Nx和Turborepo的新竞争者，这次是用Rust写的😏

**拓展阅读**

-   [TypeScript 4.8 Beta](https://devblogs.microsoft.com/typescript/announcing-typescript-4-8-beta/?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)
-   [Why You Might Prefer Map Over Object In JavaScript](https://www.zhenghao.io/posts/object-vs-map?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)
-   [Sponsoring dependencies: The next step in open source sustainability](https://humanwhocodes.com/blog/2022/06/sponsoring-dependencies-open-source-sustainability/?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)
-   [CSS - Complex vs Compound Selectors](https://www.miriamsuzanne.com/2022/06/15/complex-compound/?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)
-   [Socket for GitHub 1.0](https://socket.dev/blog/socket-for-github-1.0?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)
-   [State of Open Source Security 2022](https://snyk.io/reports/open-source-security/?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)
-   [CSS - Backdrop Filter finally in Firefox 103](https://twitter.com/sebastienlorber/status/1539190607922479109?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)
-   [V8 - Discontinuing release blog posts](https://v8.dev/blog/discontinuing-release-posts?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)
-   [Bringing forward the End-of-Life Date for Node.js 16](https://nodejs.org/en/blog/announcements/nodejs16-eol/?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)
-   [CSS - New syntax for range media queries in Chrome 104](https://developer.chrome.com/blog/media-query-range-syntax/?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)
-   [Software Engineering - The Soft Parts](https://addyosmani.com/blog/software-engineering-soft-parts/?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)
-   [Lerna 5.1](https://twitter.com/NxDevTools/status/1537110739403493378?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)
-   [Boa v0.15](https://boa-dev.github.io/posts/2022-06-10-boa-release-15/?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)
-   [zx 7.0](https://github.com/google/zx/releases/tag/7.0.0?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)
-   [Tauri 1.0](https://tauri.app/blog/tauri_1_0?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)
-   [Deno 1.23](https://twitter.com/deno_land/status/1537405732349411328?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)
-   [Deno raises $21M](https://deno.com/blog/series-a?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)


<img width="530" alt="CleanShot 2022-06-22 at 11 42 01@2x" src="https://user-images.githubusercontent.com/749374/174998031-272e34a8-2a3c-4176-9009-97284b5a11a7.png">

  订阅原文:
-   🇬🇧 [ThisWeekInReact.com](https://thisweekinreact.com/)
-   🇫🇷 [ReactHebdo.fr](https://reacthebdo.fr/)
 
