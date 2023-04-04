## Official Links

[Website](https://astro.build/) | [Documentation](https://docs.astro.build/en/getting-started/) | [Integrations](https://astro.build/integrations/) | [Themes](https://astro.build/themes/) | [Blog](https://astro.build/blog/) | [Showcase](https://astro.build/showcase/)
---|---|---|---|---|---

[Repository](https://astro.build/on/github) | [Changelog](https://github.com/withastro/astro/blob/main/packages/astro/CHANGELOG.md) | [Docs Repository](https://github.com/withastro/docs) | [RFC Repository](https://github.com/withastro/rfcs) | [Roadmap](https://github.com/orgs/withastro/projects/11)
---|---|---|---|---

[Templates](https://astro.new/) | [Huoston](https://houston.astro.build/) | [Badges](https://astro.badg.es/) | [Hyperdrive Speedometer](https://hyperdrive-speedometer.netlify.app/) | [VS Code Theme](https://marketplace.visualstudio.com/items?itemName=astro-build.houston)
---|---|---|---|---

[Discord](https://astro.build/chat) | [Twitter](https://astro.build/on/twitter) | [Youtube](https://www.youtube.com/@astrodotbuild) | [Mastadon](https://m.webtoo.ls/@astro) | [Open Collective](https://opencollective.com/astrodotbuild)
---|---|---|---|---

## Support

Need help? [Join the Discord](https://astro.build/chat) and create a post in the [`#support`](https://discord.com/channels/830184174198718474/1019713903481081876) channel

## Resources
### [FAQ](/FAQ.md)
### [Youtube](/YOUTUBE.md)
### [Blogs](/BLOGS.md)
### [Examples](/EXAMPLES.md)

## What Do I Use...

### If I want to add a font?

[Using Custom Fonts](https://docs.astro.build/en/guides/fonts/)

- [Fontsource](https://docs.astro.build/en/guides/fonts/#using-fontsource) - Self-host Open Source fonts in neatly bundled NPM packages, faster than Google Fonts
  - [Fontsource’s catalog](https://fontsource.org/fonts) - Catalog of all fonts supported by Fontsource
- [astro-google-fonts-optimizer](https://github.com/sebholstein/astro-google-fonts-optimizer) - Component, downloads the CSS of a Google Fonts stylesheet and inlines it directly into the page, inspired by [NextJS font optimization](https://nextjs.org/blog/next-10-2#automatic-webfont-optimization)
- [astro-fonts-next](https://github.com/dc7290/astro-fonts-next) - Integration, applies [NextJS font optimization](https://nextjs.org/blog/next-10-2#automatic-webfont-optimization) to Google Fonts

### If I want to add icons?

- [astro-icon](https://github.com/natemoo-re/astro-icon) - (Un)Official `<Icon>` component powered by [Iconify](https://iconify.design/)
  - [Icon set reference](https://icon-sets.iconify.design/) - List of available icons
  - [Icônes](https://icones.js.org/) - Tool for exploring and downloading icons
  - [Iconify Components](https://docs.iconify.design/develop/) - Official [Iconify](https://iconify.design/) components
- [astro-feather-icons](https://github.com/edazpotato/astro-feather-icons) - Icon components for [Feather icons](https://feathericons.com/)
- [astro-heroicons](https://github.com/seanmcp/astro-heroicons) - Icon components for [Heroicons](https://heroicons.com/)
- [@astropub/icons](https://github.com/astro-community/icons) - Icon components for [Radix icons](https://icons.radix-ui.com/)
- [phosphor-astro](https://github.com/seanmcp/phosphor-astro) - Icon components for [Phosphor icons](https://phosphoricons.com/)
- [astro-svg-loaders](https://github.com/codiume/orbit/tree/main/packages/astro-svg-loaders) - Icon components for [svg loading icons by @SamHerbert](https://github.com/SamHerbert/SVG-Loaders)
- [astro-emoji](https://github.com/seanmcp/astro-emoji) Create accessible emojies

### If I want to add SEO?

- [astro-seo](https://github.com/jonasmerlin/astro-seo) - (Recommended) Most popular `<SEO>` component
- [@astrolib/seo](https://github.com/onwidget/astrolib/tree/main/packages/seo) - Based on [NextSEO](https://github.com/garmeeh/next-seo)
- [astro-seo-meta](https://github.com/codiume/orbit/tree/main/packages/astro-seo-meta) - Minimal SEO component
- [simple-astro-seo](https://github.com/perkinsjr/simple-astro-seo) - Minimal SEO component
- [astro-seo-metadata](https://github.com/JulianCataldo/web-garden/tree/develop/app/SEOMetadata) - Minimal SEO component

### If I want to create open graph images?

[Open Graph Protocol](https://ogp.me/)

- [satori-html](https://github.com/natemoo-re/satori-html) - Create og images using html strings and [satori](https://github.com/vercel/satori)
  - [Dynamic OG images using Satori and Astro Server Endpoints - Rumaan K](https://rumaan.dev/blog/open-graph-images-using-satori)
  - [Recreating Vercel's OG Image Generation - Otterlord](https://blog.otterlord.dev/post/dynamic-opengraph/)
- [@vercel/og](https://vercel.com/docs/concepts/functions/edge-functions/og-image-generation) - Vercel's official open graph image generation using [satori](https://github.com/vercel/satori)
  - [Adding Vercel og:image generation to Astro project with Edge functions - Thomas Ledoux](https://dev.to/thomasledoux1/adding-vercel-ogimage-generation-to-astro-project-with-edge-functions-4mj2)
- [astro-og-canvas](https://github.com/delucis/astro-og-canvas/tree/latest/packages/astro-og-canvas) - This package provides utlities for generating OpenGraph images
- [astro-og-image](https://www.npmjs.com/package/astro-og-image) - Screenshot pages as open graph images

[Tool for previewing open graph images and meta tags](https://www.opengraph.xyz/)

### If I want to add optimized images?

- [@astrojs/image](https://docs.astro.build/en/guides/integrations-guide/image/) - Official image optimization integration
- [astro-imagetools](https://github.com/RafidMuhymin/astro-imagetools) - Community image optimization integration
- [astro-eleventy-img](https://github.com/Princesseuh/astro-eleventy-img) - Generate images using [eleventy-img](https://github.com/11ty/eleventy-img)
- [astro-imagekit](https://www.npmjs.com/package/astro-imagekit) - An opinionated toolset for using ImageKit.io with your Astro website

### If I want to use relative images in my markdown?

- [Siena](https://github.com/pilcrowOnPaper/siena) - A Rehype plugin for Astro that makes working with images inside markdown easier
- [astro-m2dx](https://www.npmjs.com/package/astro-m2dx#relative-images) - Resolve relative image references in MDX files, and tons more
- [astro-md-image-integration](https://github.com/userquin/astro-md-image-integration) - Use images outside of `/src`, [example](https://github.com/withastro/roadmap/discussions/334)

### If I want to render a string of markdown?

[Fetching Remote Markdown](https://docs.astro.build/en/guides/markdown-content/#fetching-remote-markdown)

- [astro-remote](https://github.com/natemoo-re/astro-remote) - (Recommended) SSR, render remote markdown content in Astro with full control over the output including adding components. Does not inherit markdown setttings from Astro config
- [@astropub/md](https://github.com/astro-community/md) - (Recommended) SSG, render markdown using settings defined in Astro config
  - [@astrojs/markdown-remark](https://github.com/withastro/astro/blob/52209ca2ad72a30854947dcb3a90ab4db0ac0a6f/packages/markdown/remark/src/index.ts#L42) - SSG, Astro's built in markdown rendering library, exports a `renderMarkdown()` utility
- [@astrojs/markdown-component](https://github.com/withastro/astro/tree/main/packages/markdown/component) - SSG, Official `<Markdown>` component

### If I want to style my markdown?

- [Global Styling](https://docs.astro.build/en/guides/styling/#global-styles) - Use global vanilla css styling
- [@tailwindcss/typography](https://tailwindcss.com/docs/typography-plugin) - Official tailwind plugin for styling markdown
- [Tailwind @apply directive](https://tailwindcss.com/docs/functions-and-directives#apply) - Create global tailwind styles using @apply directive
- [rehype-add-classes](https://github.com/martypdx/rehype-add-classes) - Markdown plugin that lets you add classes(tailwind) to selectors

### If I want to use a CSS framework?

- [astro-cube](https://github.com/williamhzo/astro-cube) - Starter template for [CUBE CSS](https://cube.fyi/)
- [Tailwindcss](https://docs.astro.build/en/guides/integrations-guide/tailwind/) - [Documentation](https://tailwindcss.com/docs/configuration)
- [UnoCSS](https://github.com/unocss/unocss) - [Documentation](https://uno.antfu.me)
- [Vanilla Extract](https://github.com/codiume/orbit/tree/main/packages/astro-vanilla-extract) - [Documentation](https://vanilla-extract.style/documentation/getting-started)
  - [Astro Vanilla-Extract Styling: CSS in TypeScript](https://dev.to/askrodney/astro-vanilla-extract-styling-css-in-typescript-35f)
- [Windi CSS](https://github.com/Dv-Dn/astro-integration-windicss) - [Documentation](https://windicss.org/guide/)
- [Stylify](https://stylifycss.com/docs/integrations/astro) - [Documentation](https://stylifycss.com/docs/get-started)
  - [Stylify CSS: Automagic CSS bundles splitting into CSS layers in Astro.build](https://dev.to/machy8/stylify-css-automagic-css-bundles-splitting-into-css-layers-in-astrobuild-3po9)

### If I want to add client side interactivity?

[Client Side Scripting Guide](https://docs.astro.build/en/guides/client-side-scripts/)

[UI Frameworks](https://docs.astro.build/en/core-concepts/framework-components/)

- [`<script>`](https://docs.astro.build/en/core-concepts/astro-components/#client-side-scripts)
- [Web components](https://docs.astro.build/en/guides/client-side-scripts/#web-components-with-custom-elements)
  - [astro-xelement](https://github.com/aFuzzyBear/xelement) - Create web components natively in Astro
- [SolidJS](https://docs.astro.build/en/guides/integrations-guide/solid-js/)
- [Preact](https://docs.astro.build/en/guides/integrations-guide/preact/)
- [Lit](https://docs.astro.build/en/guides/integrations-guide/lit/)
- [Svelte](https://docs.astro.build/en/guides/integrations-guide/svelte/)
- [Vue](https://docs.astro.build/en/guides/integrations-guide/vue/)
- [React](https://docs.astro.build/en/guides/integrations-guide/react/)
- [AlpineJS](https://docs.astro.build/en/guides/integrations-guide/alpinejs/)

[Size comparison of UI Frameworks](https://dev.to/this-is-learning/javascript-framework-todomvc-size-comparison-504f)

### If I want to share state between components?

[Sharing State](https://docs.astro.build/en/core-concepts/sharing-state/)

- [nanostores](https://github.com/nanostores/nanostores) - Currently reccomended by Astro, can be used between React, React Native, Preact, Vue, Svelte, and vanilla JavaScript
  - [@nanostores/persistent](https://github.com/nanostores/persistent) - Persist nanostores between pages using localStorage
  - [How to manage state in Astro applications? - CodeWithLuke](https://www.youtube.com/watch?v=R3N_zg7Lz6Q)
- [Svelte stores](https://svelte.dev/docs#run-time-svelte-store) - Share state between Svelte components
- [SolidJS signal](https://www.solidjs.com/docs/latest#createsignal) - SolidJS signals can be used in the frontmatter of `.astro` files
- [Custom Event](https://developer.mozilla.org/en-US/docs/Web/Events/Creating_and_triggering_events) - Use vanilla JavaScript to send custom events

### If I want to add the ability to search?

- [Pagefind](https://pagefind.app/)
  - [Add Searching To Your Astro Static Site - Otterlord](https://blog.otterlord.dev/post/astro-search/)
  - [Pagefind is quite a find for site search - Bryce Wray](https://www.brycewray.com/posts/2022/07/pagefind-quite-find-site-search/)
  - [Sweeter searches with Pagefind - Bryce Wray](https://www.brycewray.com/posts/2022/12/sweeter-searches-pagefind/)
- [@lyrasearch/plugin-astro](https://github.com/LyraSearch/plugin-astro) - Astro integration for [Lyra](https://lyrajs.io/) search
- [astro-lunr](https://github.com/jackcarey/astro-lunr) - Astro integration for [Lunr](https://github.com/siverv/astro-lunr) search
- [@barnabask/astro-minisearch]() - Build an index from markdown and search it using [MiniSearch](https://github.com/lucaong/minisearch)
  - [Client-Side Search -Barnabas Kendall](https://barnabas.me/articles/client-side-search/)
 
 <br>

- [fuse.js](https://fusejs.io/) - Powerful lightweight fuzzy-search library with zero dependencies
  - [Writing a Fuzzy Search Component With Preact and Fuse for Astro - Lloyd Atkinson](https://www.lloydatkinson.net/posts/2022/writing-a-fuzzy-search-component-with-preact-and-fuse-for-astro/)
  - [How to Create an Astro Search component - Daniel Diaz](https://danidiaztech.com/create-astro-search-component/)

### If I want to handle form submissions?

- [astro-form-actions](https://github.com/pilcrowOnPaper/astro-form-actions) - SSR, utility for handling form submissions within Astro
- [@astro-reactive/form](https://www.npmjs.com/package/@astro-reactive/form) - Generate a dynamic form based on your data, and modify programmatically
  - [@astro-reactive/validator](https://www.npmjs.com/package/@astro-reactive/validator) - Easily set up validators for your forms
- [Web3Forms](https://web3forms.com/) - Receive form submissions directly in your email inbox without any server or back-end code
- [Netlify Forms](https://www.netlify.com/products/forms/) - Just add the `netlify` attribute to any form and everything gets wired up automatically

### If I want to add a RSS feed?

[What is RSS?](https://aboutfeeds.com/)

- [@astrojs/rss](https://docs.astro.build/en/guides/rss/#setting-up-astrojsrss) - Official integration for generating a RSS feed

### If I want to create a sitemap?

- [@astrojs/sitemap](https://docs.astro.build/en/guides/integrations-guide/sitemap/) - Automatically generates a sitemap based on your routes when you build your project
  - [Astro Sitemaps: Add Post and Page XML Sitemaps](https://dev.to/askrodney/astro-sitemaps-add-post-and-page-xml-sitemaps-1l8g)

### If I want to add a CMS?

[Connecting a CMS](https://docs.astro.build/en/guides/cms/)

- [@storyblok/astro](https://docs.astro.build/en/guides/cms/storyblok/) - Astro integration for [Storyblok](https://www.storyblok.com/)
  - [Announcing @storyblok/astro](https://www.storyblok.com/mp/announcing-storyblok-astro)
- [astro-sanity](https://github.com/littlesticks/astro-sanity) - Astro integration for [Sanity](https://www.sanity.io/)
  - [Integrate Astro and Sanity with our new Astro Integration! 🚀 - Little Sticks](https://www.youtube.com/watch?v=NM0FPzVdeUw)
  - [Playing around with Sanity.io ](https://dev.to/palmiak/playing-around-with-sanityio-3l5e)
- [astro-netlify-cms](https://github.com/delucis/astro-netlify-cms) - Astro integration for [Netlify CMS](https://www.netlifycms.org/)
- [Astro - Starter Ghost](https://github.com/PhilDL/astro-starter-ghost) - A starter template to build super fast websites with [Ghost](https://ghost.org/docs/) and Astro

### If I want to add E-Commerce?

- [astro-snipcart](https://github.com/lloydjatkinson/astro-snipcart) - Astro integration for [Snipcart](https://snipcart.com/)

### If I want to add internationalization?

- [astro-i18next](https://github.com/yassinedoghri/astro-i18next) - Astro integration for [i18next](https://github.com/i18next/i18next)
- [astro-i18n](https://github.com/alexandre-fernandez/astro-i18n) - A TypeScript-first internationalization library

### If I want to minify my website?

- [astro-compress](https://github.com/astro-community/astro-compress) - Compresses CSS, HTML, JSON, JavaScript, Images, and SVGs
- [astro-critters](https://github.com/astro-community/astro-critters) - Automatically inline the critical CSS
- [astro-html-minifier](https://github.com/sondr3/astro-html-minifier) - HTML minifier for Astro
- [astro-purgecss](https://github.com/codiume/orbit/tree/main/packages/astro-purgecss) - Integration for [purgecss](https://purgecss.com/) helps you remove unused CSS rules from your final astro bundle.
- [Jampack](https://jampack.divriots.com/) - SSG, post build tool for optimizing static websites
- [Netlify asset optimization](https://docs.netlify.com/configure-builds/file-based-configuration/#post-processing)
  - [Control your asset optimization settings from `netlify.toml`](https://www.netlify.com/blog/2019/08/05/control-your-asset-optimization-settings-from-netlify.toml/)

### If I want to add authentication?

- [astro-auth](https://github.com/nowaythatworked/auth-astro) - Astro integration for Auth.js
- [Lucia](https://lucia-auth.vercel.app/astro/start-here/getting-started) - Simple yet flexible user and session management library, provides an abstraction layer between your app and your database

### If I want to create a PWA?

- [@vite-pwa/astro](https://vite-pwa-org.netlify.app/frameworks/astro) - Astro integration for creating PWAs with [vite-pwa](https://vite-pwa-org.netlify.app/)
- [astro-webmanifest](https://github.com/alextim/astro-lib/tree/main/packages/astro-webmanifest) - Generates a web application manifest, favion, icons

### If I want to add SPA functionality?

[Blogs about SPAs in Astro](https://github.com/BryceRussell/my-awesome-astro/blob/main/BLOGS.md#spa)

- [@tanstack/router](https://tanstack.com/router/v1/docs/overview) - TanStack Router
  - [Are you an @astrodotbuild fan? Check out the latest @tan_stack Router beta working in Astro!](https://twitter.com/tannerlinsley/status/1623016669177315329?cxt=HHwWgoDQ7ffDjoYtAAAA)
- [@solidjs/router](https://github.com/solidjs/solid-router) - Router for SolidJS
  - [Did you know you can slap an SPA inside @astrodotbuild?? It's so easy! Let's see the `@solid_js router` in action, with SSR and route animations to boot 🙌](https://twitter.com/bholmesdev/status/1582726860646993920)
- [QGP](https://qgp.deno.dev/) - HMR for SPA routes/pages
- [astro-spa](https://github.com/RafidMuhymin/astro-spa) - Astro SPA is a SPA component/library that is built using Astro components. Includes support for animations, caching, containerization, local link detection, prefetching, progress bar, and more. 1.2kb(min+gzipped)

["Building SPA with Astro 1.0 Beta" Youtube series by Parasocial Fix](https://github.com/BryceRussell/my-awesome-astro/blob/main/YOUTUBE.md#building-spa-with-astro-10-beta-by-parasocial-fix)

### If I want to cache API requests?

- [@11ty/eleventy-fetch](https://github.com/11ty/eleventy-fetch) - Fetch network resources and cache them so you don’t bombard your API (or other resources)
