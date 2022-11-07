## ⚛️ React

**[React RFC: First class support for promises and async/await](https://github.com/reactjs/rfcs/pull/229)**

React团队决定回到`async/await` 模型以简化服务器组件的使用。问题是：在客户端组件上很难支持`async/await` 。所以他们提议在客户端引入`use(promise)`API。与其他hooks不同， `use`可以被有条件地调用。后来，它可以和其他 "可使用 "的东西一起使用，比如React context（实际上，你已经可以有[条件地使用useContext！](https://twitter.com/acdlite/status/1581401077915975680)）。使用不同的API也可以被看作是一种特性：它允许区分服务器组件和客户端组件。

这个RFC引起了有趣的争论。我们想知道与data fetching库的集成会是什么样子。generators的使用似乎适合这种情况，但它们在实践中很难使用。我们正在等待一个新的RFC，它将引入一个缓存API。

**[The Web’s Next Transition](https://www.epicweb.dev/the-webs-next-transition)**

Kent C. Dodds对3种主要的网络架构进行了很好的回顾，并作了很好的说明和记录。他强调了最新的架构，即当前的趋势。逐步增强的单页应用。Remix是这种架构的一个实现，它有经过深思熟虑的抽象概念，鼓励模仿浏览器的本地行为。我不太同意服务器是绝对必要的。[Docusaurus](https://github.com/facebook/docusaurus)也是一个PESPA的实现，没有JavaScript也能很好地工作。

**[A World-Class Code Playground with Sandpack](https://www.joshwcomeau.com/react/next-level-playground/)**

Josh Comeau赞扬了 [Sandpack](https://github.com/codesandbox/sandpack)，他用来创建交互式代码游乐场的CodeSandbox工具箱。它看起来很容易使用，而且非常灵活!

- 📜 [Streaming: is it worth it?](https://www.builder.io/blog/streaming-is-it-worth-it): Qwik的作者Solid和Marko解释了流媒体的优势，以及为什么很难采用这种技术。在React背景下，所使用的库（Helmet、CSS-in-JS、Redux......）必须兼容，才能使流媒体有效。
- 📜 [Storybook - First-class Vite support](https://storybook.js.org/blog/first-class-vite-support-in-storybook/): 7.0即将进入测试阶段：支持无配置的Vite，预捆绑，不再需要Webpack，支持Vue 2、Lit和Svelte等新。
- 📜 [Moving From React to htmx](https://htmx.org/essays/a-real-world-react-to-htmx-port/): 关于从React成功迁移到[htmx]（https://htmx.org/）的反馈（文章+视频）。我们是在Python后端环境中，他们的结论跟所有开发人员都是全栈的JavaScript环境中可能会有所不同。这位JS开发人员做了POC，之后就失去了工作😅。
- 📜 [Prioritise content over components](https://www.simeongriggs.dev/components-considered-harmful-for-content): 从不同的角度对React组件的设计提出有趣的想法：设计师、开发人员和内容作者（CMS）。
- 📜 [A little semantic HTML trick for React components](https://queen.raae.codes/emails/2022-10-10-semantic-react/): explains how to respect the semantics of HTML by passing the DOM element to be created in props.
- 📜 [Using Web Components With Next (or Any SSR Framework)](https://css-tricks.com/using-web-components-with-next-or-any-ssr-framework/)
- 📜 [Exploring how virtual DOM is implemented in React](https://indepth.dev/posts/1501/exploring-how-virtual-dom-is-implemented-in-react)
- 📜 [Lazy-load React components in Remix](https://sergiodxa.com/articles/lazy-load-react-components-in-remix)
- 🐦 [React tip: isFocused should almost never be a prop](https://twitter.com/DavidKPiano/status/1580179833052876800)
- 🚧 [Streaming SSR in Preact prototype](https://twitter.com/marvinhagemeist/status/1581762567328104448)
- 🧑‍🎓 [Create a 3D site with Game Controls in Spline and React](https://designcode.io/spline2) ([video](https://www.youtube.com/watch?v=uYp_ipIasYE))
- 🎨 [Satori + React-Three-Fiber demo](https://twitter.com/0xca0a/status/1581751380339232768)
- 🎨 [Satori + SVG code syntax highlighting demo](https://twitter.com/shuding_/status/1581358324569645056)
- 🎙️ [Docusaurus 2 is a pretty big deal](https://changelog.com/jsparty/247)
- 🎥 [In Defense of useEffect](https://www.youtube.com/watch?v=Zw4lJqBphvA)
- 🎥 [Making React Context Fast!](https://www.youtube.com/watch?v=ZKlXqrcBx88)
- 📦 [Planby - React.js based component for schedules and timelines](https://planby.netlify.app/)
- 📦 [Gatsby v5 beta](https://twitter.com/GatsbyJS/status/1580288285229735936)
- 📦 [Astro 1.5](https://twitter.com/astrodotbuild/status/1580611193429168129)
- 📦 [SWR 2.0 RC](https://github.com/vercel/swr/releases/tag/2.0.0-rc.0)


## 📱 React-Native

**[2022: How can we improve React Native?](https://github.com/react-native-community/discussions-and-proposals/discussions/528)**

React-Native团队希望得到关于React-Native中需要改进的内容的反馈。提到的一些要点。CSS支持（Yoga, gap, grid, shadows...），跨平台支持，版本升级，调试，键盘，Metro symlinks...

- 💬 [Restructuring React Native's Public API](https://github.com/react-native-community/discussions-and-proposals/discussions/523)
- 📜 [Setting up React Native Monorepo with Yarn Workspaces](https://www.callstack.com/blog/setting-up-react-native-monorepo-with-yarn-workspaces)
- 📜 [How to Use Module Federation with Re.Pack 3](https://www.callstack.com/blog/module-federation-with-re-pack-3)
- 🚧 [Expo Router 0.0.27](https://twitter.com/Baconbrix/status/1579912795323215872) + [Layout API change RFC](https://twitter.com/Baconbrix/status/1582057133939384321)
- 🚧 [React-Native Bottom Sheet v5 will have web support](https://twitter.com/gorhom/status/1581334529121218561)
- 🚧 [React-Native Flex gap support coming?](https://twitter.com/Baconbrix/status/1580587087174062080)
- 📖 [Expo docs improvements](https://twitter.com/amanhimself/status/1580615698321399811): "Running E2E tests on EAS Build now works on Android"
- 📦 [Metro 0.73.0](https://github.com/facebook/metro/releases/tag/v0.73.0)
- 📦 [React-Native 0.70.3](https://twitter.com/Kelset/status/1580210635266084864)
- 🎥 [Flip card Animation in React-Native Re-Animated 2](https://www.youtube.com/watch?v=nVsvcu93488)
- 🎙️ [React-Native-Radio 248 - Introducing Ignite v8: Maverick!](https://reactnativeradio.com/episodes/rnr-248-introducing-ignite-v8-maverick)


## 🔀 Other

**[StackBlitz Codeflow](https://stackblitz.com/codeflow)**

StackBlitz [WebContainers](https://blog.stackblitz.com/posts/introducing-webcontainers/)允许通过WebAssembly在浏览器中运行Node.js。你可以直接在浏览器中运行VS Code、Next.js或Docusaurus，而不是通过远程Docker容器。Codeflow增加了与GitHub的整层集成，使得通过在本地以安全的方式运行pull-request，可以很容易地打开、审查或编辑：对于开源项目非常有用。

他们还推出了Web Publisher，一个简化的Markdown文件的编辑视图（编辑器、预览、保存按钮）。对于在Git上贡献文档来说非常方便，即使是技术性不强的用户。有一个真正的内容预览，而不是GitHub Markdown预览的降级体验。这是一个[Docusaurus用户的重要需求]（https://twitter.com/ericsimons40/status/1580371754974781440）

**[Fontaine - Automatic font fallback based on font metrics](https://github.com/unjs/fontaine)**

允许在加载自定义字体时避免布局转移。使后备字体与最终字体的大小相同，这样过渡就很平稳，不会影响文本容器的大小。好主意!

- [Node.js 19](https://twitter.com/nodejs/status/1582401871179747329)
- [Node 18.11](https://nodejs.org/en/blog/release/v18.11.0/): adds a new `--watch` mode and a [few other cool things](https://twitter.com/matteocollina/status/1580911016506163202)
- [Unplugin - Unified plugin system for Vite, Rollup, Webpack, and more](https://github.com/unjs/unplugin): to create agnostic plugins that work on all bundlers!
- [CSS - Help pick a syntax for nesting - Survey results](https://developer.chrome.com/blog/help-css-nesting-results/)
- [Status update of my tsc port](https://kdy1.dev/posts/2022/10/tsc-port-status) + [Speedy TypeScript type checker public repo](https://twitter.com/kdy1dev/status/1582174891230760960)
- [TypeRunner - High-performance TypeScript compiler](https://github.com/marcj/TypeRunner)
- [Lerna reborn — What’s new in v6?](https://blog.nrwl.io/lerna-reborn-whats-new-in-v6-10aec6e9091c)
- [What’s new in Nx 15?](https://blog.nrwl.io/whats-new-in-nx-15-7e14e1ff282d)
- [JetBrains Fleet - Public Preview](https://blog.jetbrains.com/fleet/2022/10/introducing-the-fleet-public-preview/)
- [Import maps soon available in all browsers](https://twitter.com/sebastienlorber/status/1582024272788480000)
- [Bun's, ViteConf talk](https://twitter.com/jarredsumner/status/1581427214691708929)
- [rRPC-chrome - tRPC adapter for Web Extensions](https://github.com/jlalmes/trpc-chrome)
- [What is pnpm? Is it really so fast and space-efficient?](https://dev.to/stackblitz/what-is-pnpm-and-is-it-really-so-fast-and-space-efficient-29la)
- [Intl Explorer - A tool for experimenting and trying out the ECMAScript Internationalization API](https://www.intl-explorer.com/)
- [Why We Use Babylon.js Instead Of Three.js in 2022](https://www.spotvirtual.com/blog/why-we-use-babylonjs-instead-of-threejs-in-2022)
- [How Vite Came to Be - ViteConf 2022 slides](https://docs.google.com/presentation/d/1O09rAOu_wRLHVjukVbBeSlRkLeX-dcYZfsdjPiU4kGQ/edit#slide=id.p)
- [Rollup v3](https://github.com/rollup/rollup/releases/tag/v3.0.0)
- [Jest 29.2](https://github.com/facebook/jest/releases/tag/v29.2.0)
- [Obsidian 1.0](https://obsidian.md/1.0)


