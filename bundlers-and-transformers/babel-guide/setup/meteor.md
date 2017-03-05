# Setup Babel with Meteor

## Installation

```bash
$ meteor add ecmascript
```

> **Note:** As of Meteor 1.2, the `ecmascript` package is installed by default for all new apps.

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
