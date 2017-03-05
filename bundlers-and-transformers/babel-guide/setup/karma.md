# Setup Babel with Karma

## Installation

```bash
$ npm install --save-dev karma-babel-preprocessor
```

## Usage

```javascript
module.exports = function(config) {
    config.set({
        files: [
            "src/**/*.js",
            "test/**/*.js"
        ],
        preprocessors: {
            "src/**/*.js": [ "babel" ],
            "test/**/*.js": [ "babel" ]
        },
        "babelPreprocessor": {
            // options go here
        }
    });
};
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
