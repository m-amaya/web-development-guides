# Setup Babel with Nodemon

## Installation

```bash
$ npm install --save-dev babel-cli babel-preset-latest
```

## Usage

In your `package.json` file make the following changes.
```json
{
    "scripts": {
        "babel-node": "babel-node --presets=/*a*/ --ignore='foo|bar|baz'"
    }
}
```

```bash
$ nodemon --exec npm run babel-node -- path/to/script.js
```

### Arguments Caveat

Calling nodemon with `babel-node` may lead to arguments getting parsed incorrectly if you forget to use a double dash. Using npm-scripts helpers prevent this. If you choose to skip using npm-scripts, it can be expressed as:

```bash
$ nodemon --exec babel-node --presets=es2015 --ignore='foo\|bar\|baz' -- path/to/script.js
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
