This Week In React #96: Next.js, Gatsby, Remix, Remotion, React-Native, Glassmorphism, Deno, TypeScript, Qwik...
===

Hi everyone!

It has been a tough week. Not easy to focus on React content when terrible war videos are everywhere on Twitter. To provide direct financial support to Ukraine: go to an **official website** such as [Ukraine.ua](https://war.ukraine.ua/?utm_campaign=React%20Hebdo&utm_medium=email&utm_source=Revue%20newsletter), or be vigilant (many scams...). I choose [UNHCR](https://donner.unhcr.org/urgence-ukraine/~mon-don?utm_campaign=React%20Hebdo&utm_medium=email&utm_source=Revue%20newsletter) because French gov matches x4 the donation.

This week remains interesting in terms of content.

I created a Twitter community [This Week In React](https://twitter.com/i/communities/1498347452826537990?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter) to test the new Twitter feature, I don't know yet what will come out of it. Do not hesitate to join and we'll figure out.

🙏 **Support the newsletter:**

-   😘 **Recommend it to your friends**: it really helps!
-   💸 [**Sponsorise This Week In React**](https://gist.github.com/slorber/cb732fb5d0a002c4d73236a9baeba7bb?utm_campaign=thisweekinreact&utm_medium=email&utm_source=Revue%20newsletter)
-   😍 [**Write testimonials on Twitter**](https://twitter.com/sebastienlorber/timelines/1448942785814466561?utm_campaign=thisweekinreact&utm_medium=email&utm_source=Revue%20newsletter)
-   🧵 [**Retweet the latest Twitter thread**](https://slo.im/thread?utm_campaign=thisweekinreact&utm_medium=email&utm_source=Revue%20newsletter)
-   📨 Reply to this [**email**](mailto:lorber.sebastien@gmail.com?utm_campaign=thisweekinreact&utm_medium=email&utm_source=Revue%20newsletter): feedback is welcome

[![](https://user-images.githubusercontent.com/749374/153181021-8fdb0ece-270a-4cf2-980b-4557d04316ad.png)](https://thisweekinreact.com)

## React

[**Comparing Gatsby and Next.js for website development**](https://dev.to/alex_barashkov/comparing-gatsby-and-nextjs-for-website-development-13b7?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)

Alex explains why his agency prefers Gatsby over Next.js for website development. It's pretty well argued. Gatsby is not very fashionable at the moment but I think it's still a good solution to ship a website quickly and easily integrate with a CMS out-of-the-box.

[**Optimizing third-party script loading in Next.js**](https://web.dev/script-component/?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)

Presentation of the work of the Aurora team at Google who worked on the `<Script>` component of Next.js, optimizing the loading of third-party scripts. There may be an upcoming integration with [Partytown](https://partytown.builder.io/?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter), to run these scripts in a worker.

[**Moving from Next to Remix**](https://www.adamcollier.co.uk/blog/moving-from-next-to-remix?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)

Adam shares his motivations for migrating his site from Next.js to Remix, as well as many other details (Prisma, Planetscale, UnoCSS...). Next.js remains a good choice. He really likes how Remix handle forms.

[**Interaction Testing with Storybook**](https://storybook.js.org/blog/interaction-testing-with-storybook/?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)

Storybook now offers an interaction testing system (beta) co-located with stories to test components with Jest, Playwright and Testing Library. That looks quite convenient.

**Extras:**

-   🐦 [React-18 RC1](https://twitter.com/acdlite/status/1497662815519260678?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter): should be released soon
-   🐦 [Rachel Nabors leaves the React team at Meta](https://twitter.com/rachelnabors/status/1497179514773942272?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter) after greatly contributing to the [new beta React docs site](https://beta.reactjs.org/?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter) and React-Native docs.
-   💬 Mark Erikson suggests to create a [React Docs Working Group](https://github.com/reactjs/reactjs.org/issues/3308?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter#issuecomment-1051055907).
-   📜 [A Fundamental Guide To React Suspense](https://www.chakshunyu.com/blog/a-fundamental-guide-to-react-suspense/?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)
-   📜 [Share session and cookies between Next and Remix](https://sergiodxa.com/articles/share-session-and-cookies-between-next-and-remix?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter#share-session-and-cookies-between-next-and-remix)
-   📜 [Higher-Order Components in React Hooks era](https://www.developerway.com/posts/higher-order-components-in-react-hooks-era?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)
-   📜 [Doordash: Building a Marketing Engineering Platform using Next.js, Cloudflare, and Contentful](https://doordash.engineering/2022/02/22/building-a-marketing-engineering-platform-using-next-js-cloudflare-and-contentful/?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)
-   👥 [GatsbyConf 2022](https://gatsbyconf.com/?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter): 2-3 March
-   🎥 [Figma + Remotion](https://twitter.com/JNYBGR/status/1496748768821133312?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)
-   📦 [Redux Toolkit 1.8](https://github.com/reduxjs/redux-toolkit/releases/tag/v1.8.0?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter): listener side-effect middleware inspired by Redux-Saga: dispatch actions in reaction to other actions
-   📦 [Gatsby 4.8](https://www.gatsbyjs.com/docs/reference/release-notes/v4.8/?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter) + [Gatsby 4.9](https://www.gatsbyjs.com/docs/reference/release-notes/v4.9/?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter): improves TypeScript support, reduces memory footprint
-   📦 [Docusaurus 2.0 beta.16](https://twitter.com/docusaurus/status/1497227180295823366?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter): swizzle CLI, breadcrumbs...
-   📦 [GraphCMS Docs Starter](https://graphcms.com/blog/announcing-graphcms-docs-starter?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter): Remix + Tailwind
-   📦 [Headless UI 1.5](https://tailwindcss.com/blog/headless-ui-v1-5?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter): with Combobox
-   📦 [Radix UI](https://twitter.com/radix_ui/status/1498331815781842947?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter): release with Select, NavigationMenu and Toast
-   📦 [Remix 1.2.3](https://twitter.com/remix_run/status/1498453130458976258?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)

## React-Native

[**React Native New Architecture Working Group**](https://github.com/reactwg/react-native-new-architecture?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)

GitHub discussions repo to support the rollout of the new React-Native architecture. Read-only but possible to request an invitation. Quite similar to the React-18 Working Group. Already a few interesting subjects under discussion.

**Extras:**

-   🐦 [React-Native 0.68](https://twitter.com/reactnative/status/1497273574784073729?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter): pre-release announced as available (now in [RC2](https://github.com/facebook/react-native/releases/tag/v0.68.0-rc.2?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter))
-   🎥 [Glassmorphism in React Native](https://www.youtube.com/watch?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter&v=ao2i_sOD-z0): last Skia video from William Candillon, nice demos of what is now possible in React-Native using blur/backdrop filters
-   🎙️ [RNR 227 - Better React Native Tooling with Tommy Nguyen and Adam Foxman](https://reactnativeradio.com/episodes/rnr-227-better-react-native-tooling-with-tommy-nguyen-and-adam-foxman?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter): Microsoft engineers presenting [rnx-kit](https://github.com/microsoft/rnx-kit?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)


## Other

[**How to publish Deno modules to NPM**](https://deno.com/blog/dnt-oak?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)

Kitson introduces [dnt](https://github.com/denoland/dnt/?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter), a tool for transforming Deno code into Node.js compatible code. They managed to publish the Deno [oak](https://github.com/oakserver/oak?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter) http framework on npm, but it is not without any challenges. I find this very encouraging: it should drive incremental adoption of Deno. As a TypeScript library author, I definitively want to target both ecosystems so that's a really good incentive to give Deno a try on a small lib.

[**Why Progressive Hydration is Harder than You Think**](https://www.builder.io/blog/why-progressive-hydration-is-harder-than-you-think?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)

Miško Hevery is the creator of Angular, he is now working on [Qwik](https://github.com/BuilderIO/qwik?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter), a new generation framework with a strong focus on progressive hydration. It will be difficult for current existing frameworks to fully support this concept without changing mental models. It's not an afterthought for Qwik, unlike other frameworks.

**Extras:**

-   [TypeScript 4.6](https://devblogs.microsoft.com/typescript/announcing-typescript-4-6/?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter): with [great Control Flow Analysis improvements](https://twitter.com/sebastienlorber/status/1498584209375518726?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)
-   [Type Polymorphic Functions In TypeScript](https://www.zhenghao.io/posts/type-functions?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)
-   [What are wrapper objects for primitive values?](https://2ality.com/2022/02/wrapper-objects.html?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)
-   [5 things you don't need Javascript for](https://lexoral.com/blog/you-dont-need-js/?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)
-   [Track down the JavaScript code responsible for polluting the global scope](https://mmazzarolo.com/blog/2022-02-16-track-down-the-javascript-code-responsible-for-polluting-the-global-scope/?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)
-   [State of frontend 2022 Survey](https://tsh.io/state-of-frontend/?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)
-   [Parcel CSS 1.4](https://twitter.com/devongovett/status/1496516023775903745?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)
-   [*"Nice, the CSS on the webpack website is now minified by Parcel CSS."*](https://twitter.com/devongovett/status/1497282820443713537?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)
-   [Things the CSS Spec Folks Got Right](https://blog.jim-nielsen.com/2022/things-the-css-spec-folks-got-right/?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)
-   [Rust 1.59.0](https://blog.rust-lang.org/2022/02/24/Rust-1.59.0.html?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)
-   [Node v17.6.0](https://nodejs.org/en/blog/release/v17.6.0/?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)
-   [Vite in 100 seconds](https://www.youtube.com/watch?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter&v=KCrXgy8qtjM)
-   [Astro 0.23](https://astro.build/blog/astro-023/?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)
-   [Prisma 3.10](https://twitter.com/prisma/status/1496166878506631173?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)
-   [Javascript Records and Tuples](https://fjolt.com/article/javascript-records-and-tuples?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)
-   [Putting Javascript in CSS with Paint Worklets](https://fjolt.com/article/javascript-putting-js-in-css?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)
-   [Zap: Dart-powered web framework](https://simonbinder.eu/zap/?utm_campaign=This%20Week%20In%20React&utm_medium=email&utm_source=Revue%20newsletter)


<img width="691" alt="image" src="https://user-images.githubusercontent.com/749374/156231195-b778b71b-8e36-4e83-93f2-990cdf14f395.png">
