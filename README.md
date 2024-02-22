<div align="center">
  <img src="https://grow.empress.eco/uploads/default/original/2X/1/1f1e1044d3864269d2a613577edb9763890422ab.png" alt="Logo" width="80" height="80">
  <h3 align="center">Streamline Your CSS Preprocessing with esbuild-plugin-postcss2</h3>
  <p align="center">
    An optimized and type-friendly plugin for efficient CSS preprocessing and CSS modules.
    <br />
    <a href="https://grow.empress.eco/"><strong>Explore the Docs »</strong></a>
    <br />
    <br />
    <a href="https://github.com/empress-eco/esbuild-plugin-postcss2/issues">Report Bug</a>
    ·
    <a href="https://github.com/empress-eco/esbuild-plugin-postcss2/issues">Request Feature</a>
  </p>
</div>

## About The Project

`esbuild-plugin-postcss2` is a powerful, type-friendly plugin designed to simplify your CSS preprocessing and CSS modules. It provides developers with an efficient way to integrate CSS preprocessing into their projects with ease.

### Key Features
- Full support for CSS preprocessors and CSS modules.
- Seamless integration with esbuild plugins.
- Customizable modules and preprocessors.

## Technical Stack and Setup Instructions

This project uses:
- JavaScript
- Node.js
- esbuild
- postcss

### Installation

Start by cloning the repository:

```sh
git clone https://github.com/empress-eco/esbuild-plugin-postcss2.git
```

After that, you can install the plugin using Yarn or npm:

**Yarn:**
```sh
yarn add -D esbuild-plugin-postcss2
```

**npm:**
```sh
npm i -D esbuild-plugin-postcss2
```

## Usage

Integrate the plugin to your esbuild plugins:

```js
const esbuild = require("esbuild");
const postCssPlugin = require("esbuild-plugin-postcss2");

esbuild.build({
  ...
  plugins: [
    postCssPlugin.default()
  ]
  ...
});
```

You can extend the functionality of this plugin by adding any PostCSS plugin to the plugins array as per your requirements. For example, to add the autoprefixer plugin, use the following code:

```js
const autoprefixer = require("autoprefixer");

esbuild.build({
  ...
  plugins: [
    postCssPlugin.default({
      plugins: [autoprefixer]
    })
  ]
  ...
});
```

PostCSS modules are enabled by default. You can pass in a config or disable it with the `modules` field. For more information and examples, consult the [official documentation](https://grow.empress.eco/).

## Contribution Guidelines

We welcome contributions from the community! Follow these steps to contribute:

- Fork the Project
- Create your feature branch (`git checkout -b feature/AmazingFeature`)
- Commit your changes (`git commit -m 'Add some AmazingFeature'`)
- Push to the branch (`git push origin feature/AmazingFeature`)
- Open a Pull Request

## License and Acknowledgements

### License

This project is under the MIT License. Your contributions are also licensed under the MIT License.

### Acknowledgments

We extend our heartfelt gratitude to the Empress Community, whose innovative tools form the backbone of this project. Their commitment to innovation has been instrumental in building the features and functionalities we rely on. We are profoundly thankful for their pioneering work and ongoing support.