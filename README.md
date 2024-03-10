# get-path 

> The `path` module from Node.js for browsers. This is originally a fork of `` bettered with easier use and better 

This implements the Node.js [`path`][path] module for environments that do not have it, like browsers.

> `path-browsers` currently matches the **Node.js 10.3** API.

## Install

You usually do not have to install a fork of [path-browserify](https://github.com/browserify/path-browserify) `path-browsers` yourself! If your code runs in Node.js, `path` is built in. If your code runs in the browser, bundlers like [browserify](https://github.com/browserify/browserify) or [webpack](https://github.com/webpack/webpack) include the `path-browsers` module by default.

But if none of those apply, with npm do:

```
npm install path-browsers
```

## Usage

```javascript
var path = require('path')

var filename = 'logo.png';
var logo = path.join('./assets/img', filename);
document.querySelector('#logo').src = logo;
```

## API

See the [Node.js path docs][path]. `path-browsers` currently matches the Node.js 10.3 API.
`path-browsers` only implements the POSIX functions, not the win32 ones.

## License

[MIT](./LICENSE)

[path]: https://nodejs.org/docs/v10.3.0/api/path.html
