# My Awesome Astro

## Official

### [Website](https://astro.build/)
#### [Discord](https://astro.build/chat)
#### [Documentation](https://docs.astro.build/en/getting-started/)
#### [Themes](https://astro.build/themes/)
#### [Integrations](https://astro.build/integrations/)
#### [Official Templates](https://astro.new/)
#### [Badges](https://astro.badg.es/)
### [Repository](https://github.com/withastro/astro)
#### [Docs Repository](https://github.com/withastro/docs)
#### [RFC Repository](https://github.com/withastro/rfcs)

## What Do I Use

### If I want to render a string of markdown?

[Fetching Remote Markdown](https://docs.astro.build/en/guides/markdown-content/#fetching-remote-markdown)

- [astro-remote](https://github.com/natemoo-re/astro-remote) - SSR/SSG, ability to use components in markdown
- [@astropub/md](https://github.com/astro-community/md) - SSG, markdown component and function
- [@astrojs/markdown-component](https://github.com/withastro/astro/tree/main/packages/markdown/component) - SSG, markdown component

### If I want to style my markdown?

- [Global Styling](https://docs.astro.build/en/guides/styling/#global-styles) - Use global vanilla css styling
- [Tailwind/typography plugin](https://tailwindcss.com/docs/typography-plugin) - Official tailwind plugin for styling markdown
- [Tailwind @apply directive](https://tailwindcss.com/docs/functions-and-directives#apply) - Create global tailwind styles using @apply directive
- [rehype-add-classes plugin](https://github.com/martypdx/rehype-add-classes) - Markdown plugin that lets you add classes(tailwind) to selectors

### If I want to create open graph images?

- [satori-html](https://github.com/natemoo-re/satori-html)
  - [Rumaan K - Dynamic OG images using Satori and Astro Server Endpoints](https://rumaan.dev/blog/open-graph-images-using-satori)
  - [Otterlord - Recreating Vercel's OG Image Generation](https://blog.otterlord.dev/post/dynamic-opengraph/)
- [@vercel/og](https://vercel.com/docs/concepts/functions/edge-functions/og-image-generation)
  - [Thomas Ledoux - Adding Vercel og:image generation to Astro project with Edge functions](https://dev.to/thomasledoux1/adding-vercel-ogimage-generation-to-astro-project-with-edge-functions-4mj2)
- [astro-og-image](https://www.npmjs.com/package/astro-og-image)

### If I want to search my website?

- [Pagefind](https://pagefind.app/)
- [Lunr](https://github.com/siverv/astro-lunr)
- [Lyra](https://github.com/LyraSearch/plugin-astro#readme)

### If I want to share state?

- [nanostores](https://github.com/nanostores/nanostores) - Currently reccomended by Astro, can be used between React, React Native, Preact, Vue, Svelte, and vanilla JavaScript
  - [@nanostores/persistent](https://github.com/nanostores/persistent) - Persist nanostores between pages using localStorage
- [Svelte stores](https://svelte.dev/docs#run-time-svelte-store) - Share state between Svelte components
- [SolidJS Signal](https://www.solidjs.com/docs/latest#createsignal) - SolidJS signals can be used in the frontmatter of `.astro` files
- [CustomEvent](https://developer.mozilla.org/en-US/docs/Web/Events/Creating_and_triggering_events) - Use vanilla JavaScript to send custom events

### If I want to add authentication?

- [Lucia](https://lucia-auth.vercel.app/astro/start-here/getting-started)
