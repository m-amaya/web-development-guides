# Setup Babel with Webpack

## Installation

```bash
$ npm install --save-dev babel-loader babel-core babel-polyfill
```

## Usage

`app.js`

```javascript
import "babel-polyfill";
```

Via `webpack.config.js`
```javascript
module.exports = {
    entry: [ 'babel-polyfill', './app.js' ],
    module: {
        rules: [
            {
                test: /\.js$/,
                exclude: /node_modules/,
                loader: 'babel-loader'
            }
        ]
    }
}
```

Via Loader
```javascript
var Person = require("babel!./Person.js").default;
new Person();
```

## Create `.babelrc` Configuration File

Save a preset:
```bash
$ npm install babel-preset-env --save-dev
```

Enable presets in `.babelrc` file:
```json
{
    "presets": [ "env" ]
}
```
