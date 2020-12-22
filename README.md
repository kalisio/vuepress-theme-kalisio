# vuepress-theme-kalisio

[![Latest Release](https://img.shields.io/github/v/tag/kalisio/vuepress-theme-kalisio?sort=semver&label=latest)](https://github.com/kalisio/vuepress-theme-kalisio/releases)

This is a simple [VuePress](https://vuepress.vuejs.org/) theme for [Kalisio](https://kalisio.com) projects.

This theme extends the default **VuePress** theme in order to provides additional functionalities such as diagramming and mapping. Read this section to understand [theme inheritance](https://vuepress.vuejs.org/theme/inheritance.html#motivation).

In addition, the theme includes the following plugins:
* [back-to-top](https://v1.vuepress.vuejs.org/plugin/official/plugin-back-to-top.html)
* [paw](https://v1.vuepress.vuejs.org/plugin/official/plugin-pwa.html)
* [kano](https://github.com/kalisio/vuepress-plugin-kano)
* [mermaid.js](https://github.com/eFrane/vuepress-plugin-mermaidjs)

## Installation

You can install it with

```bash
yarn add -D https://github.com/kalisio/vuepress-theme-kalisio#<version>
```

And then you just need to register the theme in your `.vuepress/config.js`:

```js
module.exports = {
    // ...
    theme: 'kalisio',
    // ...
}
```

## Usage

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

## Contributing

Found a bug ? Missing a Feature ? Want to contribute ? check out our [contribution guidelines](./CONTRIBUTING.md) for details

## Authors

This project is sponsored by 

[![Kalisio](https://s3.eu-central-1.amazonaws.com/kalisioscope/kalisio/kalisio-logo-black-256x84.png)](https://kalisio.com)

## License

This project is licensed under the MIT License - see the [license file](./LICENSE) for details


