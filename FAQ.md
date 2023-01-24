# FAQ

## Questions

### Why do Astro commands like `astro dev` not work?

If your project was just cloned make sure to use `npm i` to install node dependencies

Another issue could be your version of Node, Astro 2.0 is compatible with `v16.12` - `v18`,  while Astro 1.0 is only compatible up to `v17`

### Why is my `<style>` tag not applying styles?

`<style>` tags in Astro are [scoped by default](https://docs.astro.build/en/guides/styling/#scoped-styles), this means the styles will only be applied to HTML inside of the file. To opt out of scoping you can use [global styles](https://docs.astro.build/en/guides/styling/#global-styles)

### Why do I have duplicated CSS styles?

Styles are only duplicated when using the dev server, if you build and preview the website using `npm run build` and `npm run preview` then the styles will not be duplicated

### Why is my `<script>` tag not working?

`<script>` tags are [hoisted as modules by default](https://docs.astro.build/en/guides/client-side-scripts/#script-bundling), if your `<script>` tag is not working it most likely needs an [`is:inline` directive](https://docs.astro.build/en/reference/directives-reference/#isinline) to opt out of hoisting

### How do I use frontmatter variables in my `<script>` tag?

You can use the [`define:vars` directive](https://docs.astro.build/en/reference/directives-reference/#definevars) to pass frontmatter variables to a `<script>` tag. Using this directive also applies the [`is:inline` directive](https://docs.astro.build/en/reference/directives-reference/#isinline)

If you want to [avoid `define:vars`](https://docs.astro.build/en/guides/client-side-scripts/#pass-frontmatter-variables-to-scripts) another option is using [`data-*` attributes](https://developer.mozilla.org/en-US/docs/Learn/HTML/Howto/Use_data_attributes) 

### How do I conditionally render something?

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
```

### How do I loop X number of time using JSX?

```jsx
// Loops 10 times, returns index as argument
[...Array(10).keys()].map(index => {
  return <li>{i + 1}</li>
})
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
