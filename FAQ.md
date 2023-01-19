# FAQ

## Questions

### Why is my `<style>` tag not applying styles?

`<style>` tags in Astro are [scoped by default](https://docs.astro.build/en/guides/styling/#scoped-styles) meaning styles will only be applied to HTML inside of the file. To opt out of scoping you can use [global styles](https://docs.astro.build/en/guides/styling/#global-styles)

### Why is the JavaScript for my component not working?

[UI Framework components](https://docs.astro.build/en/core-concepts/framework-components/) require a [client directive](https://docs.astro.build/en/reference/directives-reference/#client-directives) to control how the component is hydrated onto the page

### Why do I get an error when using an Astro component inside of a Svelte/Vue/React component?

Astro components cannot be used inside of [UI Framework components](https://docs.astro.build/en/core-concepts/framework-components/).

**Alternatives**:

- Use props to pass [Astro variables](https://docs.astro.build/en/reference/api-reference/#astro-global) like `Astro.url.pathname`
- [Use slots](https://docs.astro.build/en/core-concepts/astro-components/#slots) to pass Astro components to [UI Framework components](https://docs.astro.build/en/core-concepts/framework-components/)
- Turn your [UI Framework component](https://docs.astro.build/en/core-concepts/framework-components/) into a Astro component by wrapping with a `.astro` file

### Why can't I create a tailwind class dynamically?

[Dynamic Class Names](https://tailwindcss.com/docs/content-configuration#dynamic-class-names)

Tailwind classes must be statically analyzable, classes must exist inside the project files as a full unbroken string in order for tailwind to find the class and generate a style for it

### How do I avoid using relative imports ('../../Component.astro')?

You can use [import aliases](https://docs.astro.build/en/guides/typescript/#import-aliases) to avoid relative imports

### Why don't I have syntax highlighting in my MDX files?

To get syntax highlighting in MDX files you must install the [MDX VS Code plugin](https://marketplace.visualstudio.com/items?itemName=unifiedjs.vscode-mdx)
