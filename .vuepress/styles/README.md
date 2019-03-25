# Styles

**This directory is not required, you can delete it if you don't want to use it.**

This directory stores style related files.

## palette.styl

The [palette.styl](https://v1.vuepress.vuejs.org/config/#palette-styl) file is used to override the default theme color constants and to set the color constants of Stylus. If you wish, you can also apply simple color overrides to the styling of the default theme or define your own color variables for later use in the palette.styl file

### Note

You should ONLY write color variables in the palette.styl file. Because it (palette.styl) will be imported at the end of the root stylus config file, as a config, it will be used by multiple files, so if you include other styles here, they will be duplicated across files multiple times.

## index.styl

VuePress provides a convenient way to add extra styles to your app by creating an [index.styl](https://v1.vuepress.vuejs.org/config/#index-styl) file in this directory (.vuepress/styles). This is a Stylus file, but you can use normal CSS syntax in the file as well.