# vite react ssr critical css issue

Dev mode in a react server-rendered application the initial critical css is not inlined into the html.
Styles kicks in only after the react hydration and the vite runtime loaded.

This results in a very bad flickering, especially in big applications since it takes few seconds before the vite fetches all the required js and is browser ready.

## command

```sh
yarn dev
```

### issue

https://github.com/vitejs/vite/issues/16515
