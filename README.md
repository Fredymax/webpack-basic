# Js-Porfolio

## Para minimizar CSS

Add feature [contenthash] for files.

> npm i css-minimizer-webpack-plugin terser-webpack-plugin --save-dev

```
module.exports = {
  ...
  optimization: {
    minimize: true,
    minimizer: [new CssMinimizerWebpackPlugin(), new TerserWebpackPlugin() ],
  }
}
```

## Working with environment variables

> npm i dotenv-webpack --save-dev

```
const Dotenv = require("dotenv-webpack");
module.exports = {
  ...
  module: {
    rules: [
      new Dotenv();
    ]
  }
}
```

## Working Live Server

> npm i webpack-dev-server -D

```
devServer: {
  static: path.join(__dirname, 'dist'),
  compress: true,
  historyApiFallback: true,
  port: 8080,
  open: true,
}
```
