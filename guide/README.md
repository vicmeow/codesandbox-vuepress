# Welcome

Welcome to the VuePress starter template for [CodeSandbox](https://codesandbox.io). This template uses the default VuePress theme. To find out what it offers, please see to the [Default Theme Config](https://v1.vuepress.vuejs.org/theme/default-theme-config.html#homepage) guide.

To learn more about VuePress and how to customise this project, please see the official [VuePress documentation](https://v1.vuepress.vuejs.org).

## Using a Custom Theme

When you want to create a custom theme, you create a `theme` directory under `.vuepress` (`.vuepress/theme`) and start by adding a `Layout.vue` file. From there it's the same as developing a normal Vue application. It is entirely up to you how to organize your theme.

The content of your `markdown` files that will be rendered will be available as a special `<Content/>` global component. You will need to render it somewhere in your layout in order to display the content of the page. 

The simplest theme can be a single `Layout.vue` component with the following content:

```html
<template>
  <div class="theme-container">
    <Content/>
  </div>
</template>
```

If you want to customise the default VuePress theme, you can copy the default theme source code into `.vuepress/theme` using the `vuepress eject [targetDir]` command. Note, however, once you eject, you are on your own and won't be receiving future updates or bug fixes to the default theme even if you upgrade VuePress.

To get started with custom themes, please refer to the [Writing a theme](https://v1.vuepress.vuejs.org/theme/writing-a-theme.html) guide. If you would like to see how others have created custom themes, see the [VuePress Gallery](https://vuepress.gallery).