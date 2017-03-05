# Setup Babel with Jasmine

## Installation

```bash
$ npm install --save-dev babel-register
```

## Usage

In your `spec/support/jasmine.json` file, make the following changes:
```json
{
    "helpers": [
        "../node_modules/babel-register/lib/node.js"
    ]
}
```

This file is created when you setup a project with the `jasmine init` command.

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
