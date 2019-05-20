---
layout: SpecialLayout
---

# Example

This is markdown content rendered inside a special layout component. We have specified a layout component in yaml front matter that VuePress will use for this specific page. This layout component can be found here: `.vuepress/components/SpecialLayout.vue`.

```yaml
---
layout: SpecialLayout
---
```

Notice how only the layout has changed, not the general styles. This is because we are still using the default theme, but with a custom layout instead of the default one.

To learn more, please read the official documentation on [custom page layouts](https://v1.vuepress.vuejs.org/theme/default-theme-config.html#custom-layout-for-specific-pages).