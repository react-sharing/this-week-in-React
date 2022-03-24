This Week In React #98: React 18 RC2, Framer Motion, 3D Avatar, Parca, React-Native, Solito, Flutter, TypeScript, Safari...


## React

[**How to Upgrade to the React 18 Release Candidate**](https://reactjs.org/blog/2022/03/08/react-18-upgrade-guide.html?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)

[React 18.0.0-rc.2](https://www.npmjs.com/package/react?activeTab=versions&utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter) 已经发布 (可以使用npm tag `@rc`). React团队发表了一篇博文 (+ 🧵 [thread](https://twitter.com/reactjs/status/1501258790666178563?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)) 让我们为这个新版本的到来做好准备。它包括新的并发功能，我们可以逐步采用这些功能。

他们鼓励我们测试已发布的rc版本以检测最新的潜在错误，记录了主要的api和行为变化并提供了相当完整的升级指南。还有一个关于各种新的API的简要介绍。

直接阅读这个帖子，它包含许多有趣的细节。就我个人而言，我发现的概念是[Strict Effects](https://github.com/reactwg/react-18/discussions/19?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter) 以及[ composants现在支持渲染undefined](https://twitter.com/sebastienlorber/status/1501590568597610503?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter).

[**Delightful React File/Directory Structure**](https://www.joshwcomeau.com/react/file-structure/?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)

Josh Comeau的互动文章，介绍了他组织React应用的文件结构选择。强烈建议：他特别解释了为什么他更喜欢按类型而不是按功能分组文件。我不一定同意所有的东西，但它仍然是一个有趣的读物，有一些很好的论据。

[**Everything about Framer Motion layout animations**](https://blog.maximeheckel.com/posts/framer-motion-layout-animations/?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)

交互式文章，介绍了用Framer Motion制作的布局动画。介绍得非常好，有很多例子。我非常喜欢带有共享布局动画的标签的例子：API非常直观，我不知道有这么简单。

**拓展阅读:**

-   📜 [How to Use Three.js And React to Render a 3D Model of Your Self](https://blog.nourdinedev.com/how-to-use-three.js-and-react-to-render-a-3d-model/?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter): 原创文章，建议创建你自己的个人3D头像，用React-Three-Fiber显示它，并让它跳一些霹雳舞😄我真的想测试一下。
-   📜 [Profiling Next.js apps with Parca](https://www.polarsignals.com/blog/posts/2022/03/02/profiling-nextjs-app-with-parca/?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter): 这是我第一次听说Parca。对于那些自行托管Node.js应用程序的人来说，这似乎是一个有趣的持续集成评测工具（例如使用Kubernetes），在本地剖析性能问题时也可能很方便。在这个例子中，该工具检测到了一个与不必要地使用immutability有关的性能问题。
-   📜 [Why Did And Don't You Need To Import React](https://www.chakshunyu.com/blog/why-did-and-dont-you-need-to-import-react/?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)
-   📜 [Automatic batching support in React 18](https://www.dtreelabs.com/blog/automatic-batching-support-in-react-18?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)
-   📜 [What it's like to migrate a high-traffic website from Gatsby to Next.js](https://mikebifulco.com/posts/migrate-gatsby-to-nextjs-apisyouwonthate-com?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)
-   [🧑‍🎓](https://emojikeyboard.org/copy/Student_Emoji_%F0%9F%A7%91%E2%80%8D%F0%9F%8E%93?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=extlink) [Learn Next.js foundations](https://twitter.com/vercel/status/1503407398534500352?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter): Vercel为那些想在Next.js中打下坚实基础的初学者提供的新资源：假设你可能不知道React
-   👥 [Xuan Huang](https://twitter.com/Huxpro/status/1502483206569807874?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter): 新的React核心团队成员，主要从事于 [React-Forget](https://www.youtube.com/watch?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter&v=lGEMwh32soc)
-   👥 [Remix Conf Speakers](https://twitter.com/remix_run/status/1503400608165892098?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter) have been announced
-   🎙️ [Remix Podcast - Season 1](https://twitter.com/remix_run/status/1501716370831994885?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter): 12 episodes released
-   🐦 Malte Ubi: [*"JSX should be part of JavaScript"*](https://twitter.com/cramforce/status/1485778298042945540?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter) & Nicole Sullivan: [*"YES! But JSX is not enough on its own. Let me explain..."*](https://twitter.com/stubbornella/status/1502724909184679939?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)
-   🐦 [form attribute](https://twitter.com/sebastienlorber/status/1503428181134557185?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter), [formAction](https://twitter.com/ryanflorence/status/1502349821054644225?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter): web APIs that we (I) discover using Remix 🤯
-   🐦 [SolidJS signals in React](https://twitter.com/tannerlinsley/status/1502116674689925123?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter) + [Preact/reactive addon](https://github.com/preactjs/preact/pull/3474?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter): several experiments around reactivity
-   🎥 [Basic React To Svelte Conversion](https://www.youtube.com/watch?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter&v=DiSuwLlhOxs)
-   🎥 [React Query in 100 Seconds](https://www.youtube.com/watch?t=1s&utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter&v=novnyCaa7To)

## React-Native

[**An update on the New Architecture Rollout**](https://reactnative.dev/blog/2022/03/15/an-update-on-the-new-architecture-rollout?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)

Nicola提醒说，新的架构即将到来，并介绍了为社区做准备的不同举措：

-   [工作群](https://github.com/reactwg/react-native-new-architecture?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)
-   [升级指南](https://reactnative.dev/docs/next/new-architecture-intro?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)
-   [新架构文档](https://reactnative.dev/architecture/overview?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)
-   能够在React-Native 0.68中轻松启用新架构 -- 即将推出
-   第三方库的转换
-   默认启用Hermes引擎

[**Solito**](https://github.com/nandorojo/solito?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)

Fernando Rojo经常推动跨平台领域的创新（也见[Moti](https://moti.fyi/?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)和[Dripsy](https://www.dripsy.xyz/?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)）。Solito通过提供React-Navigation和Next.js之间共享的导航基础，使网络和移动之间共享更多的代码成为可能。他在这方面已经工作了一段时间了，这不是第一次迭代。它还提供了一个 [monorepo的例子](https://github.com/nandorojo/solito/tree/master/example-monorepos/blank?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)来让你快速入门。

[**Flutter is better than React Native***](https://shift.infinite.red/flutter-is-better-than-react-native-fed10c92a768?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)

*...在所有不重要的方面 😄

Jamon意识到Flutter在很多方面都很好（DX、CLI、e2e测试、升级、性能...）。他很公平地介绍了两个框架的利弊。没有明显的赢家。在一些重要的方面，Flutter很难与之竞争：网络支持、共享代码和知识，以及招聘规模。

[**Flutter Web vs HTML, CSS & JS: Performance Comparison**](https://codewithandrea.com/videos/flutter-web-html-css-js-performance-comparison/?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)

对于React-Native开发者来说，这很有趣（也和上面的文章有关），因为它强调了其竞争对手Flutter在支持网络方面的局限性（React-Native-Web在这方面运作良好à）。对于内容网站来说，Flutter web不是一个好的选择，但对于较重的web应用来说，仍然是一个好的解决方案。请注意，React-Native-Skia在网络上也会有类似的权衡。

**拓展阅读:**

-   📜 [Avoid Keyboard in React Native Like a Pro](https://www.netguru.com/blog/avoid-keyboard-react-native?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter): 非常详细的资源，用gif图片记录了iOS和Android在几个生态系统库管理虚拟键盘的行为：这显然不是React-Native最简单的部分。 😅
-   🧑‍🎨 React-Native-Skia: [inner shadows](https://twitter.com/wcandillon/status/1503015924932218884?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter), [animations](https://twitter.com/chrfalch/status/1501213385253429258?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)
-   🎥 [React-Native-Skia with Christian Falch & Jamon Holmgren](https://www.youtube.com/watch?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter&v=56PRggTDcAY)
-   📦 [React-Native-Performance](https://twitter.com/almouro/status/1501550641843429377?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter): now supports iOS
-   📦 [React-Native TVOS 0.66.3-2](https://twitter.com/douglowder/status/1502484616497688582?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter): Fabric support for Apple TV
-   📦 [React-Native-Gesture-Handler 2.3](https://twitter.com/swmansion/status/1503748969201127429?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter): Fabric support
-   🧵 [What's next in React Native?](https://twitter.com/axeldelafosse/status/1503327627133829127?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)

## 其它

[**A Proposal For Type Syntax in JavaScript**](https://devblogs.microsoft.com/typescript/a-proposal-for-type-syntax-in-javascript/?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)

😱 微软正在进行一项 [TC39提案](https://github.com/giltayar/proposal-types-as-comments/?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)（第0阶段），在TypeScript的启发下，为JavaScript语言语法带来类型注释（没有`enums`, `namespaces` 等）。

浏览器将简单地忽略这些类型注释，不做任何类型检查，所以TypeScript（或其他类型检查器）仍然需要。

这在开发中很有意思：我们可以直接执行TypeScript代码，而不需要在浏览器中进行任何转换。在生产中，我们会继续捆绑代码，因为最小化和删除类型仍然有用（见[Ryan Cavanaugh对最小化的比喻](https://twitter.com/SeaRyanC/status/1501645753730560000?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)）。

也请看专门的 [提案网站](https://giltayar.github.io/proposal-types-as-comments/?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)。

**拓展阅读:**

-   [New WebKit Features in Safari 15.4](https://webkit.org/blog/12445/new-webkit-features-in-safari-15-4/?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter): [一批新的功能 ](https://twitter.com/jensimmons/status/1503454398487408640?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)! 现在许多功能在主流的浏览器中都可用，后续将逐渐在生产中使用（如CSS容器查询🙌）。
-   [Tao of Node - Design, Architecture & Best Practices](https://alexkondov.com/tao-of-node/?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter): 在流行的[Tao of React](https://alexkondov.com/tao-of-react/?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)之后，Alex分享了他在开发Node.js应用程序时遵循的原则的清单。
-   [A Complete Guide To TypeScript's Never Type](https://www.zhenghao.io/posts/ts-never?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter): 完整关于TypeScript底层类型`never`的文章
-   [twitter-api-typescript-sdk](https://github.com/twitterdev/twitter-api-typescript-sdk?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter): 终于有了一个官方的SDK
-   [CSS: @when or @if](https://meyerweb.com/eric/thoughts/2022/03/14/if-or-when/?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)
-   [SWC v1.2.154](https://twitter.com/swc_rs/status/1502622757271441417?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter): minifier perf improvements
-   [Vite 2.9 beta](https://twitter.com/stackblitz/status/1503379677456523266?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter): much faster cold starts
-   [pnpm-7.0.0-beta.0](https://github.com/pnpm/pnpm/releases/tag/v7.0.0-beta.0?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)
-   [TypeScript PR - Optional variance annotations](https://github.com/microsoft/TypeScript/pull/48240?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)
-   [TypeScript: optional vs. undefined](https://tkdodo.eu/blog/optional-vs-undefined?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)
-   [StackBlitz February 2022 Update](https://blog.stackblitz.com/posts/update-2022-02/?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)
-   [StackBlitz has joined the Bytecode Alliance](https://blog.stackblitz.com/posts/bytecode-alliance/?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)
-   [Front-end Testing Strategy](https://itnext.io/front-end-testing-strategy-5fddfd463feb?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)
-   [What's New In DevTools (Chrome 100)](https://twitter.com/ChromeDevTools/status/1501932135988568064?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)
-   [What Is Vitest?](https://www.youtube.com/watch?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter&v=5ddeTxyfgcE)
-   [Turborepo Demo (Remote Caching & Deploying to Vercel)](https://www.youtube.com/watch?t=1s&utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter&v=_sB2E1XnzOY)
-   [How Storybook helps designers & developers stay in sync](https://storybook.js.org/blog/how-storybook-helps-designers-developers-stay-in-sync/?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)
-   [A look at the dialog element's super powers](https://www.stefanjudis.com/blog/a-look-at-the-dialog-elements-super-powers/?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)
-   [Aligning Content In Different Wrappers](https://ishadeed.com/article/aligning-content-different-wrappers/?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)
-   [GraphQL error handling to the max with Typescript, codegen and fp-ts](https://www.the-guild.dev/blog/graphql-error-handling-with-fp?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)
-   [Typescript Tuples, and how they work](https://fjolt.com/article/typescript-tuples?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)
-   [How to use Google Analytics in Deno Deploy](https://deno.com/blog/ga-with-deno-deploy?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)
-   [Partytown 0.5](https://twitter.com/Steve8708/status/1502306419151757316?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)


<img width="694" alt="image" src="https://user-images.githubusercontent.com/749374/158568305-8bb27548-cef3-480a-827a-d949d49711fb.png">

 
