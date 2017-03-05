# Babel Packages

## Core Packages

**[babel-core](https://github.com/babel/babel/blob/7.0/packages/babel-core)** - the Babel compiler itself; it exposes the `babel.transform` method, where `transformCode = transform(src).code`. The compiler can be broken down into three parts:

    1. [babylon](https://github.com/babel/babylon) - a JavaScript parser used in Babel
    2. The transformer[s] (a.k.a all the plugins/presets). These all use [babel-traverse](https://github.com/babel/babel/blob/7.0/packages/babel-traverse) to traverse through the AST.
    3. [babel-generator](https://github.com/babel/babel/blob/7.0/packages/babel-generator) - the generator

The flow:

```
input string --> babylon parset --> AST --> transformer[s] --> AST --> babel-generator --> output string
```

## Other Packages

* [babel-cli](https://github.com/babel/babel/blob/7.0/packages/babel-cli) - the CLI tool that runs `babel-core` and helps with outputting to a directory, a file, stdout, and more (also includes `babel-node`).
* [babel-types](https://github.com/babel/babel/blob/7.0/packages/babel-types) - used to validate, build, change AST nodes. It is a Lodash-esque utility library for AST nodes.
* [babel-polyfill](https://github.com/babel/babel/blob/7.0/packages/babel-polyfill) - literally a wrapper around `core-js` and `regenerator-runtime`.
* [babel-runtime](https://github.com/babel/babel/blob/7.0/packages/babel-runtime) - similar to the polyfill except that it doesn't modify the global scope and is to be used with `babel-plugin-transform-runtime` (usually in library/plugin code).
* [babel-register](https://github.com/babel/babel/blob/7.0/packages/babel-register) - a way to automatically compile files with babel on the fly by binding to node's `require`.
* [babel-template](https://github.com/babel/babel/blob/7.0/packages/babel-template) - a helper function to make AST nodes. Instead you can pass a string representing the code you want to create rather than tediously building them using `babel-types`.
* [babel-helpers](https://github.com/babel/babel/blob/7.0/packages/babel-helpers) - a collection of helper functions used by Babel transforms.
* [babel-code-frame](https://github.com/babel/babel/blob/7.0/packages/babel-code-frame) - a standalone package used to generate errors that prints the source code and points to error locations.
