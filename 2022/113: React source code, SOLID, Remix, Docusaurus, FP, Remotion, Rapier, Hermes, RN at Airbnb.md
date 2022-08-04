## React

[**Reading Source Code: React**](https://alexkondov.com/readint-source-code-react/?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)

Alex阅读了React的源代码，并对几个部分进行了评论，以React应用程序的安装为切入点。关于原型的使用、JJSX以及（不可知的）调和器与DOM渲染器的交互，都是有趣的细节。

[**Can We All Just Admit React Hooks Were a Bad Idea?**](https://medium.com/codex/can-we-all-just-admit-react-hooks-were-a-bad-idea-c48120c5188d?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)

Amy认为，React hooks 不尊重SOLID架构原则。我不太同意，但我承认，在网上找到的大多数例子都是简化的，不一定能突出一个好的架构。

[**Applying SOLID principles in React**](https://konstantinlebedev.com/solid-in-react/?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)


几乎是对上述文章的直接回答，即使SOLID的应用在这里被更广泛地覆盖（components + hooks）。注意：不要犹豫，使用React上下文进行依赖注入。


**拓展阅读**

-   📜 [Avoid anonymous components with displayName](https://julesblom.com/writing/component-displayname?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter): sometimes React can't infer a good name for your components, which complicates the use of devtools (Context, memo, forwardRef, HOC)
有时React不能为你的组件推断出一个好的名字，这使得devtools的使用变得复杂（Context, memo, forwardRef, HOC）。
-   📜 [Why Remix is not a React framework but a full stack web framework](https://andre-landgraf.dev/blog/2022-07-16_why_remix_is_not_a_react_framework_but_a_full_stack_web_framework/?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter): a well-written overview of the differences between Remix and other frameworks. Remix is full-stack and framework-agnostic.
这篇文章很好地概述了Remix与其他框架之间的区别。Remix是全栈式的，与框架无关。
-   📜 [Functional programming is finally going mainstream](https://github.com/readme/featured/functional-programming?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter): GitHub highlights the popularization of functional programming, in part thanks to React, Redux and hooks. I personally switched career from Scala to React after reading David Nolen's famous post. Didn't even like JS before 2014 😅
GitHub强调了函数式编程的普及，部分归功于React、Redux和hooks。我个人在读了David Nolen的名帖后，从Scala转行到React。2014年之前甚至不喜欢JS 😅。
-   📜 [Why Docusaurus is a powerful documentation framework](https://blog.1password.com/docusaurus-documentation-framework/?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter): 1Password explains why Docusaurus is a good solution for their developer documentation portal. Touch various advanced topics, including site customizations, remark plugins to extend MDX/Markdown...
1Password解释了为什么Docusaurus是他们开发者文档门户的一个很好的解决方案。触摸各种高级主题，包括网站定制，评论插件来扩展MDX/Markdown...
-   📜 [Store data in a cookie with sessions and Remix](https://jonmeyers.io/blog/store-data-in-a-cookie-with-sessions-and-remix?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter): creation of a visit counter cookie
-   📖 [Remix Deferred](https://github.com/remix-run/remix/blob/deferred/docs/guides/streaming.md?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter#using-deferred): new API under development that gives fine control over data loading tradeoffs on initial page load. Optimize for Time-to-first-byte or Cumulative Layout Shift.
正在开发的新的API，可以在初始页面加载时对数据加载的权衡进行精细控制。优化第一个字节的时间或累计布局转移。
-   📖 [Next.js accessibility doc improvements](https://twitter.com/nextjs/status/1549043787330375680?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)
-   🐦 [New Preact VDOM state model](https://twitter.com/_developit/status/1549001036802625536?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)
-   🐦 [Remix + React 18 startTransition + time-sliced hydration](https://twitter.com/ryanflorence/status/1547959632663961602?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter): Ryan Florence sharing a controversial tip. Starts interesting discussions about hydration ([Ryan Carniato](https://twitter.com/RyanCarniato/status/1549100194708353024?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter), [Andrew Clark](https://twitter.com/acdlite/status/1549109283387744256?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)...)
-   📦 [pmndrs/react-three-rapier](https://github.com/pmndrs/react-three-rapier?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter): integrates react-three-fiber with Rapier (physics engine)
-   📦 [Remotion 3.1](https://www.remotion.dev/blog/3-1?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter): many new features! Gifs, Tailwind CSS, springs with duration, OffthreadVideo...
-   📦 [Remix 1.6.5](https://github.com/remix-run/remix/releases/tag/remix%401.6.5?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter): loader + useLoaderData TypeScript inference👌
-   📦 [Framer Motion 6.5](https://twitter.com/mattgperry/status/1547581579974696961?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter): scroll animations
-   📦 [Zustand 4.0.0-rc.2](https://twitter.com/dai_shi/status/1548685973558800384?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter): ready for production
-   📦 [Redwood 2.1](https://github.com/redwoodjs/redwood/releases/tag/v2.1.0?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)

## React-Native

[**Hermes as the Default**](https://reactnative.dev/blog/2022/07/08/hermes-as-the-default?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)

JS Hermes引擎是JSC/V8的一个替代品。它可以通过字节码的预编译来帮助你的应用程序更快地启动。在React-Native 0.70（现在是 [候选版本](https://github.com/facebook/react-native/releases/tag/v0.70.0-rc.0?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)）中，Hermes被默认启用。Michael分享了来自开源应用Mattermost的各种基准数据。Hermes的发布模式已经改变，以避免ABI不兼容的问题。在iOS上增加了缺失的Intl APIs。即将推出对BigInt和WeakRef的支持。

[**What working at Airbnb during its React Native era taught me about web3**](https://medium.com/@devinabbott/what-working-at-airbnb-during-its-react-native-era-taught-me-about-web3-6d34d855d892?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)

Devin回顾了React-Native在Airbnb的历史，以及对其逐渐落幕的非常微妙的决定。 他与web3做了有趣的比较。 从长远来看，技术潜力胜过早期采用者的痛苦。

**拓展阅读**

-   📜 [Ionic - Announcing Portals for React Native](https://ionicframework.com/blog/announcing-portals-for-react-native/?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter): allows an integration of WebView Ionic experiences in a React-Native app. Paid product.
-   🎙️ [React-Native-Radio #242 - Inspecting React Native 0.69](https://reactnativeradio.com/episodes/rnr-242-inspecting-react-native-069?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)
-   🎙️ [The React Native Show #14 - React Native Paper v.5](https://www.callstack.com/podcasts/react-native-paper-v-5-update-overview?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)
-   📦 [Vision Camera 2.14](https://twitter.com/mrousavy/status/1548953154993127426?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter): can now chain frame processors
-   📦 [expo vscode 0.8](https://twitter.com/cedricvanputten/status/1549051333595971585?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter): JSON config autocomplete 👍
-   📦 [expo-music-picker](https://github.com/barthap/expo-music-picker?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)
-   📦 [react-native-iconic](https://github.com/nandorojo/react-native-iconic?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)
-   🧑‍🎨 [React-Native-Skia + Expo web demo](https://twitter.com/Baconbrix/status/1547974280670875648?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)
-   🧑‍🎨 [Instagram iOS page transitions demo](https://twitter.com/enesozt_/status/1549049433148403712?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)

---

## Other

[**Vite 3**](https://vitejs.dev/blog/announcing-vite3.html?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)

Vite很快成为了前端生态系统中的一个参考。今天，它是Create-React-App的一个很好的替代品，DX速度更快，一些React元框架也在使用它（Storybook，Hydrogen...）。V3有很多变化，新的文档，各种框架（包括React）的启动程序，全局导入的改进，新的文档... 也请看10月份的[ViteConf](https://viteconf.org/?utm_会议。

**拓展阅读**

-   [The Cost of Consistency in UI Frameworks](https://dev.to/this-is-learning/the-cost-of-consistency-in-ui-frameworks-4agi?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)
-   [Node.js 18.6 - Custom ESM loaders: Who, what, when, where, why, how](https://dev.to/jakobjingleheimer/custom-esm-loaders-who-what-when-where-why-how-4i1o?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)
-   [A New Pattern For The Jamstack: Segmented Rendering](https://www.smashingmagazine.com/2022/07/new-pattern-jamstack-segmented-rendering/?ref=sidebar&utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)
-   [Event-Driven JavaScript Development](https://whistlr.info/2022/event-driven-js/?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)
-   [Chrome Dev Insider: The CSS and UI edition](https://developer.chrome.com/blog/insider-july-2022/?linkId=8100396&utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)
-   [Safari Technology Preview 149](https://webkit.org/blog/12998/release-notes-for-safari-technology-preview-149/?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)
-   [NestJS v9](https://trilon.io/blog/nestjs-9-is-now-available?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)
-   [Parcel CSS 1.12](https://twitter.com/devongovett/status/1547615708988600322?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)

---

<img width="685" alt="CleanShot 2022-07-19 at 21 09 19@2x" src="https://user-images.githubusercontent.com/749374/179829775-1e041995-9a6e-4681-aed4-ae661c58d84f.png">


  订阅原文:
-   🇬🇧 [ThisWeekInReact.com](https://thisweekinreact.com/)
-   🇫🇷 [ReactHebdo.fr](https://reacthebdo.fr/)
