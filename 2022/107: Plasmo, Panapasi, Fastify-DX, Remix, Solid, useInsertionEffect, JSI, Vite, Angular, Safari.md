This Week In React #107: Plasmo, Panapasi, Fastify-DX, Remix, Solid, useInsertionEffect, JSI, Vite, Angular, Safari...

## React

[**Plasmo - Like Next.js for browser extensions!**](https://github.com/PlasmoHQ/plasmo?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)

一个专注于创建浏览器扩展程序的新框架，基于React和TypeScript。开源的、免费的，它提供付费的CI/CD云服务。

[**Panapasi - The Universal UI Library**](https://papanasi.js.org/?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)

我们看到越来越多的UI库希望提供原生的跨框架支持（见Chakra、TanStack库...）。据我所知，Panapasi是第一个基于[Mitosis](https://github.com/BuilderIO/mitosis?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)的项目，它将JSX Lite语言编译到目标框架中。

[**Fastify DX for React**](https://github.com/fastify/fastify-dx/blob/main/packages/fastify-dx-react/README.md?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)

正在开发中的新全栈框架，基于Fastify和Vite。不可知性：可以适应多个框架（React、Vue、Solid...）。React集成目标在于成为Next.js和Remix的轻量级替代品，基于React-Router和Valtio。

[**Converting a React Component to SolidJS**](https://dev.to/mbarzeev/converting-a-react-component-to-solidjs-5bgj?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)

将一个分页组件从React转换为Solid。很多JSX代码都可以照搬，但钩子必须稍作调整。Solid代表了一种真正的创新：代码最后看起来很像React（没有依赖阵列😏），但执行模型是反应式的。

[**Redux Toolkit's new listener middleware vs. Redux-Saga**](https://blog.logrocket.com/redux-toolkits-new-listener-middleware-vs-redux-saga/?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)

新的RTK监听器系统与Redux Saga的良好的侧面比较。比较了许多用例的实现。RTK Listener似乎是Redux-Saga的一个很好的轻量级替代品，学习曲线相对较低。这是一个很好的资源，可以选择一个或另一个，或计划一个迁移。

[**React 18 useEffect Double Call for APIs: Emergency Fix**](https://javascript.plainenglish.io/react-18-useeffect-double-call-for-apis-emergency-fix-724b7ee6a646?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)

Jack给出了6种可能的解决方案，以避免React 18的StrictMode出现双重查询问题。使用像React-Query或RTK-Query（嗯，TanStack Query 😏）这样的lib似乎是最简单的。

**拓展阅读**

-   📖 [Second draft of the useEffect guide](https://twitter.com/dan_abramov/status/1532754556488146947?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter): new beta doc
-   📜 [Remix-ing Routing in Angular](https://dev.to/brandontroberts/remix-ing-routing-in-angular-4g90?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter): Remix is ​​framework-agnostic. Brandon shows how it can be integrated with the brand new Angular v14.
-   📜 [Setting up a dev environment with React, Vite, and Tailwind](https://blog.logrocket.com/setting-up-dev-environment-react-vite-tailwind/?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter): highlights the advantages of Vite over Webpack/CRA.
-   📜 [Know about the useInsertionEffect hook in React 18](https://blog.saeloun.com/2022/06/02/react-18-useinsertioneffect?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter): presentation of a hook intended for authors of CSS-in-JS libs. Allows styles to be inserted at the best time.
-   📜 [Modulz has been acquired by WorkOS](https://modulz.app/blog/modulz-acquired-by-workos?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter): gives details on the maintenance of their popular React libs Radix and Stitches.
-   📜 [The Case For Prisma In The Jamstack](https://www.smashingmagazine.com/2022/06/case-prisma-jamstack/?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter): explains the interest of combining Prisma with various frameworks like Next.js or Redwood.
-   🐦 [React Server Components + SSG/ISR](https://twitter.com/sebmarkbage/status/1532755826850537475?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter): it will be possible to use Server Components with static generation: the SSG framework will output static `.rsc` files.
-   🐦 [useRef<HTMLElement> + TypeScript contravariance](https://twitter.com/sebastienlorber/status/1533799576985124865?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter): my analysis + 2 suggested solutions.
-   🐦 [CSS @scope + React](https://twitter.com/sebastienlorber/status/1533767305875824641?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter): upcoming CSS feature that could be useful for the React component model and encapsulation
-   📦 [TanStack](https://tanstack.com/?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter): TanStack libs are gradually becoming framework-agnostic! TanStack Query, TanStack Virtual, TanStack Table...
-   📦 [Remix-Flat-Routes](https://github.com/kiliman/remix-flat-routes?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter): package to support a flat file-system routing convention for Remix. Gives good arguments for using it.
-   📦 [Jest-Image-Snapshot](https://github.com/americanexpress/jest-image-snapshot?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter): visual regression testing tool. New v5 upgrades to Jest 28. Best used with [Storybook StoryShots](https://github.com/storybookjs/storybook/tree/main/addons/storyshots/storyshots-core?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter).
-   📦 [Recoil Relay 0.1.0](https://recoiljs.org/blog/2022/06/02/recoil-relay-0.1.0-release?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)
-   🎥 [Redwood in 100 Seconds](https://www.youtube.com/watch?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter&v=o5Mwa_TJ3HM)


## React-Native

[**React Native JSI/TurboModules pitfalls**](https://ospfranco.com/post/2022/06/05/jsi-pitfalls/?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)
  
Oscar拥有丰富的JSI经验：他是React-Native包的作者，也是[Youtube上专门介绍JSI的播放列表](https://www.youtube.com/watch?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter&v=DA3KXef81sg)。他给了我们一些有趣的反馈，比如在原生端使用各种语言，或者与旧的桥梁架构相比，很难对JSI进行适当的基准测试。

**拓展阅读**

-   🧵 [React-Native @ Shopify](https://twitter.com/fnthawar/status/1532054866788593665?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter): VP Engineering at Shopify gives update on internal usage, and the significant Shopify contribution in the ecosystem.
-   🐦 [It's Flutter but in React Native... but in ReactJS...](https://twitter.com/chrfalch/status/1534145338935853056?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter): React-Native-Skia also works on the web thanks to Flutter [CanvaKit](https://skia.org/docs/user/modules/canvaskit/?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)
-   🐦 [Multiplying 2 numbers: React-Native bridge vs JSI benchmark](https://twitter.com/LinguaBrowse/status/1533011223729807361?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)
-   📦 [react-native-lightbox](https://github.com/alantoa/react-native-lightbox?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)

## 其它

[**WebContainers are now supported in Firefox**](https://blog.stackblitz.com/posts/webcontainers-are-now-supported-on-firefox/?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)
  
StackBlitz的这项创新允许你直接在浏览器中运行Node.js代码，包括Next.js、Remix、Docusaurus等React框架。它刚刚通过这个新的Firefox支持实现了一个大飞跃（除了Chrome）。

**拓展阅读**

-   [WebKit Features in Safari 16 Beta](https://webkit.org/blog/12824/news-from-wwdc-webkit-features-in-safari-16-beta/?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter): CSS Container Queries, Web Push (in 2023) 🤯
-   [Safari Technology Preview 146](https://webkit.org/blog/12745/release-notes-for-safari-technology-preview-146/?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter): with [Change Array by Copy](https://twitter.com/robpalmer2/status/1532674320350191616?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter) ❤️️
-   [You may not need a bundler for your NPM library](https://cmdcolin.github.io/posts/2022-05-27-youmaynotneedabundler?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)
-   [Using yup and typescript for typesafe select validation](https://yidaotus.medium.com/using-yup-and-typescript-for-typesafe-select-validation-e9ee9d4bceec?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)
-   [Angular 14](https://blog.angular.io/angular-v14-is-now-available-391a6db736af?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)
-   [Node.js 18.3 parseArgs](https://twitter.com/simonplend/status/1532304908585779201?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)
-   [Chrome - How and why we built Performance Insights](https://developer.chrome.com/articles/performance-insights/?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)
-   [WebPageTest - Opportunities & Experiments](https://blog.webpagetest.org/posts/introducing-opportunities-and-experiments/?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)
-   [Why most design systems implode](https://storybook.js.org/blog/why-most-design-systems-implode/?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)
  
 
 <img width="476" alt="CleanShot 2022-06-08 at 00 06 57@2x" src="https://user-images.githubusercontent.com/749374/172491158-f06941a4-6948-4732-96b4-1c067241bd50.png">
  
    
  订阅原文:
-   🇬🇧 [ThisWeekInReact.com](https://thisweekinreact.com/)
-   🇫🇷 [ReactHebdo.fr](https://reacthebdo.fr/)
 
