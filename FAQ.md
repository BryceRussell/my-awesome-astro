# FAQ

## Questions

### Why can't I create a tailwind class dynamically?

Tailwind classes must be statically analyzable meaning classes must exist inside the project files as a full unbroken string in order for tailwind to find the class and generate a style for it, [more information](https://tailwindcss.com/docs/content-configuration#dynamic-class-names)

### How do I avoid using relative imports ('../../')?

To avoid relative imports use [import aliases](https://docs.astro.build/en/guides/typescript/#import-aliases)

### Why don't I have syntax highlighting in my MDX files?

To get syntax highlighting in MDX files you must install the [MDX VS Code plugin](https://marketplace.visualstudio.com/items?itemName=unifiedjs.vscode-mdx)
