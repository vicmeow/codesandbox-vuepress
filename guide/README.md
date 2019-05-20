---
sidebar: auto
pageClass: custom-page-class
---

# Guide

Welcome to the VuePress starter template for [CodeSandbox](https://codesandbox.io). To learn more about VuePress in general and how to customize this project, please see the [VuePress documentation](https://v1.vuepress.vuejs.org).

## Theme Customization

This template uses the default VuePress theme. To learn more about what you can do with it, please see the [Default Theme Config](https://v1.vuepress.vuejs.org/theme/default-theme-config.html#homepage) guide.

If you want to customize the default VuePress theme, you can do this in a few ways, but to various extents.

### Color Overrides

If you would like to keep the default theme and only change the colors, you can change a few variables by creating a `palette.style` file in a `styles` directory under `.vuepress`. Here you have the option to pick a new accent, text, border and code block background color.

```stylus
// showing default values
$accentColor = #3eaf7c
$textColor = #2c3e50
$borderColor = #eaecef
$codeBgColor = #282c34
```

### Style Overrides

You can also add your own styles or override general styles by creating a `index.styl` file in the same `/styles` directory as the `palette.styl` file mentioned above. This is a Stylus file, but you can write normal CSS syntax as well.

```css
.sidebar {
  background: pink;
}
```

### Custom Page Classes

VuePress also lets you specify custom classes for your pages in YAML front matter. This can be useful when you want to target specific content on a page. Use `pageClass` to add a class to the theme container div tag:

```yaml
---
pageClass: custom-page-class
---
```

Then you can write CSS to target that specific page in `.vuepress/styles/index.styl`:

```css
.theme-container.custom-page-class .language-example {
  border: 4px solid #3eaf7c;
}
```

As an example, we have added a `pageClass` of `custom-page-class` to this page and targeted this code block that has a language of `example` with the styles from above:

```example
A code block with a custom language targeted with a custom page class.
```

### Ejecting

If you would like to customize the default theme even more and have full control over how the different components look like, you can eject the default theme.

::: warning
When ejecting you are on your own and **will not** be receiving future updates or bug fixes to the default theme even if you upgrade your VuePress version.
:::

To get started, copy the default theme source code into `.vuepress/theme` using the `vuepress eject [targetDir]` command.

## Custom Layouts

VuePress also lets you specify custom layout components for specific pages, instead of the default page layout component provided by the default theme.

To do this, you add YAML front matter to your markdown file and specify the layout component you want to use.

 ```yaml
 ---
 layout: SpecialLayout
 ---
 ```

Visit our [Special Layout Page](/special-layout) to see an example of a custom page layout in action. This component is located in the `.vuepress/components` directory, which is where you register custom layout components and other components you want to have global access to.

## Custom Themes

When you want to create a custom VuePress theme, you add a `theme` directory under `.vuepress` (`.vuepress/theme`) and start by adding a `Layout.vue` file. From there it's the same as developing a normal Vue application. It is entirely up to you how you organize your theme.

The content of your `markdown` files to be rendered will be available as a special global component called `<Content/>`. You will need to add this somewhere in your layout in order to render and display the content of the page/markdown file. 

The simplest theme can be a single `Layout.vue` component with the following content:

```html
<template>
  <div class="theme-container">
    <Content/>
  </div>
</template>
```

For more information about how to get started with custom VuePress themes, please refer to the [Writing a theme](https://v1.vuepress.vuejs.org/theme/writing-a-theme.html) guide. If you would like to see how others have created custom themes, see the [VuePress Gallery](https://vuepress.gallery).

## Credits

This codesandbox template was created by [Victoria Bergquist](https://twitter.com/vicbergquist). The information on this page is gathered from the official [VuePress documentation](https://v1.vuepress.vuejs.org) for the latest version of VuePress.

If you would like to contribute to this template, please go to the [codesandbox-vuepress repository](https://github.com/vicbergquist/codesandbox-vuepress) on GitHub.
