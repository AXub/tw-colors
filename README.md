# Welcome to [tw-colors](https://github.com/L-Blondy/tw-colors)

**tw-colors** is the most powerful and easy-to-use theming plugin for [tailwindcss](...)

*Inspired by [daisyui](https://daisyui.com/) 🔥*

## Highlights

-  🚀 Support for nested themes
-  📦 Zero import on the bundle size
-  🤩 Intuitive and easy to use API
-  ✨ Can handle any color format (HEX, rgb, hsl, color names...)
-  🎯 Supports opacity modifiers
-  💫 Full [Tailwind CSS Intellisense](https://marketplace.visualstudio.com/items?itemName=bradlc.vscode-tailwindcss) support

## The gist

1. Define your themes in `tailwind.config.js`

```js
const createThemes = require('tw-colors')

module.exports = {
   // ...your tailwind config
   plugins: [
      createThemes({
         light: {
            primary: 'teal',
            secondary: '#7c3aed',
            accent: 'hsl(50 13% 54%)',
            'base-100': '#f0f0f0'
            ...
         },
         dark: {
            primary: 'gold',
            secondary: '#7c3aed',
            accent: 'rgb(255,165,0)',
            'base-100': '#404040'
            ...
         },
         forest: {
            primary: 'green',
            secondary: '#adff2',
            accent: 'hsl(156 24% 84%)',
            'base-100': '#d05612'
            ...
         },
      ...
      }),
   ],
};

```

2. Add the class `theme-[name]` to an element, and use the colors <ins><b>as usual</b></ins> 🚀

```html
<section class="theme-light">
   <div class="bg-base-100">
      <h2 class="text-primary">
         ...
      </h2>

      <p class="text-secondary">
         ...
      </p>

      <button class="bg-primary text-white hover:bg-opacity-75">
         ...
      </button>
   </div>
</section>
```

3. switch the themes as you like... or even apply **nested themes** 🔥

## 📀 Install now!

```bash
npm i tw-colors
// or
yarn add tw-colors
```

## ✨ Demo

See the demo [here](...)

<div align="center">
Please share

[![][tweet]][tweet-url]

</div >

[tweet]: https://img.shields.io/twitter/url?style=social&url=https%3A%2F%2Fgithub.com%2Fsaadeghi%2Fdaisyui
[tweet-url]: https://twitter.com/intent/tweet?text=tw-colors%0ATailwind%20color%20themes%20made%20easy!%0AURL_TO_GITHUB