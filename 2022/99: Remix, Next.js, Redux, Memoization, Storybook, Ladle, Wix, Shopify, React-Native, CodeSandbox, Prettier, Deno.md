This Week In React #99: Remix, Next.js, Redux, Memoization, Storybook, Ladle, Wix, Shopify, React-Native, CodeSandbox, Prettier, Deno...


## React


[**Ladle - A drop-in alternative to Storybook**](https://www.ladle.dev/blog/introducing-ladle/?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)

Ladle is a project from an Uber engineer who loves Storybook but still sees various performance issues within his company: build time, startup time, Time-To-Interactive... So he created a much faster alternative , based on Vite and ES modules, and compatible with the [Component Story Format](https://storybook.js.org/docs/react/api/csf?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter) to make adoption easy ([demo](https://baseweb.netlify.app/?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)).

[**Preemptive Memoization In React Is Probably Not Evil**](https://www.zhenghao.io/posts/memo-or-not?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)

A very interesting and well-documented article on the stability of objects and callbacks. Despite the fact that the use of `useMemo` may look like a premature optimization, Zhenghao recommends stabilizing identities as much as possible, at least for libs and custom hooks. We look forward to [React-Forget](https://www.youtube.com/watch?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter&v=lGEMwh32soc) and [Records & Tuples](https://sebastienlorber.com/records-and-tuples-for-react?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter) which could greatly simplify our lives.

[**Remix Stacks**](https://remix.run/blog/remix-stacks?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)** & **[**Remix v1.3**](https://github.com/remix-run/remix/releases/tag/v1.3.0?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)

The Remix CLI now allows you to initialize a project with a given stack. Remix offers 3 built-in stacks to get started very fast (DB, auth, host, tests...), and it is possible to create your own stack (for your company projects for example). On the 3 stacks available, the difference is mainly on hosting or persistence, and we find in common base: Tailwind, TypeScript, Prettier, ESLint, Cypress, MSW, Docker, Vitest, Testing Library.

I find it good to provide starters to get started quickly, but I have mixed feelings about the "template" approach, I prefer the ["company-scripts"](https://kentcdodds.com/blog/tools-without-config?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter) approach (like CRA) that Kent previously advocated for, to reduce the maintenance of existing projects over time.

[**Upgrading Next.js for instant performance improvements**](https://vercel.com/blog/upgrading-nextjs-for-instant-performance-improvements?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)

Vercel recently upgraded a demo app ([Virtual Reality Store](https://serverless-vrs.vercel.app/?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)) from Next.js v8 to v12. Lydia takes the opportunity to list the many improvements that come with the latest versions, and that you get with a minimal upgrade effort. A nice overview of new features that you might have missed.

[**How Wix Applied Multi-threading to Node.js and Cut Thousands of SSR Pods and Money**](https://openjsf.org/blog/2022/03/17/openjs-in-action-how-wix-applied-multi-threading-to-node-js/?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)

Feedback from Wix explaining how they optimized their platform running React Server-Side-Rendering with high CPU demand. They used the new Node.js API 14 [worker_threads](https://nodejs.org/api/worker_threads.html?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter) (allows memory sharing unlike [child_process](https://nodejs.org/api/child_process.html?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)) and got very good results. It's more about Node.js but still find it interesting for those that run self-hosted React SSR pipelines.

[**Shopify: Creating a React Library for Consistent Data Visualization**](https://shopify.engineering/react-library-consistent-data-visualization?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)

Feedback from Shopify reporting consistency issues on its data-visualizations. Solution: the creation of the Polaris Viz lib, that will be open-sourced soon. They explain in particular the use of the React context to create default themes and the possibility of creating variants via partial overrides.

[**Idiomatic Redux: Designing the Redux Toolkit Listener Middleware**](https://blog.isquaredsoftware.com/2022/03/designing-rtk-listener-middleware/?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)

Mark Erikson does a retrospective on the design of the new Redux Toolkit 1.8 [Listener Middleware](https://redux-toolkit.js.org/api/createListenerMiddleware?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter) API, which spans over 2 years, with many iterations. They managed to cover many Redux-Saga/Observable use cases with a relatively simple API. I like the concept of `await condition(predicate)`.

**Extras:**

-   📜 [Nexus --- a Component Tree Visualizer for Next.js](https://levelup.gitconnected.com/introducing-nexus-a-component-tree-visualizer-for-next-js-1109f31e118e?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter): extension VSCode
-   📜 [Using SVG sprites in a React app](https://dev.to/mbarzeev/using-svg-sprites-in-a-react-app-477d?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)
-   📜 [Implementing advanced usePrevious hook with React useRef](https://www.developerway.com/posts/implementing-advanced-use-previous-hook?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)
-   📜 [Remix - Full Context Review](https://www.fullcontextdevelopment.com/blog/remix-full-context-review?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)
-   📜 [Remix vs Next.js](https://bejamas.io/blog/remix-vs-nextjs/?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)
-   📜 [Storybook Community Showcase #1](https://storybook.js.org/blog/community-showcase-1/?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)
-   📖 [Partydown + Gatsby](https://partytown.builder.io/gatsby?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter): integration doc
-   📖 Dan Abramov [annonced 3 new doc pages](https://twitter.com/dan_abramov/status/1504503103109926919?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter) on the beta site: [useReducer](https://beta.reactjs.org/apis/usereducer?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter), [useContext](https://beta.reactjs.org/apis/usecontext?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter), [createContext](https://beta.reactjs.org/apis/createcontext?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)
-   📦 [React-Runner v1](https://twitter.com/_neonie/status/1505880831092482052?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter): stable release for this modern alternative to React-Live permitting to create a code editor with a live preview. Similar to CodeSandbox [Sandpack](https://codesandbox.io/post/sandpack-announcement?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter) but without any iframe, running directly in the browser.
-   📦 [React-Spline](https://github.com/splinetool/react-spline?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter): to run 3D experiences created with the [Spline](https://spline.design/?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter) tool. Not 100% sure what this is, but it looks like a possible alternative to Blender + React-Three-Fiber?
-   📦 [Remix-ETag](https://github.com/donavon/remix-etag?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)
-   📦 [MDX v2.1](https://github.com/mdx-js/mdx/releases/tag/2.1.0?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)

## React-Native

-   📦 [React-Native v0.68.0-rc.3](https://twitter.com/reactnative/status/1506327122771513345?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter): stable v0.68 planned for next week, including a switch to enable Fabric and the new architecture 🤯
-   📜 [Using Storybook and MSW in React Native](https://phelipetls.github.io/posts/using-storybook-and-msw-in-react-native/?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)
-   🧑‍🎨 React-Native-Skia: [shadows](https://twitter.com/wcandillon/status/1505907265072738307?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)
-   🎙️ [RNR 229 - Building an Expo App for Mobile and Web with Josh Justice](https://reactnativeradio.com/episodes/rnr-229-building-an-expo-app-for-mobile-and-web-with-josh-justice?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)
-   😢 [React-Native Weekly - The End](https://andrei-calazans.com/posts/2022-03-22/react-native-weekly?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)
-   📦 [React-Native-Quick-SQLite](https://twitter.com/ospfranco/status/1504389581264896004?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter): async callbacks support
-   📦 [React-Native-Elements v4.0.0-rc.0](https://github.com/react-native-elements/react-native-elements/releases/tag/v4.0.0-rc.0?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)

## Other

[**CodeSandbox Projects**](https://codesandbox.io/post/announcing-codesandbox-projects?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)

CodeSandbox rewrite, new cloud dev experience for projects of any size, with IDE integration (now VSCode, more to come) and even iPad support. Nice contribution workflow, seems handy for quickly collaborating or reviewing a pull-request without switching your local git branch.

**Extras:**

-   [Prettier 2.6](https://prettier.io/blog/2022/03/16/2.6.0.html?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter): new `singleAttributePerLine` option, TS 4.6 support...
-   [Deno 1.20](https://deno.com/blog/v1.20?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter): significant perf improvements, TS 4.6 support, V8 upgrade...
-   [welcome2web3.com](https://welcome2web3.com/?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter): ironic site, demo the web3 UX 😂
-   [Lamina](https://twitter.com/0xca0a/status/1504140883167703044?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter): *"Tailwind for shaders"*
-   [Vercel Deploy](https://chrome.google.com/webstore/detail/vercel-deploy/nkignhibadhmcbiiilleogljodcaonjk?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter): Chrome Extension
-   [Boa v0.14](https://boa-dev.github.io/posts/2022-03-15-boa-release-14/?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)
-   [Parcel CSS v1.7](https://twitter.com/devongovett/status/1505327865553997824?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)
-   [Wave.js 2.0](https://github.com/foobar404/Wave.js?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)
-   [Your SSR is slow & your devtools are lying to you](https://dev.to/mlrawlings/your-ssr-is-slow-your-devtools-are-lying-to-you-3056?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)
-   [Debugging TypeScript using Replay Node](https://medium.com/replay-io/debugging-typescript-using-replay-node-646087b6712?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)
-   [OpenSSL security releases require Node.js security releases](https://nodejs.org/en/blog/vulnerability/mar-2022-security-releases/?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)
-   [Conquering JavaScript Hydration](https://dev.to/ryansolid/conquering-javascript-hydration-a9f?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)
-   [experiences. Web. frameworks. future. me.](https://igor.dev/posts/experiences-web-frameworks-future-me/?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)
-   [Motion Developer Tools](https://twitter.com/mattgperry/status/1505918782685921282?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)
-   [How to write fast code](https://twitter.com/devongovett/status/1504476131818237967?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)
-   [Vitest inline assertions](https://twitter.com/antfu7/status/1505299814069977088?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)? 🤔
-   [hidden="until-found"](https://twitter.com/cramforce/status/1504539803336929282?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)
-   [Alert: peacenotwar module sabotages npm developers in the node-ipc package to protest the invasion of Ukraine](https://snyk.io/blog/peacenotwar-malicious-npm-node-ipc-package-vulnerability/?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)
-   [Protestware is trending in open source: 4 different types and their impact](https://snyk.io/blog/protestware-open-source-types-impact/?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)
-   [Packages with high download numbers that nobody wanted to install](https://www.stefanjudis.com/notes/packages-with-high-download-numbers-that-nobody-wanted-to-install/?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)
-   [CSS-Tricks is joining DigitalOcean!](https://css-tricks.com/css-tricks-is-joining-digitalocean/?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)
-   [In Defense of Sass](https://thinkdobecreate.com/articles/in-defense-of-sass/?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)
-   [Gotchas with Git and the GitHub API](https://retool.com/blog/gotchas-git-github-api/?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)
-   [Retro-specifying fetch/performance](https://blog.whatwg.org/retro-specifying-fetch-performance?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)
-   [Making WebViews work for the Web](https://www.w3.org/blog/2022/03/making-webviews-work-for-the-web/?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)
-   [Why I Prefer Makefiles Over package.json Scripts](https://spin.atomicobject.com/2021/03/22/makefiles-vs-package-json-scripts/?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)

![image](https://user-images.githubusercontent.com/749374/159665898-2cf1c82b-55c8-4a74-8fd4-ebdc53f5db82.png)
 
