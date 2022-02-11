
原文地址：https://www.getrevue.co/profile/thisweekinreact/issues/this-week-in-react-91-remix-next-js-server-components-forms-react-native-typescript-monorepos-994552

## React

### [Remix vs Next.js](https://remix.run/blog/remix-vs-next?utm_campaign=thisweekinreact&utm_medium=email&utm_source=Revue%20newsletter)

我们终于有了与Next.js的正式比较！

首先，你应该知道，Remix团队非常欣赏Vercel平台，尽管Next.js和Remix之间存在竞争。但他们说Remix显然更好😏而且有很好的论据和watefalls来证明这一点。

这个比较是基于一个真实世界的电子商务应用，与Shopify的API集成，他们基本上分析了2个页面：一个具有相当静态内容的登陆页面和一个非常动态的搜索页面。所有这些都部署在Vercel和Fly上。

服务器渲染的优势的一个很好的亮点：有时在服务器端渲染所有内容，而不是将两者混合在一起（正如Next.js似乎推荐的那样）：静态外壳，以及在客户端获取的搜索结果。

Next.js更复杂，它的生命周期函数到处运行（服务器、浏览器等）。Remix更倾向于保持简单，只做动态渲染，但要做得好。通过依赖浏览器的本地函数，这也减少了客户端需要发送的JavaScript数量。

文章很长，不容易总结，读完后可以自己做决定。我还没有完全理解Remix，对于Shopify API宕机时的错误处理、安全性、Redis缓存的架构复杂性、缓存失效时应用的重新部署......总之，Jamstack有很多我们喜欢的，而且也不想失去的东西

总的来说，这真的让我想在一个非关键项目上尝试Remix：幸运的是，正好我需要为我的文章建立一个网站，刚好可以尝试下。

### [How React server components work: an in-depth guide](https://blog.plasmic.app/posts/how-react-server-components-work/?utm_campaign=thisweekinreact&utm_medium=email&utm_source=Revue%20newsletter)

这是一篇关于服务器组件如何工作的非常有趣且相当技术性的文章。很多细节都是我到目前为止在其他地方都没见过的。特别解释了服务器端的React树是如何通过 "模块引用 "在JSON中序列化的，并提供了一些客户端/服务器通信的有效负载示例。

**Extras:**

-   [What is a react component, anyways?](https://thoughtspile.github.io/2022/01/25/what-is-react-component/?utm_campaign=thisweekinreact&utm_medium=email&utm_source=Revue%20newsletter): 关于究竟什么是React组件的有趣想法。不太容易描述，即使是官方文档也是如此。建议4个定义，其中一个是 "*unite of update*".
-   [Mastering the art of forms in React](https://engineering.udacity.com/mastering-the-art-of-forms-in-react-1bd65fb664d7?utm_campaign=thisweekinreact&utm_medium=email&utm_source=Revue%20newsletter): Kolby认为使用受控输入不应该是自动的,他推荐React-Hook-Form + Zod来满足高级需求.
-   [Sneak peek into React 18 useDeferredValue hook](https://blog.saeloun.com/2022/01/13/react-18-usedefferedvalue-hook?utm_campaign=thisweekinreact&utm_medium=email&utm_source=Revue%20newsletter): 允许在React中取消一些渲染工作的优先级，使紧急更新的速度更快
-   [Exploring React 18’s three new APIs](https://blog.logrocket.com/exploring-react-18-three-new-apis/?utm_campaign=thisweekinreact&utm_medium=email&utm_source=Revue%20newsletter): useId, useSyncExternalStore, useInsertionEffect
-   [How Redux DevTools broke Jira for 14 hours](https://nathanbierema.com/redux-devtools-jira/?utm_campaign=thisweekinreact&utm_medium=email&utm_source=Revue%20newsletter): 有趣的事后总结，与React没有多大关系
-   [Vercel Platforms Starter Kit](https://demo.vercel.pub/platforms-starter-kit?utm_campaign=thisweekinreact&utm_medium=email&utm_source=Revue%20newsletter): Vercel发布了一个基于Next.js的模板，供那些想要创建平台（多租户，每个租户一个域名）的人使用。给出了一些例子，比如Hashnode博客平台。
-   [Blitz pivot is confirmed](https://github.com/blitz-js/blitz/discussions/3075?utm_campaign=thisweekinreact&utm_medium=email&utm_source=Revue%20newsletter#discussioncomment-1951662): meta-framework将转化为Blitz Toolkit，这是一个与框架无关的工具包，应该可以很好地在其他框架之上工作（首先是Next.js）, 与[tRP的合作](https://github.com/blitz-js/blitz/discussions/3083?utm_campaign=thisweekinreact&utm_medium=email&utm_source=Revue%20newsletter#discussioncomment-1841427) 是可能的.
-   Custom Elements + React: [Dan Abramov asks again for community feedback](https://github.com/facebook/react/issues/11347?utm_campaign=thisweekinreact&utm_medium=email&utm_source=Revue%20newsletter#issuecomment-1016816876)
-   [Storybook Addon Next](https://twitter.com/storybookjs/status/1484910294694604807?utm_campaign=thisweekinreact&utm_medium=email&utm_source=Revue%20newsletter)
-   [Remix Conf](https://remix.run/conf?utm_campaign=thisweekinreact&utm_medium=email&utm_source=Revue%20newsletter): 24-25th May
-   🐦 Daishi Kato 解释了这些库的工作原理 : [Zustand](https://twitter.com/dai_shi/status/1484849542671790081?utm_campaign=thisweekinreact&utm_medium=email&utm_source=Revue%20newsletter), [Jotai](https://twitter.com/dai_shi/status/1485434083778117632?utm_campaign=thisweekinreact&utm_medium=email&utm_source=Revue%20newsletter), [Valtio](https://twitter.com/dai_shi/status/1484496249776934917?utm_campaign=thisweekinreact&utm_medium=email&utm_source=Revue%20newsletter)
-   🐦 [Props drilling: context is not the only option](https://twitter.com/asidorenko_/status/1484934183361339399?utm_campaign=thisweekinreact&utm_medium=email&utm_source=Revue%20newsletter)
-   🎥 [Remix Singles](https://www.youtube.com/watch?list=PLXoynULbYuEDG2wBFSZ66b85EIspy3fy6&utm_campaign=thisweekinreact&utm_medium=email&utm_source=Revue%20newsletter&v=jd_bin5HPrw): new series of videos about Remix
-   🧵 [Amazon dev: “SSR React wasn’t fast enough for us.”](https://twitter.com/amilajack/status/1484970825568505856?utm_campaign=thisweekinreact&utm_medium=email&utm_source=Revue%20newsletter): an Amazon employee explains how they optimized the site. Not a lot of details about React unfortunately.
-   [Deep dive into the new Suspense Server-side Rendering](https://blog.saeloun.com/2022/01/20/new-suspense-ssr-architecture-in-react-18.html?utm_campaign=thisweekinreact&utm_medium=email&utm_source=Revue%20newsletter)
-   [Type-safe routing in React with ](https://oliverjash-me.vercel.app/2022/type-safe-routing-in-react-with-fp-ts-routing-part-1?utm_campaign=thisweekinreact&utm_medium=email&utm_source=Revue%20newsletter)`fp-ts-routing`[ (part 1)](https://oliverjash-me.vercel.app/2022/type-safe-routing-in-react-with-fp-ts-routing-part-1?utm_campaign=thisweekinreact&utm_medium=email&utm_source=Revue%20newsletter) 

## React Native
### [Announcing React Native 0.67](https://reactnative.dev/blog/2022/01/19/version-067?utm_campaign=thisweekinreact&utm_medium=email&utm_source=Revue%20newsletter)

It’s not the release with the most exciting highlights 😅 This blog post mainly talks about the improvements of the release process, that should be more robust and regular.This process is also mentioned in another post

这并不是最令人兴奋的发布点 😅 这篇文章主要谈了发布过程中的改进，应该更稳健和规范。这个过程另外一篇文章中被提及到

### [React Native - H2 2021 Recap](https://reactnative.dev/blog/2022/01/21/react-native-h2-2021-recap?utm_campaign=thisweekinreact&utm_medium=email&utm_source=Revue%20newsletter)

this is an important step for the rollout of the [New Architecture](https://deploy-preview-2879--react-native.netlify.app/docs/next/new-architecture-intro?utm_campaign=thisweekinreact&utm_medium=email&utm_source=Revue%20newsletter). Another reminder that React-Native is not just iOS + Android 😏.Note: we should have some updates from Microsoft about the MacOS and Windows platforms, as they are catching up with upstream releases.

### [From Native to React Native to Flutter](https://zerodha.tech/blog/from-native-to-react-native-to-flutter?utm_campaign=thisweekinreact&utm_medium=email&utm_source=Revue%20newsletter)

Quite a long but very interesting article, which fairly discusses the various problems encountered with both React-Native and Flutter.I think their conclusion would be different if they were building for other platforms than iOS + Android (web support for example), or if they had a regular need to [mix native views with Flutter view](https://docs.flutter.dev/development/platform-integration/platform-views?utm_campaign=thisweekinreact&utm_medium=email&utm_source=Revue%20newsletter). Too bad [React-Native-Skia](https://github.com/Shopify/react-native-skia?utm_campaign=thisweekinreact&utm_medium=email&utm_source=Revue%20newsletter) didn’t exist earlier 😄, they might have liked it.

**附加功能：**

-   [Chain React cancelled this year](https://shift.infinite.red/chain-react-conf-vs-covid-2022-919724bf5aae?utm_campaign=thisweekinreact&utm_medium=email&utm_source=Revue%20newsletter)
-   🎥 [Unboxing Expo SDK 44](https://www.youtube.com/watch?utm_campaign=thisweekinreact&utm_medium=email&utm_source=Revue%20newsletter&v=bnMUQv2beXU)
-   🎙️ [RNR 224 - React Native Web on Next.js with Fernando Rojo](https://www.reactnativeradio.com/episodes/rnr-224-react-native-web-on-nextjs-with-fernando-rojo?utm_campaign=thisweekinreact&utm_medium=email&utm_source=Revue%20newsletter)
-   🐦 [React-Native Fabric + Apple TV](https://twitter.com/douglowder/status/1485780397787324419?utm_campaign=thisweekinreact&utm_medium=email&utm_source=Revue%20newsletter)
-   🐦 [iOS UI recreated with React-Native](https://twitter.com/enesozt_/status/1484627273009569794?utm_campaign=thisweekinreact&utm_medium=email&utm_source=Revue%20newsletter)
-   🐦 [Enter/Exit Layout animations with Reanimated](https://twitter.com/swmansion/status/1483475519970574336?utm_campaign=thisweekinreact&utm_medium=email&utm_source=Revue%20newsletter)
-   🐦 [Skia + Raycasting](https://twitter.com/Andriy20408222/status/1484484246009958400?utm_campaign=thisweekinreact&utm_medium=email&utm_source=Revue%20newsletter)
-   🐦 Flutter web: opinions from [Jake Archibald](https://twitter.com/jaffathecake/status/1483707543989936129?utm_campaign=thisweekinreact&utm_medium=email&utm_source=Revue%20newsletter) & [Jamie Kyle](https://twitter.com/buildsghost/status/1484637941460733952?utm_campaign=thisweekinreact&utm_medium=email&utm_source=Revue%20newsletter): confirms our choice to use React-Native for cross-platform 😄 

## 其它
### [Announcing TypeScript 4.6 Beta](https://devblogs.microsoft.com/typescript/announcing-typescript-4-6-beta/?utm_campaign=thisweekinreact&utm_medium=email&utm_source=Revue%20newsletter)

A great release that keeps adding useful improvements, notably on the [Control Flow Analysis](https://devblogs.microsoft.com/typescript/announcing-typescript-4-6-beta/?utm_campaign=thisweekinreact&utm_medium=email&utm_source=Revue%20newsletter#control-flow-analysis-for-dependent-parameters) that can be very useful for a React dev. The official blog post does not showcase this, but I tested and this will [improve a bit on React props destructuring](https://twitter.com/sebastienlorber/status/1485944134091354113?utm_campaign=thisweekinreact&utm_medium=email&utm_source=Revue%20newsletter), but unfortunately [not enough to work with ](https://twitter.com/sebastienlorber/status/1485944774506987526?utm_campaign=thisweekinreact&utm_medium=email&utm_source=Revue%20newsletter)`{...props}`: maybe for the next release?

### [Monorepo.tools](https://monorepo.tools/?utm_campaign=thisweekinreact&utm_medium=email&utm_source=Revue%20newsletter)

A well-presented page that gives you good reasons to adopt the monorepo, and compares some popular tools: Lerna, Nx, Turborepo, Bazel, Lage… Published by Nwrl (behind Nx), the comparison remains fair and quite objective.

**拓展阅读：**

-   [SpiderMonkey Newsletter (Firefox 96-97)](https://spidermonkey.dev/blog/2022/01/14/newsletter-firefox-96-97.html?utm_campaign=thisweekinreact&utm_medium=email&utm_source=Revue%20newsletter): Records & Tuples has been implemented in Firefox! You know [I love this](https://sebastienlorber.com/records-and-tuples-for-react?utm_campaign=thisweekinreact&utm_medium=email&utm_source=Revue%20newsletter) 😍!
-   [TypeScript Features to Avoid](https://www.executeprogram.com/blog/typescript-features-to-avoid?utm_campaign=thisweekinreact&utm_medium=email&utm_source=Revue%20newsletter): enums, namespaces, decorators, `private`
-   [TypeScript: How Type Guards Can Help You Get Rid of ‘as’](https://blog.theodo.com/2022/01/typescript-replace-as-typeguards/?utm_campaign=thisweekinreact&utm_medium=email&utm_source=Revue%20newsletter)
-   [What is the Jamstack in 2022?](https://remotesynthesis.com/blog/jamstack-in-2022?utm_campaign=thisweekinreact&utm_medium=email&utm_source=Revue%20newsletter)
-   [Div divisiveness](https://www.scottohara.me/blog/2022/01/20/divisive.html?utm_campaign=thisweekinreact&utm_medium=email&utm_source=Revue%20newsletter): when to use a `<div>` exactly?
-   [Safari Technology Preview 138](https://webkit.org/blog/12176/release-notes-for-safari-technology-preview-138/?utm_campaign=thisweekinreact&utm_medium=email&utm_source=Revue%20newsletter): with `:focus-visible` support. Controversial because [Apple needed crowdfunding](https://twitter.com/devongovett/status/1484893652728135685?utm_campaign=thisweekinreact&utm_medium=email&utm_source=Revue%20newsletter) 😅
-   [Fly: Free Postgres Databases](https://fly.io/blog/free-postgres/?utm_campaign=thisweekinreact&utm_medium=email&utm_source=Revue%20newsletter): moderne host @ Edge
-   [Opera Crypto Browser](https://blogs.opera.com/crypto/2022/01/opera-crypto-browser-project-web3?utm_campaign=thisweekinreact&utm_medium=email&utm_source=Revue%20newsletter)
-   `structuredClone()`[: deeply copying objects in JavaScript](https://2ality.com/2022/01/structured-clone.html?utm_campaign=thisweekinreact&utm_medium=email&utm_source=Revue%20newsletter)
-   🐦 [“Got tired of tsc taking forever to type check my code so I made a Typescript type checker in Rust for fun”](https://twitter.com/zack_overflow/status/1484277253353709570?utm_campaign=thisweekinreact&utm_medium=email&utm_source=Revue%20newsletter)
-   🎥 [Should you, a JavaScript developer, learn Rust in 2022?](https://www.youtube.com/watch?utm_campaign=thisweekinreact&utm_medium=email&utm_source=Revue%20newsletter&v=u-MyTHAXT6w) 
