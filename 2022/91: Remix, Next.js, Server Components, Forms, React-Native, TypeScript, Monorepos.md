
原文地址：https://www.getrevue.co/profile/thisweekinreact/issues/this-week-in-react-91-remix-next-js-server-components-forms-react-native-typescript-monorepos-994552

## React

### [Remix vs Next.js](https://remix.run/blog/remix-vs-next?utm_campaign=thisweekinreact&utm_medium=email&utm_source=Revue%20newsletter)

We finally have an official comparison with Next.js!

First, you should know that the Remix team really appreciates the Vercel platform, despite the competition between Next.js and Remix. But they say Remix is better obviously 😏 and there are good arguments and waterfalls to prove it.

This comparison is based on a real-world e-commerce app with a Shopify API integration, on which they essentially analyze 2 pages: a landing page with fairly static content, and a very dynamic search page. All this deployed on Vercel and Fly.

A good highlight of the advantages of server rendering: sometimes it’s better to render everything on the server side rather than doing a mix of the 2 (as Next.js seems to recommend): static shell, and search results fetched on the client side.

Next.js is more complex, with life-cycle functions that run everywhere (server, browser, etc.). Remix prefers to keep it simpler, just do dynamic rendering, but do it well. By relying on the browser’s native functions, this also reduces the amount of JavaScript to be sent on the client side.

Very long article, not easy to summarize, read it to make up your own mind. I haven’t fully understood Remix yet, and I still have some questions about error handling if the Shopify API goes down, security, architecture complexity with Redis cache, app redeployment with invalidation of the caches… In short, a lot of things that we like about the Jamstack and that we don’t necessarily want to lose.

Overall it really makes me want to try Remix on a non-critical project: luckily I need to build a website for this newsletter 😏

### [How React server components work: an in-depth guide](https://blog.plasmic.app/posts/how-react-server-components-work/?utm_campaign=thisweekinreact&utm_medium=email&utm_source=Revue%20newsletter)

Very interesting and quite technical article on how Server Components work. A lot of details that I haven’t seen anywhere else so far. Explains in particular how a server-side React tree is serialized in JSON with “module references”, and presents some examples of payloads for client/server communication.

**Extras:**

-   [What is a react component, anyways?](https://thoughtspile.github.io/2022/01/25/what-is-react-component/?utm_campaign=thisweekinreact&utm_medium=email&utm_source=Revue%20newsletter): interesting thoughts on what exactly is a React component. Not so easy to describe, even for the official docs. Suggest 4 definitions, one of them is “*unite of update*”.
-   [Mastering the art of forms in React](https://engineering.udacity.com/mastering-the-art-of-forms-in-react-1bd65fb664d7?utm_campaign=thisweekinreact&utm_medium=email&utm_source=Revue%20newsletter): Kolby believes that using controlled inputs shouldn’t be automatic, and recommends React-Hook-Form + Zod for advanced needs.
-   [Sneak peek into React 18 useDeferredValue hook](https://blog.saeloun.com/2022/01/13/react-18-usedefferedvalue-hook?utm_campaign=thisweekinreact&utm_medium=email&utm_source=Revue%20newsletter): permits to de-prioritize some rendering work in React, allowing urgent updates to be faster
-   [Exploring React 18’s three new APIs](https://blog.logrocket.com/exploring-react-18-three-new-apis/?utm_campaign=thisweekinreact&utm_medium=email&utm_source=Revue%20newsletter): useId, useSyncExternalStore, useInsertionEffect
-   [How Redux DevTools broke Jira for 14 hours](https://nathanbierema.com/redux-devtools-jira/?utm_campaign=thisweekinreact&utm_medium=email&utm_source=Revue%20newsletter): funny post-mortem, not so related to React
-   [Vercel Platforms Starter Kit](https://demo.vercel.pub/platforms-starter-kit?utm_campaign=thisweekinreact&utm_medium=email&utm_source=Revue%20newsletter): Vercel published a template based on Next.js for those that want to create platforms (multi-tenant, one domain per tenant). Gives some examples like the Hashnode blogging platform.
-   [Blitz pivot is confirmed](https://github.com/blitz-js/blitz/discussions/3075?utm_campaign=thisweekinreact&utm_medium=email&utm_source=Revue%20newsletter#discussioncomment-1951662): the meta-framework will be transformed into Blitz Toolkit, a framework-agnostic toolkit that should work nicely on top of others (Next.js first). For the “zero abstraction data layer”, a [collaboration with tRPC](https://github.com/blitz-js/blitz/discussions/3083?utm_campaign=thisweekinreact&utm_medium=email&utm_source=Revue%20newsletter#discussioncomment-1841427) may be possible.
-   Custom Elements + React: [Dan Abramov asks again for community feedback](https://github.com/facebook/react/issues/11347?utm_campaign=thisweekinreact&utm_medium=email&utm_source=Revue%20newsletter#issuecomment-1016816876)
-   [Storybook Addon Next](https://twitter.com/storybookjs/status/1484910294694604807?utm_campaign=thisweekinreact&utm_medium=email&utm_source=Revue%20newsletter)
-   [Remix Conf](https://remix.run/conf?utm_campaign=thisweekinreact&utm_medium=email&utm_source=Revue%20newsletter): 24-25th May
-   🐦 Daishi Kato explains how these libs work: [Zustand](https://twitter.com/dai_shi/status/1484849542671790081?utm_campaign=thisweekinreact&utm_medium=email&utm_source=Revue%20newsletter), [Jotai](https://twitter.com/dai_shi/status/1485434083778117632?utm_campaign=thisweekinreact&utm_medium=email&utm_source=Revue%20newsletter), [Valtio](https://twitter.com/dai_shi/status/1484496249776934917?utm_campaign=thisweekinreact&utm_medium=email&utm_source=Revue%20newsletter)
-   🐦 [Props drilling: context is not the only option](https://twitter.com/asidorenko_/status/1484934183361339399?utm_campaign=thisweekinreact&utm_medium=email&utm_source=Revue%20newsletter)
-   🎥 [Remix Singles](https://www.youtube.com/watch?list=PLXoynULbYuEDG2wBFSZ66b85EIspy3fy6&utm_campaign=thisweekinreact&utm_medium=email&utm_source=Revue%20newsletter&v=jd_bin5HPrw): new series of videos about Remix
-   🧵 [Amazon dev: “SSR React wasn’t fast enough for us.”](https://twitter.com/amilajack/status/1484970825568505856?utm_campaign=thisweekinreact&utm_medium=email&utm_source=Revue%20newsletter): an Amazon employee explains how they optimized the site. Not a lot of details about React unfortunately.
-   [Deep dive into the new Suspense Server-side Rendering](https://blog.saeloun.com/2022/01/20/new-suspense-ssr-architecture-in-react-18.html?utm_campaign=thisweekinreact&utm_medium=email&utm_source=Revue%20newsletter)
-   [Type-safe routing in React with ](https://oliverjash-me.vercel.app/2022/type-safe-routing-in-react-with-fp-ts-routing-part-1?utm_campaign=thisweekinreact&utm_medium=email&utm_source=Revue%20newsletter)`fp-ts-routing`[ (part 1)](https://oliverjash-me.vercel.app/2022/type-safe-routing-in-react-with-fp-ts-routing-part-1?utm_campaign=thisweekinreact&utm_medium=email&utm_source=Revue%20newsletter) 

## React Native
### [Announcing React Native 0.67](https://reactnative.dev/blog/2022/01/19/version-067?utm_campaign=thisweekinreact&utm_medium=email&utm_source=Revue%20newsletter)

It’s not the release with the most exciting highlights 😅 This blog post mainly talks about the improvements of the release process, that should be more robust and regular.This process is also mentioned in another post

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

## 合作专栏

-   [**Start React Native**](https://start-react-native.dev/?utm_campaign=thisweekinreact&utm_medium=email&utm_source=Revue%20newsletter)：与 William Candillon 一起学习有关手势和动画的一切
-   [**React-Native Weekly**](https://andrei-calazans.com/?utm_campaign=thisweekinreact&utm_medium=email&utm_source=Revue%20newsletter)：保持最新的 React-Native 核心更新
-   [**TypeScript Weekly**](https://www.typescript-weekly.com/?utm_campaign=thisweekinreact&utm_medium=email&utm_source=Revue%20newsletter)：每周最好的 TypeScript 链接，应该在你的邮箱里面。
-   [**ES.next News**](http://esnextnews.com/?utm_campaign=thisweekinreact&utm_medium=email&utm_source=Revue%20newsletter)：了解最新的 JavaScript 和跨平台工具
-   [**Tailwind Weekly**](https://tailwindweekly.com/?utm_campaign=thisweekinreact&utm_medium=email&utm_source=Revue%20newsletter) : 所有关于Tailwind CSS的东西，每周六新一期
-   [**G2i**](https://www.g2i.co/?utm_campaign=thisweekinreact&utm_medium=email&utm_source=Revue%20newsletter)：经过预先审查的远程 React 和 React-Native 开发人员，您可以按合同或完全信任本地开发人员
-   [**Infinite Red**](https://infinite.red/?utm_campaign=thisweekinreact&utm_medium=email&utm_source=Revue%20newsletter)：美国 React-Native 专家让您的想法成为现实
-   [**Software Mansion**](https://swmansion.com/?utm_campaign=thisweekinreact&utm_medium=email&utm_source=Revue%20newsletter)：React Native 的共同创造者，众多科技公司的技术核心
