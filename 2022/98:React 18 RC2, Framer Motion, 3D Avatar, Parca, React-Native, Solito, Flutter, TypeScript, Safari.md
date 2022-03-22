This Week In React #98: React 18 RC2, Framer Motion, 3D Avatar, Parca, React-Native, Solito, Flutter, TypeScript, Safari...


## React

[**How to Upgrade to the React 18 Release Candidate**](https://reactjs.org/blog/2022/03/08/react-18-upgrade-guide.html?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)

[React 18.0.0-rc.2](https://www.npmjs.com/package/react?activeTab=versions&utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter) has just been released (under npm tag `@rc`). The React team published a blog post (+ 🧵 [thread](https://twitter.com/reactjs/status/1501258790666178563?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)) to prepare us for the arrival of this new version. It includes the new concurrent features, which we can adopt incrementally.

They encourage us to test the release-candidate to detect the latest potential bugs, and offer a fairly complete upgrade guide by documenting the main api and behavioral changes. There is also a brief presentation of various new APIs.

Read this post directly, it contains many interesting details. Personally I discovered the concept of [Strict Effects](https://github.com/reactwg/react-18/discussions/19?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter) and that[ composants are now allowed to render undefined](https://twitter.com/sebastienlorber/status/1501590568597610503?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter).

[**Delightful React File/Directory Structure**](https://www.joshwcomeau.com/react/file-structure/?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)

Interactive article by Josh Comeau on his file-system structure choices to organize a React app. Strong opinion: he explains in particular why he prefers to group files by type rather than by feature. I don't necessarily agree with everything, but it's still an interesting read and has some good arguments.

[**Everything about Framer Motion layout animations**](https://blog.maximeheckel.com/posts/framer-motion-layout-animations/?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)

Interactive article that presents layout animations with Framer Motion. Very well presented, with many examples. I really liked the example of Tabs with a shared layout animation: the API is quite intuitive, I didn't know it was that easy.

**Extras:**

-   📜 [How to Use Three.js And React to Render a 3D Model of Your Self](https://blog.nourdinedev.com/how-to-use-three.js-and-react-to-render-a-3d-model/?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter): original article that proposes to create your own personal 3D avatar, display it with React-Three-Fiber and make it do some breakdance 😄 I really want to test that.
-   📜 [Profiling Next.js apps with Parca](https://www.polarsignals.com/blog/posts/2022/03/02/profiling-nextjs-app-with-parca/?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter): first time I hear about Parca. This seems to be an interesting continuous profiling tool for those who self-host their Node.js apps (with Kubernetes for example) but might also be handy to profile performance problems locally. In this example, the tool detects a performance problem related to the unnecessary use of immutability.
-   📜 [Why Did And Don't You Need To Import React](https://www.chakshunyu.com/blog/why-did-and-dont-you-need-to-import-react/?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)
-   📜 [Automatic batching support in React 18](https://www.dtreelabs.com/blog/automatic-batching-support-in-react-18?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)
-   📜 [What it's like to migrate a high-traffic website from Gatsby to Next.js](https://mikebifulco.com/posts/migrate-gatsby-to-nextjs-apisyouwonthate-com?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)
-   [🧑‍🎓](https://emojikeyboard.org/copy/Student_Emoji_%F0%9F%A7%91%E2%80%8D%F0%9F%8E%93?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=extlink) [Learn Next.js foundations](https://twitter.com/vercel/status/1503407398534500352?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter): new resource offered by Vercel for beginners who want to build strong foundations before diving in Next.js: assume you may not know React
-   👥 [Xuan Huang](https://twitter.com/Huxpro/status/1502483206569807874?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter): new React core team member, notably working on [React-Forget](https://www.youtube.com/watch?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter&v=lGEMwh32soc)
-   👥 [Remix Conf Speakers](https://twitter.com/remix_run/status/1503400608165892098?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter) have been announced
-   🎙️ [Remix Podcast - Season 1](https://twitter.com/remix_run/status/1501716370831994885?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter): 12 episodes released
-   🐦 Malte Ubi: [*"JSX should be part of JavaScript"*](https://twitter.com/cramforce/status/1485778298042945540?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter) & Nicole Sullivan: [*"YES! But JSX is not enough on its own. Let me explain..."*](https://twitter.com/stubbornella/status/1502724909184679939?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)
-   🐦 [form attribute](https://twitter.com/sebastienlorber/status/1503428181134557185?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter), [formAction](https://twitter.com/ryanflorence/status/1502349821054644225?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter): web APIs that we (I) discover using Remix 🤯
-   🐦 [SolidJS signals in React](https://twitter.com/tannerlinsley/status/1502116674689925123?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter) + [Preact/reactive addon](https://github.com/preactjs/preact/pull/3474?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter): several experiments around reactivity
-   🎥 [Basic React To Svelte Conversion](https://www.youtube.com/watch?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter&v=DiSuwLlhOxs)
-   🎥 [React Query in 100 Seconds](https://www.youtube.com/watch?t=1s&utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter&v=novnyCaa7To)

## React-Native

[**An update on the New Architecture Rollout**](https://reactnative.dev/blog/2022/03/15/an-update-on-the-new-architecture-rollout?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)

Nicola reminds that the new architecture is coming, and presents the different initiatives to prepare the community:

-   The [working group](https://github.com/reactwg/react-native-new-architecture?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)
-   The [migration guide](https://reactnative.dev/docs/next/new-architecture-intro?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)
-   The [new architecture doc](https://reactnative.dev/architecture/overview?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)
-   The ability to easily enable the new architecture in React-Native 0.68 - coming soon
-   Conversion of third-party libs
-   The Hermes engine enabled by default

[**Solito**](https://github.com/nandorojo/solito?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)

Fernando Rojo regularly pushes innovation in the field of cross-platform (see also [Moti](https://moti.fyi/?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter) and [Dripsy](https://www.dripsy.xyz/?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)). Solito makes it possible to share even more code between web and mobile by offering navigation primitives shared between React-Navigation and Next.js. He's been working on this for a while, it's not the first iteration. It also offers a [monorepo example](https://github.com/nandorojo/solito/tree/master/example-monorepos/blank?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter) to get you started fast.

[**Flutter is better than React Native***](https://shift.infinite.red/flutter-is-better-than-react-native-fed10c92a768?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)

*...in all the ways that don't matter 😄

Jamon recognizes that Flutter is good on many aspects (DX, CLI, e2e tests, upgrades, performance...). He presents the tradeoffs of both frameworks quite fairly. There is no clear winner. Some important points on which Flutter can hardly compete: web support, sharing code and knowledge, and the ability to hire.

[**Flutter Web vs HTML, CSS & JS: Performance Comparison**](https://codewithandrea.com/videos/flutter-web-html-css-js-performance-comparison/?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)

Interesting for a React-Native dev (and also related to the article above) because it highlights the limits of its competitor Flutter to support the web (where React-Native-Web works wellà). Flutter web is not a good choice for content sites, but can remain a good solution for heavier web apps. Note that React-Native-Skia on the web will have similar tradeoffs.

**Extras:**

-   📜 [Avoid Keyboard in React Native Like a Pro](https://www.netguru.com/blog/avoid-keyboard-react-native?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter): exhaustive resource that documents with gifs the iOS and Android behavior of several ecosystem libs to manage the virtual keyboard: this is clearly not the easiest part of React-Native 😅
-   🧑‍🎨 React-Native-Skia: [inner shadows](https://twitter.com/wcandillon/status/1503015924932218884?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter), [animations](https://twitter.com/chrfalch/status/1501213385253429258?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)
-   🎥 [React-Native-Skia with Christian Falch & Jamon Holmgren](https://www.youtube.com/watch?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter&v=56PRggTDcAY)
-   📦 [React-Native-Performance](https://twitter.com/almouro/status/1501550641843429377?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter): now supports iOS
-   📦 [React-Native TVOS 0.66.3-2](https://twitter.com/douglowder/status/1502484616497688582?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter): Fabric support for Apple TV
-   📦 [React-Native-Gesture-Handler 2.3](https://twitter.com/swmansion/status/1503748969201127429?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter): Fabric support
-   🧵 [What's next in React Native?](https://twitter.com/axeldelafosse/status/1503327627133829127?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)

## Other

[**A Proposal For Type Syntax in JavaScript**](https://devblogs.microsoft.com/typescript/a-proposal-for-type-syntax-in-javascript/?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)

😱 Microsoft is working on a [TC39 proposal](https://github.com/giltayar/proposal-types-as-comments/?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter) (stage-0) to bring type annotations to the JavaScript language syntax, inspired by TypeScript (without `enums`, `namespaces` etc...).

The browser would simply ignore those type annotations and not do any type-checking, so TypeScript (or other type-checkers) remains relevant.

This is interesting in development: we can directly execute TypeScript code without any transformation in the browser. In production, we would continue to bundle the code, because minifying and removing types remains useful (see [Ryan Cavanaugh's analogy with minification](https://twitter.com/SeaRyanC/status/1501645753730560000?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)).

See also the dedicated [proposal website](https://giltayar.github.io/proposal-types-as-comments/?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter).

**Extras:**

-   [New WebKit Features in Safari 15.4](https://webkit.org/blog/12445/new-webkit-features-in-safari-15-4/?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter): a [bunch of new features](https://twitter.com/jensimmons/status/1503454398487408640?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)! Many are now available in all major browsers and will therefore gradually become usable in production (like CSS Container queries 🙌).
-   [Tao of Node - Design, Architecture & Best Practices](https://alexkondov.com/tao-of-node/?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter): after his popular [Tao of React](https://alexkondov.com/tao-of-react/?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter), Alex shared an exhaustive list of principes he follows when developing Node.js apps.
-   [A Complete Guide To TypeScript's Never Type](https://www.zhenghao.io/posts/ts-never?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter): complete article on the TypeScript bottom-type `never`
-   [twitter-api-typescript-sdk](https://github.com/twitterdev/twitter-api-typescript-sdk?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter): finally an officiel SDK
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

 
