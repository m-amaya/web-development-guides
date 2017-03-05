# Babel CLI

## Installation

```bash
$ npm install --save-dev babel-cli
```

## Usage

### Compile Files

```bash
$ babel script.js
$ babel script.js --out-file script-compiled.js
$ babel script.js --watch --out-file script-compiled.js
```

### Compile with Source Maps

```bash
$ babel script.js --out-file script-compiled.js --source-maps
$ babel script.js --out-file script-compiled.js --source-maps inline
```

### Compile Directories

```bash
$ babel src --out-dir lib
$ babel src --out-file script-compiled.js
```

### Ignore Files

```bash
$ babel src --out-dir lib --ignore spec.js,test.js
```

### Copy Files

```bash
$ babel src --out-dir lib --copy-files
```

### Piping Files

```bash
$ babel --out-file script-compiled.js < script.js
```

### Using Plugins

```bash
$ babel script.js --out-file script-compiled.js --plugins=transform-runtime,transform-es2015-modules-amd
```

### Using Presets

```bash
$ babel script.js --out-file script-compiled.js --preset=es2015,react
```

### Ignoring .babelrc

```bash
$ babel --no-babelrc script.js --out-file script-compiled.js --preset=es2015,react
```

### Advanced Options

* [list of options](https://babeljs.io/docs/core-packages/#options)
