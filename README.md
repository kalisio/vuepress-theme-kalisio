# vuepress-theme-kalisio

This is a simple [VuePress](https://vuepress.vuejs.org/) theme for Kalisio projects.

This theme extends the default **VuePress** theme in order to provides additional functionalities such as diagramming and mapping. Read this section to understand [theme inheritance](https://vuepress.vuejs.org/theme/inheritance.html#motivation).

In addition, the theme includes the following plugins:
* [back-to-top](https://v1.vuepress.vuejs.org/plugin/official/plugin-back-to-top.html)
* [paw](https://v1.vuepress.vuejs.org/plugin/official/plugin-pwa.html)
* [kano](https://github.com/kalisio/vuepress-plugin-kano)
* [mermaid.js](https://github.com/eFrane/vuepress-plugin-mermaidjs)

## Using the components

### Template URL

_TO DO_

## Configuring the theme

### Overriding the **Banner**

The **Banner** component provides two props, `image`, `slogan` and `link`, that allows you to override the default values which are respectively our logo, our slogan and the url to our website.

In your `config.js` file, add the following object in the `themeConfig` object:

```js
banner: {
  image: 'path to your image',
  slogan: 'your slogan',
  link: 'your url'  // you can also use '#' to provide a null link
}
```

### Overriding the palette

Please, report to [this section](https://vuepress.vuejs.org/config/#palette-styl).



