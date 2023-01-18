## Official

### [Website](https://astro.build/)
#### [Discord](https://astro.build/chat)
#### [Documentation](https://docs.astro.build/en/getting-started/)
#### [Themes](https://astro.build/themes/)
#### [Integrations](https://astro.build/integrations/)
#### [Official Templates](https://astro.new/)
#### [Badges](https://astro.badg.es/)
### [Repository](https://github.com/withastro/astro)
#### [Changelog](https://github.com/withastro/astro/blob/main/packages/astro/CHANGELOG.md)
#### [Docs Repository](https://github.com/withastro/docs)
#### [RFC Repository](https://github.com/withastro/rfcs)

## What Do I Use

### If I want to add a font?

[Using Custom Fonts](https://docs.astro.build/en/guides/fonts/)

- [Fontsource](https://docs.astro.build/en/guides/fonts/#using-fontsource) - Self-host Open Source fonts in neatly bundled NPM packages, faster than Google Fonts
  - [Fontsource’s catalog](https://fontsource.org/fonts) - Catalog of all fonts supported by Fontsource
- [astro-google-fonts-optimizer](https://github.com/sebholstein/astro-google-fonts-optimizer) - Component, downloads the CSS of a Google Fonts stylesheet and inlines it directly into the page, inspired by [NextJS font optimization](https://nextjs.org/blog/next-10-2#automatic-webfont-optimization)
- [astro-fonts-next](https://github.com/dc7290/astro-fonts-next) - Integration, applies [NextJS font optimization](https://nextjs.org/blog/next-10-2#automatic-webfont-optimization) to Google Fonts

### If I want add icons?

- [astro-icon](https://github.com/natemoo-re/astro-icon) - (Un)Official `<Icon>` component powered by [Iconify](https://iconify.design/)
  - [Icon set refrence](https://icon-sets.iconify.design/) - List of available icons
  - [Icônes](https://icones.js.org/) - Tool for exploring and downloading icons
  - [Iconify Components](https://docs.iconify.design/develop/) - Official [Iconify](https://iconify.design/) components
- [astro-feather-icons](https://github.com/edazpotato/astro-feather-icons) - Icon component for [Feather icons](https://feathericons.com/)
- [astro-heroicons](https://github.com/seanmcp/astro-heroicons) - Icon component for [Heroicons](https://heroicons.com/)
- [@astropub/icons](https://github.com/astro-community/icons) - Icon component for [Radix icons](https://icons.radix-ui.com/)
- [phosphor-astro](https://github.com/seanmcp/phosphor-astro) - Icon component for [Phosphor icons](https://phosphoricons.com/)
- [astro-svg-loaders](https://github.com/codiume/orbit/tree/main/packages/astro-svg-loaders) - Component for [svg loading icons by @SamHerbert](https://github.com/SamHerbert/SVG-Loaders)

### If I want to add SEO?

- [astro-seo](https://github.com/jonasmerlin/astro-seo) - (Recommended) Most popular `<SEO>` component
- [@astrolib/seo](https://github.com/onwidget/astrolib/tree/main/packages/seo) - Based on [NextSEO](https://github.com/garmeeh/next-seo)
- [astro-seo-metadata](https://github.com/JulianCataldo/web-garden/tree/develop/app/SEOMetadata) - Minimal SEO component 
- [astro-seo-meta](https://github.com/codiume/orbit/tree/main/packages/astro-seo-meta) - Minimal SEO component

### If I want to add optimized images?

- [@astrojs/image](https://docs.astro.build/en/guides/integrations-guide/image/) - Official image optimization integration
- [astro-imagetools](https://github.com/RafidMuhymin/astro-imagetools) - Community image optimization integration
- [astro-eleventy-img](https://github.com/Princesseuh/astro-eleventy-img) - Generate images using [eleventy-img](https://github.com/11ty/eleventy-img)

### If I want to render a string of markdown?

[Fetching Remote Markdown](https://docs.astro.build/en/guides/markdown-content/#fetching-remote-markdown)

- [astro-remote](https://github.com/natemoo-re/astro-remote) - SSR/SSG, ability to use components in markdown
- [@astrojs/markdown-remark](https://github.com/withastro/astro/blob/52209ca2ad72a30854947dcb3a90ab4db0ac0a6f/packages/markdown/remark/src/index.ts#L42) - SSG, built in `renderMarkdown()` utility for rendering markdown
- [@astropub/md](https://github.com/astro-community/md) - SSG, `<Markdown>` component and function
- [@astrojs/markdown-component](https://github.com/withastro/astro/tree/main/packages/markdown/component) - SSG, `<Markdown>` component

### If I want to style my markdown?

- [Global Styling](https://docs.astro.build/en/guides/styling/#global-styles) - Use global vanilla css styling
- [@tailwindcss/typography](https://tailwindcss.com/docs/typography-plugin) - Official tailwind plugin for styling markdown
- [Tailwind @apply directive](https://tailwindcss.com/docs/functions-and-directives#apply) - Create global tailwind styles using @apply directive
- [rehype-add-classes](https://github.com/martypdx/rehype-add-classes) - Markdown plugin that lets you add classes(tailwind) to selectors


### If I want to share state between components?

[Sharing State](https://docs.astro.build/en/core-concepts/sharing-state/)

- [nanostores](https://github.com/nanostores/nanostores) - Currently reccomended by Astro, can be used between React, React Native, Preact, Vue, Svelte, and vanilla JavaScript
  - [@nanostores/persistent](https://github.com/nanostores/persistent) - Persist nanostores between pages using localStorage
- [Svelte stores](https://svelte.dev/docs#run-time-svelte-store) - Share state between Svelte components
- [SolidJS signal](https://www.solidjs.com/docs/latest#createsignal) - SolidJS signals can be used in the frontmatter of `.astro` files
- [Custom Event](https://developer.mozilla.org/en-US/docs/Web/Events/Creating_and_triggering_events) - Use vanilla JavaScript to send custom events

### If I want to create open graph images?

[Open Graph Protocol](https://ogp.me/)

- [satori-html](https://github.com/natemoo-re/satori-html) - Create og images using html strings and [satori](https://github.com/vercel/satori)
  - [Dynamic OG images using Satori and Astro Server Endpoints - Rumaan K](https://rumaan.dev/blog/open-graph-images-using-satori)
  - [Recreating Vercel's OG Image Generation - Otterlord](https://blog.otterlord.dev/post/dynamic-opengraph/)
- [@vercel/og](https://vercel.com/docs/concepts/functions/edge-functions/og-image-generation) - Vercel's official open graph image generation using [satori](https://github.com/vercel/satori)
  - [Adding Vercel og:image generation to Astro project with Edge functions - Thomas Ledoux](https://dev.to/thomasledoux1/adding-vercel-ogimage-generation-to-astro-project-with-edge-functions-4mj2)
- [astro-og-image](https://www.npmjs.com/package/astro-og-image) - Screenshot pages as open graph images

[Preview open graph images and meta tags of website](https://www.opengraph.xyz/)

### If I want to add the ability to search?

- [Pagefind](https://pagefind.app/)
  - [Add Searching To Your Astro Static Site - Otterlord](https://blog.otterlord.dev/post/astro-search/)
  - [Pagefind is quite a find for site search - Bryce Wray](https://www.brycewray.com/posts/2022/07/pagefind-quite-find-site-search/)
  - [Sweeter searches with Pagefind - Bryce Wray](https://www.brycewray.com/posts/2022/12/sweeter-searches-pagefind/)
- [@lyrasearch/plugin-astro](https://github.com/LyraSearch/plugin-astro) - Astro integration for [Lyra](https://lyrajs.io/) search
- [astro-lunr](https://github.com/jackcarey/astro-lunr) - Astro integration for [Lunr](https://github.com/siverv/astro-lunr) search

### If I want to add internationalization?

- [astro-i18next](https://github.com/yassinedoghri/astro-i18next) - Astro integration for [i18next](https://github.com/i18next/i18next)
- [astro-i18n](https://github.com/alexandre-fernandez/astro-i18n) - A TypeScript-first internationalization library

### If I want to add a CMS?

[Connecting a CMS](https://docs.astro.build/en/guides/cms/)

- [@storyblok/astro](https://docs.astro.build/en/guides/cms/storyblok/) - Astro integration for [Storyblok](https://www.storyblok.com/)
- [astro-sanity](https://github.com/littlesticks/astro-sanity) - Astro integration for [Sanity](https://www.sanity.io/)
- [astro-netlify-cms](https://github.com/delucis/astro-netlify-cms) - Astro integration for [Netlify CMS](https://www.netlifycms.org/)

### If I want to create a sitemap?

- [@astrojs/sitemap](https://docs.astro.build/en/guides/integrations-guide/sitemap/) - Automatically generates a sitemap based on your routes when you build your project

### If I want to create a PWA?

- [@vite-pwa/astro](https://vite-pwa-org.netlify.app/frameworks/astro) - Astro integration for creating PWAs with [vite-pwa](https://vite-pwa-org.netlify.app/)
- [astro-webmanifest](https://github.com/alextim/astro-lib/tree/main/packages/astro-webmanifest) - Generates a web application manifest, favion, icons

### If I want to minify my website?

- [astro-compress](https://github.com/astro-community/astro-compress) - Compresses CSS, HTML, JSON, JavaScript, Images, and SVGs
- [astro-critters](https://github.com/astro-community/astro-critters) - Automatically inline the critical CSS
- [Netlify asset optimization](https://docs.netlify.com/configure-builds/file-based-configuration/#post-processing)
  - [Control your asset optimization settings from `netlify.toml`](https://www.netlify.com/blog/2019/08/05/control-your-asset-optimization-settings-from-netlify.toml/)

### If I want to add authentication?

- [Lucia](https://lucia-auth.vercel.app/astro/start-here/getting-started)
