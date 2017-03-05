# Setup Babel with Mocha

## Installation

```bash
$ npm install --save-dev babel-register babel-polyfill
```

## Usage

In your `package.json` file, make the following changes.
```json
{
    "scripts": {
        "test": "mocha --require babel-polyfill --compilers js:babel-register"
    }
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
