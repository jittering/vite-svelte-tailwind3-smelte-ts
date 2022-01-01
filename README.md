# Svelte + TS + Vite + Smelte

This is template/bootstrap combining:

- Vite
- Svelte 3
- Tailwind CSS 3
- Smelte (via [fork](https://github.com/jittering/smelte/tree/peer) which corrects dependencies in package.json)
- TypeScript

Similar to the template at
[sveltekit-tailwind3-smelte](https://github.com/jittering/sveltekit-tailwind3-smelte)
which uses svelte-kit, this one builds on the `vite` template directly, without
svelte-kit.

While both use vite as the underlying dev server/bundler, svelte-kit has a very opinionated approach. This version uses a simple SPA approach with a single `index.html`.

## Quickstart

```sh
npm install
npm run dev
# or
npm run build
```

## Notes

The following are dependencies used by `smelte` which must be added to your project:

- tailwind-css-variables
- lodash
- rollup-plugin-postcss
- merge-deep
- svelte-waypoint
- svelte-typed-component
- tinycolor2

```sh
npm install --save-dev \
  tailwind-css-variables lodash rollup-plugin-postcss merge-deep svelte-waypoint \
  svelte-typed-component tinycolor2
```
