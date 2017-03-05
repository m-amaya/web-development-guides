# Setup Babel with Grunt

## Installation

```bash
$ npm install --save-dev grunt-babel
```

## Usage

```javascript
require('load-grunt-tasks')(grunt);

grunt.initConfig({
    "babel": {
        options: {
            sourceMap: true
        },
        dist: {
            files: {
                "dist/app.js": "src/app.js"
            }
        }
    }
});

grunt.registerTask("default", [ "babel" ]);
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
