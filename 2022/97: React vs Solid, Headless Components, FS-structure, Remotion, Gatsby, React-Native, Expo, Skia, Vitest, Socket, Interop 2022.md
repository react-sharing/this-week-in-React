This Week In React #97: React vs Solid, Headless Components, FS-structure, Remotion, Gatsby, React-Native, Expo, Skia, Vitest, Socket, Interop 2022...

## React

[**Solid.js feels like what I always wanted React to be**](https://typeofnan.dev/solid-js-feels-like-what-i-always-wanted-react-to-be/?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)

Explains why Solid is simpler than React. Solid is reactive and directly updates the DOM (without virtual DOM). The render function is only called once, even if the state changes, and there are no stale closure issues. A good article to discover the differences between these 2 frameworks and discover Solid.

I find Solid really interesting. In the short term it can be a very good alternative to React for web apps. However, I am waiting to see the practical use of the innovations of React 18 because I think that the virtual DOM is interesting for the highly anticipated concurrent features.

[**Headless components in React and why I stopped using a UI library for our design system**](https://medium.com/@nirbenyair/headless-components-in-react-and-why-i-stopped-using-ui-libraries-a8208197c268?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)

Nir tells his story: from using React-Bootstrap and MUI to implementing an autocomplete from scratch, to ending up using a headless lib that encapsulates behavior and accessibility. A good intro to understand the interest of headless libs, which also lists the popular libs of the ecosystem.

[**Screaming Architecture: Evolution of a React folder structure and why to group by features right away**](https://profy.dev/article/react-folder-structure?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)

Johannes shows us how he gradually refactors his file-system structure to keep his app maintainable over time. An interesting line of thought. I don't think there is a one-size-fits-all solution that works for everyone. Personally I like fractal trees, and I would love for [IDEs to offer a way to tag files](https://twitter.com/sebastienlorber/status/1501204809193566220?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter).

[**What's New at GatsbyConf 2022**](https://www.gatsbyjs.com/blog/whats-new-at-gatsbyconf-2022/?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)

Gatsby now offers an [Image CDN](https://www.gatsbyjs.com/blog/image-cdn-lightning-fast-image-processing-for-gatsby-cloud/?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter) that reduces build times and optimizes loading (Note: Netlify offers [an equivalent](https://github.com/netlify/netlify-plugin-gatsby/blob/main/docs/image-cdn.md?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)). Other notable improvements announced: incremental deploys, full TypeScript support, GitHub Enterprise, trailing slash...

[**Hooks: React's do-notation**](https://devanshj.me/writings/hooks-reacts-do-notation?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)

For FP lovers. Devansh explains that you can convert each hook to a render-prop, but not the other way around. Hooks are just syntactic sugar to avoid the "callback hell". It is related to Haskell monads and the do notation. Show various interesting experiments like implementing conditional rendering, or using generator functions for hooks.

**Extras:**

-   📜 [Building Pages in Storybook](https://storybook.js.org/blog/building-pages-in-storybook/?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter): Storybook is not limited to the design system and can also be used on full pages. You can mock data, and the new `play()` function seems useful to setup pages in edge cases.
-   📜 [How to manage the useEffect dependency array like a pro?](https://blog.bam.tech/developer-news/how-to-avoid-bugs-in-useeffect?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)
-   📜 [A Deep Dive Comparison Between useMemo And useCallback](https://www.chakshunyu.com/blog/a-deep-dive-comparison-between-usememo-and-usecallback/?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)
-   📜 [Hosting a React App with OpenFaaS](https://www.openfaas.com/blog/react-app/?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)
-   📜 [Improving Web Performance with React Hydration Strategies](https://medium.com/cdiscount-engineering/improving-web-performance-with-react-hydration-strategies-3117f71a1695?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)
-   🧵 Sebastian Markbåge: [*"One day, React will switch to only ESM"*](https://twitter.com/sebmarkbage/status/1498841717881151489?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)
-   🐦 [Classic vs Shorthand Props](https://twitter.com/tannerlinsley/status/1499773428739416068?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)
-   🎥 [Remotion + Fireship](https://www.youtube.com/watch?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter&v=deg8bOoziaE): nice intro to discover Remotion
-   🎥 [10 React Antipatterns to Avoid](https://www.youtube.com/watch?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter&v=b0IZo2Aho9Y): Fireship suggests to avoid some React anti-patterns. A good reminder.


## React-Native


[**Expo: EAS Update Preview Progress**](https://blog.expo.dev/eas-update-preview-progress-f504a30066fc?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)

Expo shares its progress on EAS Update, the new Over-The-Air update system currently in preview. It is possible to associate a release channel with a Git branch and do continuous delivery. They also improved performance, security, and are working on a web UI to make it easier to use.

[**React Native + Github Action = ❤️**](https://www.obytes.com/blog/react-native-github-action?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)

Offers a complete workflow to automate the build of React-Native apps. The build is triggered when a new GitHub release is created. There is a bit of work, but it shows that Fastlane may not be so essential anymore.

**Extras:**

-   📜 [What makes Hermes engine (React Native) fast?](https://medium.com/tilicholabs/what-makes-hermes-engine-react-native-fast-ac6fa5e3ad2e?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)
-   📜 [How we made our React Native tests run 5x faster](https://medium.com/life-at-chime/how-we-made-our-react-native-tests-run-5x-faster-ef94ce49a83c?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)
-   🧑‍🎨 React-Native-Skia [v0.1.105](https://twitter.com/wcandillon/status/1501170689134452737?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter): [animations](https://twitter.com/wcandillon/status/1499367700581265409?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter), [drop shadow](https://twitter.com/wcandillon/status/1499351714805264387?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)...
-   🐦 [Expo deprecating expo-app-auth](https://twitter.com/Baconbrix/status/1499852086900527104?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)
-   🐦 [@margelo_io](https://twitter.com/margelo_io?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter) (Marc Rousavy) sharing interesting React-Native tips
-   📦 [Stacks](https://mobily.github.io/stacks/?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter): a set of React-Native primitives to create your layouts. Encapsulates the practice of [avoiding margins](https://mxstbr.com/thoughts/margin/?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter). [v2.0](https://github.com/mobily/stacks/releases/tag/v2.0.0?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter) has just been released.
-   📦 [react-native-reanimated-zoom](https://github.com/intergalacticspacehighway/react-native-reanimated-zoom?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)


## Other

[**Socket: Secure your JavaScript supply chain**](https://socket.dev/?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)

New tool to detect supply-chain security vulnerabilities: compromised npm libs you use in your apps.

Offers a different and pro-active approach: rather than looking for known vulnerabilities, assumes that any npm package may be compromised and looks for indicators based on the history of packages that have already been compromised. A tool to adopt quickly, given the number of attacks of this type is increasing sharply. Read also:

-   [Introducing Socket](https://socket.dev/blog/introducing-socket?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)
-   [What's Really Going On Inside Your node_modules Folder?](https://socket.dev/blog/inside-node-modules?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)
-   [Why Vulnerability Scanning Isn't Enough To Protect Your App](https://socket.dev/blog/vuln-scanning-is-not-enough?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)

[**Interop 2022: browsers working together to improve the web for developers**](https://web.dev/interop-2022/?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)

The teams of the main browsers will work together in 2022 to improve compatibility on 15 areas of focus which are particularly painful for developers today. There's even a [dashboard](https://wpt.fyi/interop-2022?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter) with a compatibility score for each browser. We find among others the cascade layers, color functions, viewport units, scroll, subgrid...

**Extras:**

-   [Vitest v0.6](https://github.com/vitest-dev/vitest/releases/tag/v0.6.0?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter): a great innovation: [In-source testing](https://vitest.dev/guide/features.html?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter#in-source-testing) permits to co-locate the test in the source code file!
-   [Monorepos are changing how teams build software](https://vercel.com/blog/monorepos-are-changing-how-teams-build-software?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter): Vercel gives 4 good reasons to adopt the monorepo
-   [The `<selectmenu>` HTML element](https://css-tricks.com/the-selectmenu-element/?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter): an upcoming HTML component could gradually replace `<select>`
-   [Future Javascript: ShadowRealms](https://fjolt.com/article/javascript-shadowrealms?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter): TC39 moved to stage-3 recently. Allows to execute code in isolation
-   [Implementing Node.js URL parser in WebAssembly with Rust](https://www.yagiz.co/implementing-node-js-url-parser-in-webassembly-with-rust/?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter): interesting feedback: using Rust compiled in WASM did not improve performance of this Node.js API
-   [Jest `--shard` option](https://github.com/facebook/jest/pull/12546?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter), parallelize the tests on its CI
-   [WebGPU --- All of the cores, none of the canvas](https://surma.dev/things/webgpu/?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)
-   [SPAs were a mistake](https://gomakethings.com/spas-were-a-mistake/?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)
-   [Steve Schoger tips on dark mode](https://twitter.com/steveschoger/status/1499780794193166341?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)
-   [Progressive enhancement + dark mode switch](https://twitter.com/sebastienlorber/status/1500872668727451651?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)
-   [How to add types for Object.fromEntries](https://dev.to/svehla/typescript-object-fromentries-389c?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)
-   [Introducing The XState CLI](https://stately.ai/blog/introducing-the-xstate-cli?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)
-   [New to the web platform in February 2022](https://web.dev/web-platform-02-2022/?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)
-   [Safari Technology Preview 141](https://twitter.com/jensimmons/status/1499541941880565760?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)
-   [New CSS Features In 2022](https://www.smashingmagazine.com/2022/03/new-css-features-2022/?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)
-   [Can you get pwned with CSS?](https://scotthelme.co.uk/can-you-get-pwned-with-css/?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)
-   [Parcel CSS 1.5](https://github.com/parcel-bundler/parcel-css/releases/tag/v1.5.0?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)
-   [*"Chrome 99 rolled out this week, with Cascade Layers on by default."*](https://twitter.com/TerribleMia/status/1499830089952858117?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)
-   [Web devs rally to challenge Apple App Store browser rules](https://www.theregister.com/2022/02/28/apple_apps_challenge/?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)
-   [Thoughts On Markdown](https://www.smashingmagazine.com/2022/02/thoughts-on-markdown/?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)
-   [Flightcontrol:world-class deployment DX natively to your AWS](https://twitter.com/flybayer/status/1498640141904138241?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)
-   [Cloudflare: Steps we've taken around Cloudflare's services in Ukraine, Belarus, and Russia](https://blog.cloudflare.com/steps-taken-around-cloudflares-services-in-ukraine-belarus-and-russia/?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)
-   [Renovated Home For WAPM WebAssembly package manager](https://wasmer.io/posts/wapm-revamp?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)
-   [A new year, a new MDN](https://hacks.mozilla.org/2022/03/a-new-year-a-new-mdn/?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)

![Capture d’écran 2022-03-09 à 09 49 18](https://user-images.githubusercontent.com/749374/157408719-35509d35-c501-46e0-a387-687d10b3aeca.png)
