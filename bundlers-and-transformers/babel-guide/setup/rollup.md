# Setup Babel with Rollup

## Installation

```bash
$ npm install --save-dev rollup rollup-plugin-babel
```

## Usage

```javascript
const rollup = require('rollup');
const babel  = require('rollup-plugin-babel');

rollup.rollup({
    entry: 'src/main.js',
    plugins: [ babel() ]
}).then(function(bundle) {
    bundle.write({
        dest: "dist/bundle.js",
        format: "umd"
    });
});
```

## Create `.babelrc` Configuration File

Save a preset:
```bash
$ npm install babel-preset-es2015-rollup --save-dev
```

Enable presets in `.babelrc` file:
```json
{
    "presets": [ "env" ]
}
```
