[![npm][npm]][npm-url]
[![node][node]][node-url]
[![deps][deps]][deps-url]
[![tests][tests]][tests-url]
[![coverage][cover]][cover-url]
[![chat][chat]][chat-url]

<div align="center">
  <a href="https://github.com/webpack/webpack">
    <img width="200" height="200"
      src="https://webpack.js.org/assets/icon-square-big.svg">
  </a>
  <h1>Script Loader</h1>
</div>

<h2 align="center">Install</h2>

```bash
npm install --save-dev script-loader
```

<h2 align="center">Usage</h2>

Executes JS script once in global context.

> :wanring: Doesn't work in NodeJS

### Config (recommended)

```js
import exec from 'script.exec.js';
```

**webpack.config.js**
```js
module.exports = {
  module: {
    rules: [
      {
        test: /\.exec.js$/,
        use: [ 'script-loader' ]
      }
    ]
  }
}
```

### Inline

```js
import exec from 'script-loader!./script.js';
```

<h2 align="center">Maintainer</h2>

<table>
  <tbody>
    <tr>
      <td align="center">
        <img width="150 height="150" src="https://github.com/sokra.png?s=150">
        <br>
        <a href="https://github.com/sokra">Tobias Koppers</a>
      </td>
    <tr>
  <tbody>
</table>


[npm]: https://img.shields.io/npm/v/script-loader.svg
[npm-url]: https://npmjs.com/package/script-loader

[node]: https://img.shields.io/node/v/script-loader.svg
[node-url]: https://nodejs.org

[deps]: https://david-dm.org/webpack/script-loader.svg
[deps-url]: https://david-dm.org/webpack/script-loader

[tests]: http://img.shields.io/travis/webpack/script-loader.svg
[tests-url]: https://travis-ci.org/webpack/script-loader

[cover]: https://coveralls.io/repos/github/webpack/script-loader/badge.svg
[cover-url]: https://coveralls.io/github/webpack/script-loader

[chat]: https://badges.gitter.im/webpack/webpack.svg
[chat-url]: https://gitter.im/webpack/webpack
