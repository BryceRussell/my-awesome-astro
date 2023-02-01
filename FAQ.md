# FAQ

## What is this?

I take notes here on commonly asked questions in Astro's `#support` channel on [Discord](https://astro.build/chat). Most of this information can be found in [the Astro docs](https://docs.astro.build) or on the [Discord](https://astro.build/chat), check there first. If you need help you can post a question to the `#support` channel in the [Discord](https://astro.build/chat)

### [Documentation](https://docs.astro.build)

### [Troubleshooting](https://docs.astro.build/en/guides/troubleshooting/)

## Table of Contents

- [Why do Astro commands like `astro dev` not work?](https://github.com/BryceRussell/my-awesome-astro/tree/main/FAQ.md#why-do-astro-commands-like-astro-dev-not-work)
- [Why is `astro-icon` not working?](https://github.com/BryceRussell/my-awesome-astro/blob/main/FAQ.md#why-is-astro-icon-not-working)
- [Why is my `<style>` tag not applying styles?](https://github.com/BryceRussell/my-awesome-astro/blob/main/FAQ.md#why-is-my-style-tag-not-applying-styles)
- [Why are my CSS styles duplicated?](https://github.com/BryceRussell/my-awesome-astro/blob/main/FAQ.md#why-are-my-css-styles-duplicated)
- [Why is my image import returning `[object Object]`?](https://github.com/BryceRussell/my-awesome-astro/blob/main/FAQ.md#why-is-my-image-import-returning-object-object)
- [Why is my image blurry when using `@astojs/image`?](https://github.com/BryceRussell/my-awesome-astro/blob/main/FAQ.md#why-is-my-image-blurry-when-using-astojsimage)
- [Why is my `<script>` tag not working?](https://github.com/BryceRussell/my-awesome-astro/blob/main/FAQ.md#why-is-my-script-tag-not-working)
- [How do I use frontmatter variables in my `<script>` tag?](https://github.com/BryceRussell/my-awesome-astro/blob/main/FAQ.md#how-do-i-use-frontmatter-variables-in-my-script-tag)
- [How do I do conditional rendering?](https://github.com/BryceRussell/my-awesome-astro/blob/main/FAQ.md#how-do-i-conditionally-render-something)
- [Why is my `.map()` not rendering anything?](https://github.com/BryceRussell/my-awesome-astro/blob/main/FAQ.md#why-is-my-map-not-rendering-anything)
- [How do I loop X number of time using JSX?](https://github.com/BryceRussell/my-awesome-astro/blob/main/FAQ.md#how-do-i-loop-x-number-of-time-using-jsx)
- [Why is my component's JavaScript not working?](https://github.com/BryceRussell/my-awesome-astro/blob/main/FAQ.md#why-is-my-components-javascript-not-working)
- [Why do I get an error when using an Astro component inside of a Svelte/Vue/React component?](https://github.com/BryceRussell/my-awesome-astro/blob/main/FAQ.md#why-do-i-get-an-error-when-using-an-astro-component-inside-of-a-sveltevuereact-component)
- [How do I use env variables?](https://github.com/BryceRussell/my-awesome-astro/blob/main/FAQ.md#how-do-i-use-env-variables)
- [How do I use an imported asset in CSS?](https://github.com/BryceRussell/my-awesome-astro/blob/main/FAQ.md#how-do-i-use-an-imported-asset-in-css)
- [How do I pass variables to JSON inside of a `<script>`?](https://github.com/BryceRussell/my-awesome-astro/blob/main/FAQ.md#how-do-i-pass-variables-to-json-inside-of-a-script)
- [Why can't I create a tailwind class dynamically?](https://github.com/BryceRussell/my-awesome-astro/blob/main/FAQ.md#why-cant-i-create-a-tailwind-class-dynamically)
- [How do I avoid using relative imports ('../../Component.astro')?](https://github.com/BryceRussell/my-awesome-astro/blob/main/FAQ.md#how-do-i-avoid-using-relative-imports-componentastro)
- [Why don't I have syntax highlighting in my MDX files?](https://github.com/BryceRussell/my-awesome-astro/blob/main/FAQ.md#why-dont-i-have-syntax-highlighting-in-my-mdx-files)
- [How do I customize the file/folder names of my output?](https://github.com/BryceRussell/my-awesome-astro/blob/main/FAQ.md#how-do-i-customize-the-filefolder-names-of-my-output)

## Questions

### Why do Astro commands like `astro dev` not work?

If your project was just cloned make sure to use `npm i` to install node dependencies

Another issue could be your version of Node, Astro 2.0 is compatible with `v16.12` - `v18`,  while Astro 1.0 is only compatible up to `v17`

### Why is `astro-icon` not working?

There could be a few issues:

- Icons have no size by default, add a `size={number}` prop or [use CSS to size icon](https://github.com/natemoo-re/astro-icon#styling)
- Some packs and icons don't work and throw a `Error: Not Found` warning, you can try [finding an alternative](https://icon-sets.iconify.design/)
- Your using an Astro component (server side) in a 
[UI Framework component](https://docs.astro.build/en/core-concepts/framework-components/) (client side), instead pass the icon using slots

### Why is my `<style>` tag not applying styles?

`<style>` tags in Astro are [scoped by default](https://docs.astro.build/en/guides/styling/#scoped-styles), this means the styles will only be applied to HTML inside of the file. To opt out of scoping you can use [global styles](https://docs.astro.build/en/guides/styling/#global-styles)

### Why are my CSS styles duplicated?

CSS Styles are only sometimes duplicated when using the develpment server. If you use `npm run build` and `npm run preview` to build and preview the website then the styles should not be duplicated

### Why is my image import returning `[object Object]`?

You most likely have the `@astrojs/image` integration installed which changes the way images are imported

If you want to use an imported image with a normal `<img>` element while this integration is installed you must add `?url` to the end of your import path

```jsx
---
// add '?url' when using <img> with @astrojs/image installed
import levi from '../levi.png?url';
---

<img src={levi} alt="My orange cat"/>
```

### Why is my image blurry when using `@astojs/image`?

The `height` and `width` props of your image must be 1.5x - 2x larger than the CSS size of the image

[Reponsive Image Rabbit Hole – Part 3 - Scott Willsey](https://scottwillsey.com/image-rabbit-hole-3/)

### Why is my `<script>` tag not working?

`<script>` tags are [hoisted as modules by default](https://docs.astro.build/en/guides/client-side-scripts/#script-bundling), if your `<script>` tag is not working it most likely needs an [`is:inline` directive](https://docs.astro.build/en/reference/directives-reference/#isinline) to opt out of hoisting

### How do I use frontmatter variables in my `<script>` tag?

You can use the [`define:vars` directive](https://docs.astro.build/en/reference/directives-reference/#definevars) to pass frontmatter variables to a `<script>` tag. Using this directive also applies the [`is:inline` directive](https://docs.astro.build/en/reference/directives-reference/#isinline)

If you want to [avoid `define:vars`](https://docs.astro.build/en/guides/client-side-scripts/#pass-frontmatter-variables-to-scripts) another option is using [`data-*` attributes](https://developer.mozilla.org/en-US/docs/Learn/HTML/Howto/Use_data_attributes) 

### How do I do conditional rendering?

```jsx
{ boolean && 
  <span>True</span>
}
```

```jsx
{ boolean
  ? <span>True</span>
  : <span>False</span>
}
```

### Why is my `.map()` not rendering anything?

If your `.map()` is not rendering anything make sure that it is formatted correctly

```jsx
{ array.map((i) => <span>{i}</span>) }

{ array.map((i) => (
  <span></span>
))}

{ array.map((i) => <>
  <span></span>
</>)}

// '{}' requires 'return'

{ array.map((i) => {
  return <span></span>
})}

{ array.map((i) => {
  return (
    <span></span>
  )
})}

{ array.map((i) => {
  return <>
    <span></span>
  </>
})}

// Nested Map
{ array.map((i) => <>
  { array.map((i) => <>
    <span></span>
  </>)}
</>)}
```

### How do I loop X number of time using JSX?

```jsx
// Loops 3 times, returns index as argument
[...Array(3).keys()].map(index => {
  return <li>{i}</li>
})
```
```html
<li>0</li>
<li>1</li>
<li>2</li>
```

### Why is my component's JavaScript not working?

[UI Framework components](https://docs.astro.build/en/core-concepts/framework-components/) require a [client directive](https://docs.astro.build/en/reference/directives-reference/#client-directives) to control how the component is hydrated onto the page

### Why do I get an error when using an Astro component inside of a Svelte/Vue/React component?

Astro components cannot be used inside of [UI Framework components](https://docs.astro.build/en/core-concepts/framework-components/).

**Alternatives**:

- Use props to pass [Astro variables](https://docs.astro.build/en/reference/api-reference/#astro-global) like `Astro.url.pathname`
- [Use slots](https://docs.astro.build/en/core-concepts/astro-components/#slots) to pass Astro components to [UI Framework components](https://docs.astro.build/en/core-concepts/framework-components/)
- Wrap your [UI Framework component](https://docs.astro.build/en/core-concepts/framework-components/) with a `.astro` file

### How do I use env variables?

[Using Enviroment Variables](https://docs.astro.build/en/guides/environment-variables/#getting-environment-variables)

You can use `import.meta.env` to access enviroment variables inside of `.env`

`.env` variables can only be accessed server side by default if you want to expose a `.env` variable 1client side the variable must be prefixed with `PUBLIC_`, DO NOT do this with secrets like API keys

If your `.env` variable can't be exposed publicly but you need it for data client side you can try creating an [API endpoint](https://docs.astro.build/en/core-concepts/endpoints) that uses the secret env variable to return JSON

### How do I use an imported asset in CSS?

- [define:vars](https://docs.astro.build/en/reference/directives-reference/#definevars)
- [set:html](https://docs.astro.build/en/reference/directives-reference/#sethtml)

```jsx
---
import bg from '../images/bg.png'
---
// Using 'define:vars'
<style define:vars={{
  bg: `url("${bg}")` 
}}>
  // creates variable '--bg: url("...");'
</style>

// Using 'style' attribute
<div style={`background-image:url("${bg}");`}></div>
<div style={`--bg:url("${bg}");`}></div>

// Using 'set:html'
<style set:html={`
  body {
    background-image: url("${bg}");
  }
`}/>
```

### How do I pass variables to JSON inside of a `<script>`?

Using [set:html](https://docs.astro.build/en/reference/directives-reference/#sethtml) with a [template string](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Template_literals)

```jsx
<script set:html={`
  {
    "key": "${value}"
  }
`}/>
```

### Why can't I create a tailwind class dynamically?

[Dynamic Class Names](https://tailwindcss.com/docs/content-configuration#dynamic-class-names)

Tailwind classes must be statically analyzable, this means classes must exist inside the project files as a full unbroken string in order for tailwind to find the class and generate a style for it

### How do I avoid using relative imports ('../../Component.astro')?

You can use [import aliases](https://docs.astro.build/en/guides/typescript/#import-aliases) to avoid relative imports

### Why don't I have syntax highlighting in my MDX files?

To get syntax highlighting in MDX files you must install the [MDX VS Code plugin](https://marketplace.visualstudio.com/items?itemName=unifiedjs.vscode-mdx)

### How do I customize the file/folder names of my output?

[Build Options](https://docs.astro.build/en/reference/configuration-reference/#build-options)

[Customising Output Filenames](https://docs.astro.build/en/guides/configuring-astro/#customising-output-filenames)

<div align="right">
    <b><a href="#table-of-contents">↥ Back To Top</a></b>
</div>
