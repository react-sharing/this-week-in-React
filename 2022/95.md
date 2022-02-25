
## React

[**React 18: onRecoverableError**](https://github.com/facebook/react/pull/23207?utm_campaign=thisweekinreact&utm_medium=email&utm_source=Revue%20newsletter)

A React 18 RC1 should be released this week, announced by Andrew Clark: [*"Small update on React 18: we're planning another RC for next week that includes improvements to error reporting"*](https://twitter.com/acdlite/status/1494753034806579200?utm_campaign=thisweekinreact&utm_medium=email&utm_source=Revue%20newsletter)

It ships with a new API `onRecoverableError`. The idea is to be able to log/report (via [`reportError`](https://www.stefanjudis.com/blog/reporterror-a-method-to-report-to-global-event-handlers/?utm_campaign=thisweekinreact&utm_medium=email&utm_source=Revue%20newsletter)) the "recoverable errors" that might happen in React, notably during the hydration process when there are some mismatches between SSR and CSR.

[**Next.js 12.1**](https://nextjs.org/blog/next-12-1?utm_campaign=thisweekinreact&utm_medium=email&utm_source=Revue%20newsletter)

Nice release including one of the most highly anticipated feature: on-demand Incremental Static Regeneration (ISR). A new API `unstable_revalidate("/static-page-url")` should significantly help for CMS integration: as you can now get an immediate update on CMS publish.

On SWC side: 6 new Babel plugins ported to Rust (including Styled-Components and Relay), SWC minify in release-candidate and a better zero-config integration with Jest

There's also some notable progress on React 18 and Server Components support, but it's still in alpha.

See also the [introduction video from Lee](https://www.youtube.com/watch?utm_campaign=thisweekinreact&utm_medium=email&utm_source=Revue%20newsletter&v=BGexHR1tuOA) or the [on-demand ISR demo from Delba](https://twitter.com/delba_oliveira/status/1494447518733717512?utm_campaign=thisweekinreact&utm_medium=email&utm_source=Revue%20newsletter).

[**Remix 1.2**](https://github.com/remix-run/remix/releases/tag/v1.2.0?utm_campaign=thisweekinreact&utm_medium=email&utm_source=Revue%20newsletter)

An interesting release on the deployment part: new `serverBuildTarget` option to configure the build (directory, module format), possibility to build the server in a single output file, and a new experimental adapter to deploy on Deno.

[**The React.ReactNode type is a black hole**](https://changelog.com/posts/the-react-reactnode-type-is-a-black-hole?utm_campaign=thisweekinreact&utm_medium=email&utm_source=Revue%20newsletter)

Widely known problem for a long time, the TypeScript type for `ReactNode` is too loose and does not permit to catch some errors at compile time. Kevin suggests to create a `StrictReactNode` type and provides an ESLint rule to forbid the usage of `ReactNode`. [Similar article](https://fettblog.eu/react-types-for-children-are-broken/?utm_campaign=thisweekinreact&utm_medium=email&utm_source=Revue%20newsletter).

**Extras:**

-   📜 [Putting test files in the pages folder in a Next.js app](https://www.benmvp.com/blog/putting-test-files-pages-folder-nextjs-app/?utm_campaign=thisweekinreact&utm_medium=email&utm_source=Revue%20newsletter): useful Next.js trick if you want to co-locate stories and tests alongside Next.js pages: the `pageExtensions` config
-   📜 [Deep dive into React keys bugs](https://dev.to/kozlovzxc/deep-dive-into-react-keys-bugs-1351?utm_campaign=thisweekinreact&utm_medium=email&utm_source=Revue%20newsletter): explains various problems related to the `key` props and suggest solutions
-   📦 [React-Runner](https://github.com/nihgwu/react-runner?utm_campaign=thisweekinreact&utm_medium=email&utm_source=Revue%20newsletter): new modern alternative to [React-Live](https://github.com/FormidableLabs/react-live?utm_campaign=thisweekinreact&utm_medium=email&utm_source=Revue%20newsletter) to provide live editor + preview, based on Sucrase instead of Bublé. This is promising and could eventually be adopted by both the [new React docs](https://github.com/reactjs/reactjs.org/pull/4339?utm_campaign=thisweekinreact&utm_medium=email&utm_source=Revue%20newsletter) and [Docusaurus](https://github.com/facebook/docusaurus/pull/6589?utm_campaign=thisweekinreact&utm_medium=email&utm_source=Revue%20newsletter).
-   📦 [Tunnel-Rat](https://github.com/pmndrs/tunnel-rat?utm_campaign=thisweekinreact&utm_medium=email&utm_source=Revue%20newsletter): new Poimandres lib based on Zustand, to create a "React tunnel" and teleport JSX from one tree to another. See also [React-Teleporter](https://github.com/gregberge/react-teleporter?utm_campaign=thisweekinreact&utm_medium=email&utm_source=Revue%20newsletter).
-   🔗 [Nextjs-blog-theme](https://www.netlify.com/blog/a-beautiful-bejamas-blog-template-with-next.js-on-netlify?utm_campaign=thisweekinreact&utm_medium=email&utm_source=Revue%20newsletter): Next.js + Tailwind blog template provided by Netlify/Bejamas
-   💬 Mark Erikson: ["when/why should I use Context, Hooks, Thunks, Sagas, React Query, RTK Query?"](https://www.reddit.com/r/reactjs/comments/svzgnu/clarifying_advice_on_strategizing_use_of/hxk9bem/?utm_campaign=thisweekinreact&utm_medium=email&utm_source=Revue%20newsletter)
-   📖 [Migrating to React Query 4](https://react-query-alpha.tanstack.com/guides/migrating-to-react-query-4?utm_campaign=thisweekinreact&utm_medium=email&utm_source=Revue%20newsletter)
-   🧵 [React Server Components, Vizualized](https://twitter.com/Steve8708/status/1494355779897364481?utm_campaign=thisweekinreact&utm_medium=email&utm_source=Revue%20newsletter)

## React-Native

[**Introducing Fabric to react-native-screens**](https://blog.swmansion.com/introducing-fabric-to-react-native-screens-fd17bf18858e?utm_campaign=thisweekinreact&utm_medium=email&utm_source=Revue%20newsletter)

With React-Native 0.68, we can easily activate the new Fabric renderer! But it will only work if all your libs are compatible.

Software Mansion announces its commitment to making its libs compatible with Fabric (starting with React-Native-Screens).

They encourage us to do the same and give us some leads (process and PRs). The idea: create libs that work as well with both the new and the old architecture at the same time, to allow an incremental migration, but without duplicating too much code.

This is very exciting, and the community provides some feedback:

-   [significant impact on memory consumption](https://twitter.com/hanno_jg/status/1494593974144806914?utm_campaign=thisweekinreact&utm_medium=email&utm_source=Revue%20newsletter)
-   [demo animated header 60 FPS](https://twitter.com/aarongrider/status/1494493944754827271?utm_campaign=thisweekinreact&utm_medium=email&utm_source=Revue%20newsletter)

Note that [React-Navigation already works under Fabric with react-native-screens](https://twitter.com/kzzzf/status/1494324980011569153?utm_campaign=thisweekinreact&utm_medium=email&utm_source=Revue%20newsletter)!

[**Flipper is coming to your web and Node.js apps**](https://fbflipper.com/blog/2022/02/21/js-flipper-announcement/?utm_campaign=thisweekinreact&utm_medium=email&utm_source=Revue%20newsletter)

[Flipper](https://fbflipper.com/?utm_campaign=thisweekinreact&utm_medium=email&utm_source=Revue%20newsletter) is initially a desktop DevTool for React-Native, permitting you to inspect logs, network requests... Andrey introduces [js-flipper](https://www.npmjs.com/package/js-flipper?utm_campaign=thisweekinreact&utm_medium=email&utm_source=Revue%20newsletter): a package that permits to integrate Flipper with web or Node.js apps ([React example](https://github.com/facebook/flipper/tree/main/js/react-flipper-example/src?utm_campaign=thisweekinreact&utm_medium=email&utm_source=Revue%20newsletter)). He shares various use-cases at Meta: mobile, web, Node.js, Desktop, Oculus Quest... there are also app-specific business use-cases such as a plugin providing a "log as user X" feature.

Flipper seems to be an ideal platform to build a universal DevTool, provided the ecosystem follows, so Andrey invites us all to create plugins.

**Extras:**

-   📜 [Security of React Native libraries: the bad, the worse and the ugly](https://www.cossacklabs.com/blog/react-native-libraries-security/?utm_campaign=thisweekinreact&utm_medium=email&utm_source=Revue%20newsletter): a fairly advanced security audit that criticizes a lot of crypto libs in React-Native. The company suggest to use [Themis](https://github.com/cossacklabs/themis?utm_campaign=thisweekinreact&utm_medium=email&utm_source=Revue%20newsletter), a cross-platform crypto library (React-Native API in beta) that encourages crypto good practices without being a crypto expert.
-   📜 [Expo 101: Building mobile apps in weeks, not years](https://dev.to/mauro_codes/expo-101-building-mobile-apps-in-weeks-not-years-aj1?utm_campaign=thisweekinreact&utm_medium=email&utm_source=Revue%20newsletter): nice overview of the whole modern Expo ecosystem based on AES. They provide a tool for each stage of our mobile projects.
-   📜 [Better Credentials Management with Expo Application Services](https://blog.expo.dev/better-credentials-management-with-expo-application-services-177ca1755f38?utm_campaign=thisweekinreact&utm_medium=email&utm_source=Revue%20newsletter)
-   📜 [Build a React Native QR Code Scanner using Vision Camera](https://www.dynamsoft.com/codepool/react-native-qr-code-scanner-vision-camera.html?utm_campaign=thisweekinreact&utm_medium=email&utm_source=Revue%20newsletter)
-   📦 [vision-camera-ocr](https://github.com/aarongrider/vision-camera-ocr?utm_campaign=thisweekinreact&utm_medium=email&utm_source=Revue%20newsletter): real-time OCR frame-processor!
-   📦 [react-native-safe-area-context v4 RC](https://github.com/th3rdwave/react-native-safe-area-context/releases/tag/v4.0.1-rc.0?utm_campaign=thisweekinreact&utm_medium=email&utm_source=Revue%20newsletter): Fabric support, backward compatible. [Looking for early adopter feedback](https://twitter.com/janicduplessis/status/1494731240624345092?utm_campaign=thisweekinreact&utm_medium=email&utm_source=Revue%20newsletter)
-   📦 [react-native-url-router](https://github.com/software-mansion-labs/react-native-url-router?utm_campaign=thisweekinreact&utm_medium=email&utm_source=Revue%20newsletter) + [overview](https://software-mansion-labs.github.io/react-native-url-router/docs/overview?utm_campaign=thisweekinreact&utm_medium=email&utm_source=Revue%20newsletter)
-   🎨 [Demo graph React-Native-Skia](https://twitter.com/mrousavy/status/1494658946547830785?utm_campaign=thisweekinreact&utm_medium=email&utm_source=Revue%20newsletter): more performant than SVG

## Other

[**State Of JS 2021**](https://2021.stateofjs.com/en-US/?utm_campaign=thisweekinreact&utm_medium=email&utm_source=Revue%20newsletter)

Unsurprisingly, React remains very popular this year, but it is surpassed by Svelte and Solid in terms of satisfaction. Next.js and Remix both at 91% satisfaction. Read in particular [Swyx's conclusion](https://www.swyx.io/state-of-js-2021/?utm_campaign=thisweekinreact&utm_medium=email&utm_source=Revue%20newsletter). A [livestream](https://dev.to/sachagreif/state-of-javascript-2021-livestream-24a5?utm_campaign=thisweekinreact&utm_medium=email&utm_source=Revue%20newsletter) is taking place today.

Remember this survey is not [without](https://twitter.com/threepointone/status/1483479895984545798?utm_campaign=thisweekinreact&utm_medium=email&utm_source=Revue%20newsletter) [bias](https://twitter.com/youyuxi/status/1493927355399606273?utm_campaign=thisweekinreact&utm_medium=email&utm_source=Revue%20newsletter), but it remains interesting to explore trends. Sacha Grief is of goodwill to improve and [addresses the criticisms on Dev](https://dev.to/sachagreif?utm_campaign=thisweekinreact&utm_medium=email&utm_source=Revue%20newsletter).

**Extras:**

-   [Rebuilding Babel: The Tokenizer](https://www.nan.fyi/tokenizer?utm_campaign=thisweekinreact&utm_medium=email&utm_source=Revue%20newsletter): great interactive article, perfect to learn what is a tokenizer
-   [Express 5.0](https://github.com/expressjs/express/releases/tag/v5.0.0-beta.1?utm_campaign=thisweekinreact&utm_medium=email&utm_source=Revue%20newsletter): first beta after a long time 😅 in the meantime it's modern contender Fastify tops the State of JS and released [v4.0.0-alpha.1](https://github.com/fastify/fastify/releases/tag/v4.0.0-alpha.1?utm_campaign=thisweekinreact&utm_medium=email&utm_source=Revue%20newsletter)
-   [GitHub Actions: `concurrency.cancel-in-progress`](https://twitter.com/sebastienlorber/status/1495776331287646209?utm_campaign=thisweekinreact&utm_medium=email&utm_source=Revue%20newsletter): useful to optimize your CI
-   [Node.js: `AbortSignal.timeout()`](https://twitter.com/simonplend/status/1494309000824954882?utm_campaign=thisweekinreact&utm_medium=email&utm_source=Revue%20newsletter)`: new API
-   [new.target](https://twitter.com/matteocollina/status/1494620426034688001?utm_campaign=thisweekinreact&utm_medium=email&utm_source=Revue%20newsletter): TIL, permits to know if a function was called with `new`, faster than `instanceof`
-   [CSS Container Queries](https://twitter.com/bramus/status/1494363331959922695?utm_campaign=thisweekinreact&utm_medium=email&utm_source=Revue%20newsletter): enabled by default in WebKit
-   [New Google Cloud Functions](https://cloud.google.com/blog/products/serverless/introducing-the-next-generation-of-cloud-functions?utm_campaign=thisweekinreact&utm_medium=email&utm_source=Revue%20newsletter): 60min execution time!
-   [Cross-Browser support with Cross-Origin isolation](https://blog.stackblitz.com/posts/cross-browser-with-coop-coep/?utm_campaign=thisweekinreact&utm_medium=email&utm_source=Revue%20newsletter): explains why StackBlitz WebContainers only work in Chromium
-   [Create your Chrome Extension using Flutter web](https://medium.com/flutter-students-club/create-your-chrome-extension-using-flutter-79712ffcb439?utm_campaign=thisweekinreact&utm_medium=email&utm_source=Revue%20newsletter): 🤔 this use-case is interesting: an extension doesn't need SEO
-   [TypeScript - Implement Rust-style Result](https://www.huy.rocks/everyday/02-14-2022-typescript-implement-rust-style-result?utm_campaign=thisweekinreact&utm_medium=email&utm_source=Revue%20newsletter): reminds the Either FP type
-   [Netlify Graph](https://www.netlify.com/blog/announcing-netlify-graph-a-faster-way-for-teams-to-develop-web-apps-with-apis?utm_campaign=thisweekinreact&utm_medium=email&utm_source=Revue%20newsletter): new Netlify service after acquiring OneGraph: a unified GraphQL API targeting lots of other third-party APIs
-   [Node.js Trademarks Transferred to OpenJS Foundation](https://openjsf.org/blog/2022/02/14/node-js-trademarks-transferred-to-openjs-foundation/?utm_campaign=thisweekinreact&utm_medium=email&utm_source=Revue%20newsletter): that would be nice if [Oracle also transferred its JavaScript trademarks](https://twitter.com/rauschma/status/1494987550250913792?utm_campaign=thisweekinreact&utm_medium=email&utm_source=Revue%20newsletter) 😅
-   [Don't trust JS library size, min+gzip](https://thoughtspile.github.io/2022/02/15/bundle-size-lies/?utm_campaign=thisweekinreact&utm_medium=email&utm_source=Revue%20newsletter)
-   [Yarn 3.2: Libc, Yarn Explain, Next Major, ...](https://dev.to/arcanis/yarn-32-libc-yarn-explain-next-major--o22?utm_campaign=thisweekinreact&utm_medium=email&utm_source=Revue%20newsletter)
-   [Testing Vite with minimal config using Vitest](https://blog.logrocket.com/testing-vite-minimal-config-using-vitest/?utm_campaign=thisweekinreact&utm_medium=email&utm_source=Revue%20newsletter)
-   [SolidJS sponsored by Vercel](https://twitter.com/solid_js/status/1495792685977948166?utm_campaign=thisweekinreact&utm_medium=email&utm_source=Revue%20newsletter)
-   [The Story of Asynchronous JavaScript](https://www.youtube.com/watch?utm_campaign=thisweekinreact&utm_medium=email&utm_source=Revue%20newsletter&v=rivBfgaEyWQ)
-   [*"TIL you can write overloads for arrow functions in TypeScript"*](https://twitter.com/steveruizok/status/1495328409613918210?utm_campaign=thisweekinreact&utm_medium=email&utm_source=Revue%20newsletter)
-   [You Can throw() Anything In JavaScript - And Other async/await Considerations](https://www.bennadel.com/blog/4210-you-can-throw-anything-in-javascript-and-other-async-await-considerations.htm?utm_campaign=thisweekinreact&utm_medium=email&utm_source=Revue%20newsletter)
-   [Exploring model-based testing for UIs](https://jlongster.com/exploring-model-based-testing?utm_campaign=thisweekinreact&utm_medium=email&utm_source=Revue%20newsletter)
-   [A Complete Guide to CSS Cascade Layers](https://css-tricks.com/css-cascade-layers/?utm_campaign=thisweekinreact&utm_medium=email&utm_source=Revue%20newsletter)
-   [Resumable JavaScript with Qwik](https://dev.to/this-is-learning/resumable-javascript-with-qwik-2i29?utm_campaign=thisweekinreact&utm_medium=email&utm_source=Revue%20newsletter)
-   [Deno 1.19](https://deno.com/blog/v1.19?utm_campaign=thisweekinreact&utm_medium=email&utm_source=Revue%20newsletter)
-   [An Introduction to Deno: Is It Better than Node.js?](https://blog.appsignal.com/2022/02/09/an-introduction-to-deno-is-it-better-than-nodejs.html?utm_campaign=thisweekinreact&utm_medium=email&utm_source=Revue%20newsletter)
-   [Survivorship Bias in Web Performance](https://simonhearne.com/2022/survorship-bias-in-webperf/?utm_campaign=thisweekinreact&utm_medium=email&utm_source=Revue%20newsletter)
-   [Hasura: Announcing our $100M Series C funding](https://hasura.io/blog/seriesc-100m-graphql-for-everyone/?utm_campaign=thisweekinreact&utm_medium=email&utm_source=Revue%20newsletter)
-   [Rome: *"A sneak peak of our formatter: being able to format partial broken code!"*](https://twitter.com/rometools/status/1493584158475665411?utm_campaign=thisweekinreact&utm_medium=email&utm_source=Revue%20newsletter)
-   [Injecting backdoors to NPM packages](https://dev.to/kozlovzxc/injecting-backdoors-to-npm-packages-a0k?utm_campaign=thisweekinreact&utm_medium=email&utm_source=Revue%20newsletter)
-   [How to Favicon in 2022: Six files that fit most needs](https://evilmartians.com/chronicles/how-to-favicon-in-2021-six-files-that-fit-most-needs?utm_campaign=thisweekinreact&utm_medium=email&utm_source=Revue%20newsletter)
-   [tooling.one: collection of useful dev tools](https://tooling.one/?utm_campaign=thisweekinreact&utm_medium=email&utm_source=Revue%20newsletter)
-   [Four reasons why WebdriverIO is better than Cypress](https://hughmccamphill.com/four-reasons-why-webdriverio-is-better-than-cypress?utm_campaign=thisweekinreact&utm_medium=email&utm_source=Revue%20newsletter)
-   [Measuring user flow performance with Lighthouse and WebdriverIO](https://hughmccamphill.com/measuring-user-flow-performance-with-lighthouse-and-webdriverio?utm_campaign=thisweekinreact&utm_medium=email&utm_source=Revue%20newsletter)
-   [*"In @ChromeDevTools holding SHIFT while moving mouse over resources in network panel shows you which asset caused to load another asset."*](https://twitter.com/coderitual/status/1088194261454127104?utm_campaign=thisweekinreact&utm_medium=email&utm_source=Revue%20newsletter)
-   [XState -> Mermaid converted?](https://twitter.com/farzad_yz/status/1495803623707713551?utm_campaign=thisweekinreact&utm_medium=email&utm_source=Revue%20newsletter)

 <img width="915" alt="image" src="https://user-images.githubusercontent.com/749374/155195798-d69e9965-bbb4-487f-8301-4592624b086f.png">
