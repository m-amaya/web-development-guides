# Setup Babel with Connect

## Installation

```bash
$ npm install --save-dev babel-connect
```

## Usage

```javascript
const babelMiddleware = require('babel-connect');

app.use(babelMiddleware({
    options: {
        // options to use when transforming files
    },
    src: "assets",
    dest: "cache"
}));

app.use(connect.static("cache"));
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
