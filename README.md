# typed-css-modules-loader

## This is a fork of https://github.com/olegstepura/typed-css-modules-loader

Simplest webpack loader for https://github.com/nanot1m/typed-css-modules

It has one option - noEmit, which turns off emitting files to the output path of webpack.

You can affect how `typed-css-modules` behaves by using query parameters. The loader
will pass any query parameters you specify (excluding noEmit) to the constructor of the `DtsCreator`
class. For more info on available options, please take a look here:
[DtsCreator constructor](https://github.com/nanot1m/typed-css-modules#new-dtscreatoroption).

```js
const settings = {
  // ...
  module: {
    rules: [
      // ...
      {
        test: /\.css$/,
        loaders: [
          "style-loader",
          "css-loader",
          "@skbkontur/typed-css-modules-loader"
        ]
      }
    ]
  }
  // ...
};
```
