# Vue Component

If one of your input files ends with `.vue`, Bili will automatically use [rollup-plugin-vue](https://rollup-plugin-vue.vuejs.org).

```bash
yarn add rollup-plugin-vue vue-template-compiler vue --dev

bili src/MyComponent.vue
```

Otherwise you need to add `rollup-plugin-vue` manually using the CLI flag `--plugin.vue` or config file:

```js
// bili.config.js
module.exports = {
  plugins: {
    vue: true,
    // or with custom options
    // vue: {}
  }
}
```
