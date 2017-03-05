# Setup Babel with Browserify

## Installation

```bash
$ npm install --save-dev babelify babel-polyfill
```

## Usage

Via CLI
```bash
$ browserify script.js -t babelify --outfile bundle.js
```

Via Node API
```javascript
require('babel-polyfill');
const fs         = require('fs');
const browserify = require('browserify');
const babelify   = require('babelify');

browserify({ debug: true })
    .transform(babelify)
    .require('./script.js', { entry: true })
    .bundle()
    .on('error', function(err) { console.log('Error:' + err.message); })
    .pipe(fs.createWriteStream('bundle.js'));
```

### Passing Options

Via CLI
```bash
$ browserify -d -e script.js -t [ babelify --comments false ]
```

Via Node API
```javascript
browserify()
    .transform(babelify.configure({ comments: false }));
```

Via `package.json`
```json
{
    "transform": [[ "babelify", { "comments": false } ]]
}
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
