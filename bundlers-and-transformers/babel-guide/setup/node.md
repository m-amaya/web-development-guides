# Setup Babel with Node

## Installation

```bash
$ npm install --save-dev babel-core babel-polyfill
```

## Usage

```javascript
require("babel-polyfill")
require("babel-core").transform("code", options);
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
