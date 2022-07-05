This Week In React #103: Contentlayer, Remotion 3, Stale Closure, Cross-platform, Jest 28, Hydration, Netlify Edge Functions...

## React

[**Contentlayer: Content Made Easy for Developers (beta)**](https://www.contentlayer.dev/blog/beta?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)

Contentlayer是一个新的系统，它提供了管理你的内容（Markdown，CMS，Notion...）和你的代码之间的联系。你定义一个模式，它将验证/编译你的内容，并高效地生成一个带有TypesScript类型的`.contentlayer`文件夹，并可以直接导入你的应用程序中。这似乎大大改善了构建性能（即使有冷缓存，也能达到X2的提升）。测试版有一个官方的[Next.js集成](https://www.contentlayer.dev/docs/environments/nextjs?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter) ，减少了生成代码的数量。我建议观看[介绍性的入门视频](https://www.youtube.com/watch?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter&v=58Pj4a4Us7A) （5分钟），以了解它在Next.js背景下的工作情况。[Johannes Schickling](https://twitter.com/schickling?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)的一个新项目，也是[Prisma](https://github.com/prisma/prisma?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)的创造者，也在研究代码和DB之间的胶水。

[**Remotion 3.0**](https://www.remotion.dev/blog/3-0?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)

Remotion可以使用用React（网络）代码和data/props的编程方式创建视频。经过10个月的开发，v3.0刚刚发布（[预告片](https://www.youtube.com/watch?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter&v=GN2jkJphR5M)），主要的新功能是对[AWS Lambda](https://www.remotion.dev/lambda?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)上的无服务器渲染的新支持，它允许你扩展，降低成本，并更快地制作视频

[**Hooks, Dependencies and Stale Closures**](https://tkdodo.eu/blog/hooks-dependencies-and-stale-closures?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)

包含调试代码的文章，帮助全面了解React中的陈旧闭包问题。如果你使用记忆化，并且未开启ESLint的`exhaustive-deps`规则，你就有可能在你的代码库中引入这种类型的问题，而这有时候很难调试!

[**The challenges of rendering an OpenLayers map in a popup through React**](https://dev.to/noriste/the-challenges-of-rendering-an-openlayers-map-in-a-popup-through-react-2elh?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)

关于在几个窗口中通过门户渲染React应用的一个有趣的反馈。它有一些优点（用一个状态来控制所有的窗口），但也有一些问题需要解决。

**拓展阅读**

-   📜 [File-based routing with React Location --- Nested layouts](https://omarelhawary.me/blog/file-based-routing-with-react-location-nested-layouts?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter): the creator of [Generouted](https://github.com/oedotme/generouted?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter) continues his series on implementing a home-made file-based routing. Here he shows how to implement nested layouts (inspired by Remix) based on Vite and React-Location.
-   📜 [React Component Composition Explained](https://felixgerschau.com/react-component-composition/?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter): composition can help solve drilling props and improve performance.
-   📜 [Upgrading to React 18 with TypeScript](https://blog.logrocket.com/upgrading-react-18-typescript/?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter): summary of TypeScript breaking changes coming with React 18, and how to automate the migration via codemod.
-   📜 [Flexible Design System Components With "as/is" Props](https://www.lloydatkinson.net/posts/2022/design-system-component-as-is-props/?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter): useful technique to use a component with different HTML tags depending on the context: `<span>`, `<h1>`...
-   📜 [Introduction to React v18 Suspense and Render-as-You-Fetch approach](https://medium.com/jspoint/introduction-to-react-v18-suspense-and-render-as-you-fetch-approach-1b259551a4c0?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter): using React 18 new features to avoid waterfalls.
-   📜 [Creating a Rich Text Editor using Rust and React](https://fiberplane.dev/blog/creating-a-rich-text-editor-using-rust-and-react/?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)
-   📜 [Create powerful and flexible forms with React Hook Form](https://daily.dev/blog/create-powerful-and-flexible-forms-with-react-hook-form?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)
-   📜 [Exploring React Suspense with React Freeze](https://blog.logrocket.com/exploring-react-suspense-react-freeze/?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)
-   💡 [Gatsby RFC: GraphQL TypeScript Generation](https://github.com/gatsbyjs/gatsby/discussions/35420?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)
-   🐦 [`next/link` will no longer require `<a>` as a child](https://twitter.com/timneutkens/status/1518595962322792448?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter): looks like a nice quality of life improvement 😉
-   🐦 [React + Qwik](https://twitter.com/Steve8708/status/1517953640673124352?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)
-   🧵 [Sebastian Markbåge: "Hydration in React was originally not built for SSR"](https://twitter.com/sebmarkbage/status/1516907614566854659?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter): there's been interesting hydration discussions this week, probably in reaction to this [Misko Hevery article](https://twitter.com/mhevery/status/1516844814792224770?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter) (creator of Qwik/Angular)
-   🧵 [Alex Russell on CSS-in-JS](https://twitter.com/slightlylate/status/1517173350467993600?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter): fair criticism of runtime-based CSS-in-JS libs
-   📦 [Create-React-App Redux Template v2](https://github.com/reduxjs/cra-template-redux/releases/tag/v2.0.0?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter): update React 18
-   📦 [Jest-Preview](https://github.com/nvh95/jest-preview?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter): new solution that integrates with React-Testing-Library to visually see your tests run and debug them more easily.
-   📦 [Rive-React](https://github.com/rive-app/rive-react?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter): React bindings for the [Rive](https://rive.app/?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter) animation platform
-   📦 [Jotai-form](https://twitter.com/dai_shi/status/1518562466627821570?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)
-   📦 [MDX-to-MD](https://github.com/souporserious/mdx-to-md?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)
-   🎥 [The Official Beginner's Guide to XState in React](https://www.youtube.com/watch?list=PLvWgkXBB3dd4ocSi17y1JmMmz7S5cV8vI&utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter&v=_5dAlGaqhck)
-   🎥 [React for the Haters in 100 Seconds](https://www.youtube.com/watch?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter&v=HyWYpM_S-2c)
-   🎥 [Redux in 100 Seconds](https://www.youtube.com/watch?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter&v=_shA5Xwe8_4)


## React-Native

[**Migrating React And Native Apps To React Native**](https://www.callstack.com/blog/migration-to-react-native?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)

Callstack工程师解释了如何为现有的应用程序采用React-Native，有两种不同的方法：greenfield（完全重写）和brownfield（增量迁移）。还唤起了如何将一个Web应用移植到React-Native。

[**Writing cross-platform components for web and React Native**](https://blog.sapegin.me/all/react-native-components/?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)

Artem gives some ideas for cross-platform web/mobile development. He suggests using primitive components, and taking a web-first approach for DX reasons: developing in the browser and testing with Cypress, then verifying that the mobile app works.

Artem给出了一些关于跨平台的网络/移动开发的想法。他建议使用原始组件，并出于DX的原因采取网络优先的方法：在浏览器中开发，用Cypress进行测试，然后验证移动应用是否正常。

**拓展阅读**

-   📜 [Use Storybook with Nx React Native](https://blog.nrwl.io/use-storybook-with-nx-react-native-2ddd8c010eda?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)
-   🎙️ [React-Native-Radio 232 - Flutter is better than React Native...in all the ways that don't matter](https://reactnativeradio.com/episodes/rnr-232-flutter-is-better-than-react-nativein-all-the-ways-that-dont-matter?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)
-   🎙️ [The React Native Show Podcast: Coffee Talk #1 - React v18.0 & React Native 0.68](https://twitter.com/callstackio/status/1517517170384719873?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)
-   👥 [React-Native EU](https://www.react-native.eu/?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter): [Call-For-Papier](https://docs.google.com/forms/d/e/1FAIpQLSdknyrQo6OVw-YgvExtFOH0xYaejKSf_R29ltQp2ghXXgWMYg/viewform?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter) open until end of Mai
-   📦 [React-Native V8 1.0](https://github.com/Kudo/react-native-v8/releases/tag/v1.0.0?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)

## 其它

[**Jest 28: Shedding weight and improving compatibility**](https://jestjs.io/blog/2022/04/25/jest-28?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)

这个版本有很多很酷的东西! 我的关注点：

- 支持分片，使测试执行并行化
- 完全支持包的 `"exports"`
- GitHub Actions Reporter看起来非常方便
- ESM支持仍然受限
- [jest-runner-tsd](https://github.com/jest-community/jest-runner-tsd?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)：用于测试TypeScript类型
- [jest-light-runner](https://github.com/nicolo-ribaudo/jest-light-runner?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)：在Babel代码库上快2倍。

[**Building a JavaScript Bundler**](https://cpojer.net/posts/building-a-javascript-bundler?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)

Christoph Nakazawa解释了如何在一些现有的Jest包基础上创建一个JavaScript bundler。读取JavaScript文件，创建依赖关系图，捆绑运行时，最终的捆绑装配...... 这是一本技术读物，极大地解开了一个简单的bundler的内部工作原理。

[**Netlify Edge Functions (beta)**](https://www.netlify.com/blog/announcing-serverless-compute-with-edge-functions?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)

After a failed attempt (Edge Handlers), Netlify releases a new serverless @ Edge offer with its Edge Functions in beta, based on the [Deno Deploy](https://deno.com/blog/netlify-edge-functions-on-deno-deploy?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter) infrastructure, and thus more compatible with web standard APIs. This allows in particular to run React meta-frameworks using server-side code more optimally: Remix, Next.js (only middleware for now), Hydrogen, Server Components, Astro...

在一次失败的尝试（Edge Handlers）之后，Netlify发布了一个新的无服务器产品，其Edge功能处于测试阶段，基于[Deno Deploy](https://deno.com/blog/netlify-edge-functions-on-deno-deploy?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)基础设施，因此与Web标准API更加兼容。这特别允许使用服务器端代码更优化地运行React元框架。Remix、Next.js（目前只有中间件）、Hydrogen、服务器组件、Astro...

[**Hydration is Pure Overhead**](https://www.builder.io/blog/hydration-is-pure-overhead?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)


Qwik/Angular的创建者继续质疑我们服务器端渲染的SPA的水化模型，并推动采用另一种更有效的模型，基于 "恢复性"。

**拓展阅读**

-   [Marko: Compiling Fine-Grained Reactivity](https://dev.to/ryansolid/marko-compiling-fine-grained-reactivity-4lk4?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)
-   [Marko for Sites, Solid for Apps](https://dev.to/this-is-learning/marko-for-sites-solid-for-apps-2c7d?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)
-   [Progressive Enhancement and HTML Forms: use FormData](https://www.bram.us/2022/04/22/progressive-enhancement-and-html-forms-use-formdata/?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)
-   [Island Architecture](https://mainawycliffe.dev/blog/island-architecture/?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)
-   [V8 - Faster initialization of instances with new class features](https://v8.dev/blog/faster-class-features?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)
-   [Learn PWA](https://web.dev/learn/pwa/?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)
-   [Div Riots: Our experience with Astro](https://divriots.com/blog/our-experience-with-astro?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)
-   [The Future of CSS: CSS Toggles](https://www.bram.us/2022/04/20/the-future-of-css-css-toggles/?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)
-   [TypeScript and Set Theory](https://ivov.dev/notes/typescript-and-set-theory?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)
-   [JSDB: Use javascript as your database](https://javascriptdb.com/?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)
-   [SvelteKit can now run on Vercel Edge Functions](https://twitter.com/leeerob/status/1517627769924034565?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)
-   [How to Use Next.js Middleware on Netlify](https://www.netlify.com/blog/next.js-middleware-on-netlify?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)
-   [Vitest VS Code Extension](https://twitter.com/vitest_dev/status/1517896780016676865?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)
-   [Nx 14.0](https://github.com/nrwl/nx/releases/tag/14.0.0?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)
-   [Deno 1.21](https://deno.com/blog/v1.21?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)
-   [Parcel 2.5](https://twitter.com/parceljs/status/1517170101799337985?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)
-   [ESLint 8.14](https://eslint.org/blog/2022/04/eslint-v8.14.0-released?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)
-   [Vitest 0.10](https://twitter.com/vitest_dev/status/1518600493614120965?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)

 <img width="687" alt="CleanShot 2022-04-27 at 11 19 35@2x" src="https://user-images.githubusercontent.com/749374/165486018-464fd017-cc65-45f5-985d-27294896cb9d.png">
 
  ---
  
  订阅原文:
-   🇬🇧 [ThisWeekInReact.com](https://thisweekinreact.com/)
-   🇫🇷 [ReactHebdo.fr](https://reacthebdo.fr/)
