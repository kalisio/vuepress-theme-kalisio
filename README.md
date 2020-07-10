# vuepress-theme-kalisio

This is a simple [VuePress](https://vuepress.vuejs.org/) theme for Kalisio projects.

This theme extends the default VuePress theme in order to provides additional functionalities such as diagramming and mapping. Read this section to understand [theme inheritance](https://vuepress.vuejs.org/theme/inheritance.html#motivation).

## Using the components

### Diagramming

This theme provides an interface to add a [Mermaid](https://mermaid-js.github.io/mermaid/#/) diagram.
**Mermaid** components can be used like:

```md
<mermaid>
graph TD
  A[Cool] -->|Get money| B(Go shopping)
  B --> C{Let me}
  C -->|Two| D[Laptop]
  C -->|Two| E[iPhone]
  C -->|Three| F[Car]
  C -->|Four| F[Mac]
</mermaid>
```

### Mapping

This theme provides an interface to add a [kano](https://kalisio.github.io/kano/) **iframe**.
**Kano** components can be instantiated like:

```md
<kano token="A-JSON-WEB-TOKEN" />
```

The tag handles the following attributes:

| Attribute | Description |
| --- | --- |
| `source` | the url to the Kano website. The default value is `https://kano.dev.kalisio.xyz` |
| `token` | the token to be used if you want to be authenticated automatically. There is no default token and if you do not provide any token you have to authenticate yourself. |
| `css-style` | The style to apply to the **iframe**. The default value is `width: 100%; height: 50vh` |

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



