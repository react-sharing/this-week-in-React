# React

[**Remix: Not Another Framework!**](https://remix.run/blog/not-another-framework?utm_campaign=thisweekinreact&utm_medium=email&utm_source=Revue%20newsletter)

Remix builds on top of Web standard APIs. Ryan Florence can’t predict if Remix will stick, but gives good reasons to learn it: the knowledge you acquire won’t be lost. It’s like React: no need to learn another templating language, and the JS knowledge you get by using JSX remains usable in many other places.

Remix is also designed to be framework-agnostic. On Twitter, [Ryan Florence teases us on the next possible targets for Remix](https://twitter.com/ryanflorence/status/1486530142507655173?utm_campaign=thisweekinreact&utm_medium=email&utm_source=Revue%20newsletter). I bet on Qwik and Solid.

I increasingly see Remix as a potential gateway to Deno (also based on web APIs), and possibly the next framework to outlive React.

Unrelated: [Kent C. Dodds had a serious car accident](https://twitter.com/kentcdodds/status/1487314342366171139?utm_campaign=thisweekinreact&utm_medium=email&utm_source=Revue%20newsletter) 🤕

[**MDX 2.0**](https://mdxjs.com/blog/v2/?utm_campaign=thisweekinreact&utm_medium=email&utm_source=Revue%20newsletter)

Official launch for MDX 2.0. This technology permits to interleave Markdown and JSX quite easily, very convenient to create interactive content (ie [Josh Comeau](https://www.joshwcomeau.com/?utm_campaign=thisweekinreact&utm_medium=email&utm_source=Revue%20newsletter)’s website, Docusaurus…).

v2 improves on many things: fixes a few syntax problems, significantly improves performances , can support other frameworks…

[**Lifetime Analysis for React Component Architecture**](https://valand.dev/blog/post/from-rust-to-typescript-lifetime-analysis?utm_campaign=thisweekinreact&utm_medium=email&utm_source=Revue%20newsletter)

Alan is inspired by the concepts of lifetime analysis and ownership of objects in Rust to deduce where to put his React state. I feel like I do exactly this, intuitively. Original reading, a little verbose initially, but this makes sense at the end. No need to understand Rust.

[**Creating a Schema-Based Form System**](https://www.taniarascia.com/schema-based-form-system/?utm_campaign=thisweekinreact&utm_medium=email&utm_source=Revue%20newsletter)

Tania explains how to drive the rendering of a React form with a JSON schema. The example is based on Formik and Yup, but it is above all the technique that matters, and can be useful for integration with a CMS or backend that sends you such schema

**Extras:**
-   Dan Abramov rewrote the [React Quick Start docs](https://twitter.com/dan_abramov/status/1486898522167427074?utm_campaign=thisweekinreact&utm_medium=email&utm_source=Revue%20newsletter) (beta site) and it looks great!
-   🎥 [The Story of React](https://www.youtube.com/watch?utm_campaign=thisweekinreact&utm_medium=email&utm_source=Revue%20newsletter&v=Wm_xI7KntDs): nice retrospective on the story of React, from JQuery/Backbone to Next.js/Remix
-   [Pause Your React App with Breakpoints](https://alexsidorenko.com/blog/debug-react-breakpoints/?utm_campaign=thisweekinreact&utm_medium=email&utm_source=Revue%20newsletter): for those still using `console.log` 😏
-   [react-zorm](https://github.com/esamattis/react-zorm?utm_campaign=thisweekinreact&utm_medium=email&utm_source=Revue%20newsletter): new React form lib (uncontrolled), typed and based on Zod, leveraging web APIs (`FormData`) to integrate nicely with Remix
-   [The baseline for web development in 2022](https://engineering.linecorp.com/en/blog/the-baseline-for-web-development-in-2022/?utm_campaign=thisweekinreact&utm_medium=email&utm_source=Revue%20newsletter): those stats on the web got the ecosystem talking this week: React doesn’t have such good scores, and in particular Next.js (beaten by Gatsby on Core Web Vitals).
-   🧵 [“Over-fetching means three things to me”](https://twitter.com/sebmarkbage/status/1485808604024385539?utm_campaign=thisweekinreact&utm_medium=email&utm_source=Revue%20newsletter): on the advantages of GraphQL with Relay, compared to modern alternatives (Remix loaders, Next.js getServerProps, tRPC…)
-   🧵 [Next.js: avoid returning too much data in getStaticProps and getServerProps](https://twitter.com/ascorbic/status/1487024158492049408?utm_campaign=thisweekinreact&utm_medium=email&utm_source=Revue%20newsletter)
-   [Recoil 0.6](https://recoiljs.org/blog/2022/01/28/0.6.0-release/?utm_campaign=thisweekinreact&utm_medium=email&utm_source=Revue%20newsletter): React 18, concurrent rendering, strict mode
-   [Docusaurus 2.0.0-beta.15](https://twitter.com/docusaurus/status/1486404763902222341?utm_campaign=thisweekinreact&utm_medium=email&utm_source=Revue%20newsletter): nice release 😌
-   [SWR 1.2](https://github.com/vercel/swr/releases/tag/1.2.0?utm_campaign=thisweekinreact&utm_medium=email&utm_source=Revue%20newsletter): supports `.mjs` + optimistic UI auto error rollback
-   [Gatsby v4.6](https://www.gatsbyjs.com/docs/reference/release-notes/v4.6/?utm_campaign=thisweekinreact&utm_medium=email&utm_source=Revue%20newsletter)
-   🎥 [Nx ❤️ Remix](https://www.youtube.com/watch?utm_campaign=thisweekinreact&utm_medium=email&utm_source=Revue%20newsletter&v=yUuEA4V6DJ0)
-   [Atomic design and storybook](https://bradfrost.com/blog/post/atomic-design-and-storybook/?utm_campaign=thisweekinreact&utm_medium=email&utm_source=Revue%20newsletter) 


# React-Native

-   [React-Native Versions](https://rn-versions.github.io/?utm_campaign=thisweekinreact&utm_medium=email&utm_source=Revue%20newsletter): TIL about this tool to know usage of each React-Native version (+ Expo SDK). Might be useful to convince your boss to upgrade.
-   [Deep dive into React Native’s New Architecture](https://medium.com/coox-tech/deep-dive-into-react-natives-new-architecture-fb67ae615ccd?utm_campaign=thisweekinreact&utm_medium=email&utm_source=Revue%20newsletter): introduce pieces of the new architecture: JSI, Fabric, Turbomodules, Codegen
-   🐦 [“We will be focusing a lot on Expo web this year”](https://twitter.com/ccheever/status/1486102143538843648?utm_campaign=thisweekinreact&utm_medium=email&utm_source=Revue%20newsletter): exciting!
-   🐦 Demo React-Native-Skia: [shaders](https://twitter.com/wcandillon/status/1488059414892400641?utm_campaign=thisweekinreact&utm_medium=email&utm_source=Revue%20newsletter), [path interpolations](https://twitter.com/chrfalch/status/1487075486161383433?utm_campaign=thisweekinreact&utm_medium=email&utm_source=Revue%20newsletter)
-   🐦 [React-Native-Performance 0.4](https://twitter.com/almouro/status/1486667676164538376?utm_campaign=thisweekinreact&utm_medium=email&utm_source=Revue%20newsletter)
-   🎙️ [RNR 225 - Behind Our Decision to Cancel Chain React 2022](https://reactnativeradio.com/episodes/rnr-225-chain-react-update-and2022-workshops?utm_campaign=thisweekinreact&utm_medium=email&utm_source=Revue%20newsletter) 

# Other

[**Porting tsc to Go (not Rust**](https://kdy1.dev/posts/2022/1/tsc-go?utm_campaign=thisweekinreact&utm_medium=email&utm_source=Revue%20newsletter)

With the arrival of new bundlers, type-checking becomes the bottleneck in larger codebases. Donny (Vercel) is the author of [SWC](http://swc.rs/?utm_campaign=thisweekinreact&utm_medium=email&utm_source=Revue%20newsletter) (Rust). He attempted a complete rewrite in Rust (POC compiles 62x faster than `tsc`), but it’s a lot of work compared to a port that would draw on existing `tsc` code.

Problem: the `tsc` codebase is difficult to port to Rust (shared mutability, GC…), and Go is better suited for this specific task.

The plan of SWC and Vercel is clear: they will provide us fast tooling for the everything we need: transpilation, typechecking, minification and bundling.

About porting tsc, another alternative in Rust exists - [tyty](https://zackoverflow.dev/writing/tyty?utm_campaign=thisweekinreact&utm_medium=email&utm_source=Revue%20newsletter) - but for the moment it’s a side-project, not yet open-sourced.

[**Deno in 2021**](https://deno.com/blog/deno-in-2021?utm_campaign=thisweekinreact&utm_medium=email&utm_source=Revue%20newsletter)

Deno shares its 2021 retrospective, with improvements on the core (opcalls, perf, FFI), their Deno Deploy service (V8 isolates, comparable to Cloudflare, good target for Remix)…

I’m excited about the compatibility with web APIs and [Node.js compat mode](https://deno.com/blog/v1.15?utm_campaign=thisweekinreact&utm_medium=email&utm_source=Revue%20newsletter#improving-node-compatibility). With Node.js gradually implementing web APIs (see below), we might be able to switch from one to the other more easily through meta-frameworks like Remix.

**Extras:**

-   Node.js: v18 will [support native ](https://github.com/nodejs/node/pull/41749?utm_campaign=thisweekinreact&utm_medium=email&utm_source=Revue%20newsletter)`fetch()` 🙌! [JSON modules unflagged](https://github.com/nodejs/node/pull/41736?utm_campaign=thisweekinreact&utm_medium=email&utm_source=Revue%20newsletter) and maybe a new API `Response.json()`?
-   [Node.js debugging and error handling with Error Cause](https://medium.com/ovrsea/power-up-your-node-js-debugging-and-error-handling-with-the-new-error-cause-feature-4136c563126a?utm_campaign=thisweekinreact&utm_medium=email&utm_source=Revue%20newsletter): nice introduction to this ES 2022 feature
-   [Trailing Slashes on URLs: Contentious or Settled?](https://www.zachleat.com/web/trailing-slash/?utm_campaign=thisweekinreact&utm_medium=email&utm_source=Revue%20newsletter): my [analysis on trailing slashe](https://github.com/slorber/trailing-slash-guide?utm_campaign=thisweekinreact&utm_medium=email&utm_source=Revue%20newsletter) (done for Docusaurus) seems useful for the community. Zach Leatherman (Eleventy/Netlify) presented it in a more appealing way 🤗 This should also [help Gatsby](https://github.com/gatsbyjs/gatsby/discussions/34205?utm_campaign=thisweekinreact&utm_medium=email&utm_source=Revue%20newsletter#discussioncomment-1954098) 😏
-   [V8 v9.9](https://v8.dev/blog/v8-release-99?utm_campaign=thisweekinreact&utm_medium=email&utm_source=Revue%20newsletter): Intl improvements
-   [prettier-plugin-tailwindcss](https://tailwindcss.com/blog/automatic-class-sorting-with-prettier?utm_campaign=thisweekinreact&utm_medium=email&utm_source=Revue%20newsletter): to sort classNames
-   [Updates from the 88th meeting of TC39](https://dev.to/hemanth/updates-from-the-88th-meeting-of-tc39-473n?utm_campaign=thisweekinreact&utm_medium=email&utm_source=Revue%20newsletter): not much 😅 Note there’s an [enum proposal](https://github.com/Jack-Works/proposal-enum?utm_campaign=thisweekinreact&utm_medium=email&utm_source=Revue%20newsletter) (stage 0) 🤔
-   [Turborepo v1.1](https://turborepo.org/blog/turbo-1-1-0?utm_campaign=thisweekinreact&utm_medium=email&utm_source=Revue%20newsletter): allows in particular to create dependencies on env variables
-   [The TypeScript converging point](https://fettblog.eu/slides/the-typescript-converging-point/?utm_campaign=thisweekinreact&utm_medium=email&utm_source=Revue%20newsletter):  *“Can we express every JavaScript program through TypeScript types?”*  Stefan answers  *“Not yet”*  and explains limitations by typing the CLI package `commander`
-   [NAPI-RS creator hired by Vercel](https://twitter.com/Brooooook_lyn/status/1488194978501500928?utm_campaign=thisweekinreact&utm_medium=email&utm_source=Revue%20newsletter) which strengthens its position on Rust
-   [Vue 3 as the New Default](https://blog.vuejs.org/posts/vue-3-as-the-new-default.html?utm_campaign=thisweekinreact&utm_medium=email&utm_source=Revue%20newsletter)
-   [Caching Header Best Practices](https://simonhearne.com/2022/caching-header-best-practices/?utm_campaign=thisweekinreact&utm_medium=email&utm_source=Revue%20newsletter)
-   [Writing build scripts using TypeScript](https://egoist.sh/build-scripts-in-ts?utm_campaign=thisweekinreact&utm_medium=email&utm_source=Revue%20newsletter)
-   [How TypeScript Won Over Developers and JavaScript Frameworks](https://thenewstack.io/how-typescript-won-over-developers-and-javascript-frameworks/?utm_campaign=thisweekinreact&utm_medium=email&utm_source=Revue%20newsletter)
-   [Demystifying TypeScript Discriminated Unions](https://css-tricks.com/typescript-discriminated-unions/?utm_campaign=thisweekinreact&utm_medium=email&utm_source=Revue%20newsletter)
-   [openapi-graphql](https://github.com/mcollina/openapi-graphql?utm_campaign=thisweekinreact&utm_medium=email&utm_source=Revue%20newsletter)
-   [The Return of Server Side Routing](https://dev.to/this-is-learning/the-return-of-server-side-routing-b05?utm_campaign=thisweekinreact&utm_medium=email&utm_source=Revue%20newsletter)
-   State of the Web: [Bundlers & Build Tools](https://byteofdev.com/posts/bundlers/?utm_campaign=thisweekinreact&utm_medium=email&utm_source=Revue%20newsletter), [Static Site Generators](https://byteofdev.com/posts/static-site-generators/?utm_campaign=thisweekinreact&utm_medium=email&utm_source=Revue%20newsletter), [Serverless Functions](https://byteofdev.com/posts/serverless/?utm_campaign=thisweekinreact&utm_medium=email&utm_source=Revue%20newsletter), [Deno](https://byteofdev.com/posts/deno/?utm_campaign=thisweekinreact&utm_medium=email&utm_source=Revue%20newsletter), [WebAssembly](https://byteofdev.com/posts/webassembly/?utm_campaign=thisweekinreact&utm_medium=email&utm_source=Revue%20newsletter)
-   [Publishing and consuming ECMAScript modules via packages](https://2ality.com/2022/01/esm-specifiers.html?utm_campaign=thisweekinreact&utm_medium=email&utm_source=Revue%20newsletter)
-   [A pipe operator for JavaScript: introduction and use cases](https://2ality.com/2022/01/pipe-operator.html?utm_campaign=thisweekinreact&utm_medium=email&utm_source=Revue%20newsletter)
-   [Storybook + Figma](https://storybook.js.org/blog/figma-plugin-sneak-peek/?utm_campaign=thisweekinreact&utm_medium=email&utm_source=Revue%20newsletter)
-   [The Web in 2036: Predictions on a Whim](https://blog.jim-nielsen.com/2022/web-predictions-on-a-whim/?utm_campaign=thisweekinreact&utm_medium=email&utm_source=Revue%20newsletter)
-   [Building a Vaporwave scene with Three.js](https://blog.maximeheckel.com/posts/vaporwave-3d-scene-with-threejs/?utm_campaign=thisweekinreact&utm_medium=email&utm_source=Revue%20newsletter)
-   [Speeding up VSCode (extensions) in 2022](https://jason-williams.co.uk/speeding-up-vscode-extensions-in-2022?utm_campaign=thisweekinreact&utm_medium=email&utm_source=Revue%20newsletter)
-   [Getting Started With CSS Cascade Layers](https://www.smashingmagazine.com/2022/01/introduction-css-cascade-layers/?utm_campaign=thisweekinreact&utm_medium=email&utm_source=Revue%20newsletter)
-   🎥 [How does !important actually work?](https://www.youtube.com/watch?utm_campaign=thisweekinreact&utm_medium=email&utm_source=Revue%20newsletter&v=dS123IXPcJ0)



