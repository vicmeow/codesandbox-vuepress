# Welcome

Welcome to the VuePress starter template for [CodeSandbox](https://codesandbox.io). To learn more about VuePress in general and how to customise this project, please see the [VuePress documentation](https://v1.vuepress.vuejs.org).

This template uses the default VuePress theme. To learn more about what you can do with it, please see the [Default Theme Config](https://v1.vuepress.vuejs.org/theme/default-theme-config.html#homepage) guide.

## Using a Custom Theme

When you want to create a custom VuePress theme, you add a `theme` directory under `.vuepress` (`.vuepress/theme`) and start by adding a `Layout.vue` file. From there it's the same as developing a normal Vue application. It is entirely up to you how to organize your theme.

The content of your `markdown` files to be rendered will be available as a special global component called `<Content/>`. You will need to add this somewhere in your layout in order to render and display the content of the page/markdown file. 

The simplest theme can be a single `Layout.vue` component with the following content:

```html
<template>
  <div class="theme-container">
    <Content/>
  </div>
</template>
```

If you want to customise the default VuePress theme, you can copy the default theme source code into `.vuepress/theme` using the `vuepress eject [targetDir]` command. Note, however, that once you eject, you are on your own and won't be receiving future updates or bug fixes to the default theme even if you upgrade your VuePress version.

For more information about how to get started with custom VuePress themes, please refer to the [Writing a theme](https://v1.vuepress.vuejs.org/theme/writing-a-theme.html) guide. If you would like to see how others have created custom themes, see the [VuePress Gallery](https://vuepress.gallery).

This template was created by [Victoria Bergquist](https://twitter.com/vicbergquist). If you would like to contribute to this template, please go to the [codesandbox-vuepress repository](https://github.com/vicbergquist/codesandbox-vuepress) on GitHub.