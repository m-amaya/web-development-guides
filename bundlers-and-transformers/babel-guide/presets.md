# Babylon Presets

## Presets

### Official Presets

* [babel-preset-es2015](https://github.com/babel/babel/blob/7.0/packages/babel-preset-es2015)
* [babel-preset-es2016](https://github.com/babel/babel/blob/7.0/packages/babel-preset-es2016)
* [babel-preset-es2017](https://github.com/babel/babel/blob/7.0/packages/babel-preset-es2017)
* [babel-preset-flow](https://babeljs.io/docs/plugins/preset-flow/)
* [babel-preset-latest](https://github.com/babel/babel/blob/7.0/packages/babel-preset-latest)
* [babel-preset-react](https://github.com/babel/babel/blob/7.0/packages/babel-preset-react)

### Stage-X (Experimental Presets)

The [TC39](https://github.com/tc39) categorizes proposals into the following stages:

* [babel-preset-stage-0](https://github.com/babel/babel/blob/7.0/packages/babel-preset-stage-0) - **Strawman:** just an idea, possible Babel plugin.
* [babel-preset-stage-1](https://github.com/babel/babel/blob/7.0/packages/babel-preset-stage-1) - **Proposal:** This is worth working on.
* [babel-preset-stage-2](https://github.com/babel/babel/blob/7.0/packages/babel-preset-stage-2) - **Draft:** Initial spec.
* [babel-preset-stage-3](https://github.com/babel/babel/blob/7.0/packages/babel-preset-stage-3) - **Candidate:** Complete spec and initial browser implementations.
* [babel-preset-env](https://github.com/babel/babel-preset-env)

Babel maintains:

* a preset for each yearly release of ECMAScript (JavaScript), starting from ES6/ES2015.
* a preset for react (JSX/Flow).
* a preset for each stage (0-3) of the TC-39 Process for ECMAScript proposals.
* a preset that can automatically determine plugins and polyfills you need based on your supported environments.

## Transformers

### ES3

* [es3-member-expression-literals](https://babeljs.io/docs/plugins/transform-es3-member-expression-literals/)
* [es3-property-literals](https://babeljs.io/docs/plugins/transform-es3-property-literals/)

### ES5

* [es5-property-mutators](https://babeljs.io/docs/plugins/transform-es5-property-mutators/)

### ES2015

* [es2015-arrow-functions](https://babeljs.io/docs/plugins/transform-es2015-arrow-functions/)
* [es2015-block-scoped-functions](https://babeljs.io/docs/plugins/transform-es2015-block-scoped-functions/)
* [es2015-block-scoping](https://babeljs.io/docs/plugins/transform-es2015-block-scoping/)
* [es2015-classes](https://babeljs.io/docs/plugins/transform-es2015-classes/)
* [es2015-computed-properties](https://babeljs.io/docs/plugins/transform-es2015-computed-properties/)
* [es2015-constants](https://babeljs.io/docs/plugins/check-es2015-constants/)
* [es2015-destructuring](https://babeljs.io/docs/plugins/transform-es2015-destructuring/)
* [es2015-duplicate-keys](https://babeljs.io/docs/plugins/transform-es2015-duplicate-keys/)
* [es2015-for-of](https://babeljs.io/docs/plugins/transform-es2015-for-of/)
* [es2015-function-name](https://babeljs.io/docs/plugins/transform-es2015-function-name/)
* [es2015-literals](https://babeljs.io/docs/plugins/transform-es2015-literals/)
* [es2015-object-super](https://babeljs.io/docs/plugins/transform-es2015-object-super/)
* [es2015-parameters](https://babeljs.io/docs/plugins/transform-es2015-parameters/)
* [es2015-shorthand-properties](https://babeljs.io/docs/plugins/transform-es2015-shorthand-properties/)
* [es2015-spread](https://babeljs.io/docs/plugins/transform-es2015-spread/)
* [es2015-sticky-regex](https://babeljs.io/docs/plugins/transform-es2015-sticky-regex/)
* [es2015-template-literals](https://babeljs.io/docs/plugins/transform-es2015-template-literals/)
* [es2015-typeof-symbol](https://babeljs.io/docs/plugins/transform-es2015-typeof-symbol/)
* [es2015-unicode-regex](https://babeljs.io/docs/plugins/transform-es2015-unicode-regex/)

### ES2016

* [exponentiation-operator](https://babeljs.io/docs/plugins/transform-exponentiation-operator/)

### ES2017

* [async-to-generator](https://babeljs.io/docs/plugins/transform-async-to-generator/)

### Modules

* [es2015-modules-amd](https://babeljs.io/docs/plugins/transform-es2015-modules-amd/)
* [es2015-modules-commons](https://babeljs.io/docs/plugins/transform-es2015-modules-commonjs/)
* [es2015-modules-systemjs](https://babeljs.io/docs/plugins/transform-es2015-modules-systemjs/)
* [es2015-modules-umd](https://babeljs.io/docs/plugins/transform-es2015-modules-umd/)

### Experimental

* [async-generator-functions](https://babeljs.io/docs/plugins/transform-async-generator-functions/)
* [async-to-module-method](https://babeljs.io/docs/plugins/transform-async-to-module-method/)
* [class-properties](https://babeljs.io/docs/plugins/transform-class-properties/)
* [decorators](https://babeljs.io/docs/plugins/transform-decorators/)
* [do-expressions](https://babeljs.io/docs/plugins/transform-do-expressions/)
* [export-extensions](https://babeljs.io/docs/plugins/transform-export-extensions/)
* [function-bind](https://babeljs.io/docs/plugins/transform-function-bind/)
* [object-rest-spread](https://babeljs.io/docs/plugins/transform-object-rest-spread/)

### Minification ([Beta](https://github.com/babel/babili))

* [inline-environment-variables](https://babeljs.io/docs/plugins/transform-inline-environment-variables/)
* [inline-consecutive-adds](https://babeljs.io/docs/plugins/transform-inline-consecutive-adds/)
* [member-expression-literals](https://babeljs.io/docs/plugins/transform-member-expression-literals/)
* [merge-sibling-variables](https://babeljs.io/docs/plugins/transform-merge-sibling-variables/)
* [minify-booleans](https://babeljs.io/docs/plugins/transform-minify-booleans/)
* [minify-constant-folding](https://babeljs.io/docs/plugins/minify-constant-folding/)
* [minify-dead-code-elimination](https://babeljs.io/docs/plugins/minify-dead-code-elimination/)
* [minify-empty-function](https://babeljs.io/docs/plugins/minify-empty-function/)
* [minify-flip-comparisons](https://babeljs.io/docs/plugins/minify-flip-comparisons/)
* [minify-guarded-expressions](https://babeljs.io/docs/plugins/minify-guarded-expressions/)
* [minify-infinity](https://babeljs.io/docs/plugins/minify-infinity/)
* [minify-mangle-names](https://babeljs.io/docs/plugins/minify-mangle-names/)
* [minify-numeric-literals](https://babeljs.io/docs/plugins/minify-numeric-literals/)
* [minify-replace](https://babeljs.io/docs/plugins/minify-replace/)
* [minify-simplify](https://babeljs.io/docs/plugins/minify-simplify/)
* [minify-type-constructors](https://babeljs.io/docs/plugins/minify-type-constructors/)
* [node-env-inline](https://babeljs.io/docs/plugins/transform-node-env-inline/)
* [property-literals](https://babeljs.io/docs/plugins/transform-property-literals/)
* [regexp-constructors](https://babeljs.io/docs/plugins/transform-regexp-constructors/)
* [remove-console](https://babeljs.io/docs/plugins/transform-remove-console/)
* [remove-debugger](https://babeljs.io/docs/plugins/transform-remove-debugger/)
* [simplify-comparison-operators](https://babeljs.io/docs/plugins/transform-simplify-comparison-operators/)
* [undefined-to-void](https://babeljs.io/docs/plugins/transform-undefined-to-void/)

### React

* [react-constant-elements](https://babeljs.io/docs/plugins/transform-react-constant-elements/)
* [react-display-name](https://babeljs.io/docs/plugins/transform-react-display-name/)
* [react-inline-elements](https://babeljs.io/docs/plugins/transform-react-inline-elements/)
* [react-jsx](https://babeljs.io/docs/plugins/transform-react-jsx/)
* [react-jsx-compat](https://babeljs.io/docs/plugins/transform-react-jsx-compat/)
* [react-jsx-self](https://babeljs.io/docs/plugins/transform-react-jsx-self/)
* [react-jsx-source](https://babeljs.io/docs/plugins/transform-react-jsx-source/)

### Other

* [eval](https://babeljs.io/docs/plugins/transform-eval/)
* [flow-comments](https://babeljs.io/docs/plugins/transform-flow-comments/)
* [flow-strip-types](https://babeljs.io/docs/plugins/transform-flow-strip-types/)
* [jscript](https://babeljs.io/docs/plugins/transform-jscript/)
* [object-assign](https://babeljs.io/docs/plugins/transform-object-assign/)
* [object-set-prototype-of-to-assign](https://babeljs.io/docs/plugins/transform-object-set-prototype-of-to-assign/)
* [proto-to-assign](https://babeljs.io/docs/plugins/transform-proto-to-assign/)
* [regenerator](https://babeljs.io/docs/plugins/transform-regenerator/)
* [runtime](https://babeljs.io/docs/plugins/transform-runtime/)
* [strict-mode](https://babeljs.io/docs/plugins/transform-strict-mode/)

### Miscellaneous

* [external-helpers](https://babeljs.io/docs/plugins/external-helpers/)
* [undeclared-variables-check](https://babeljs.io/docs/plugins/undeclared-variables-check/)

### Syntax

#### Experimental

* [async-generators](https://babeljs.io/docs/plugins/syntax-async-generators/)
* [class-properties](https://babeljs.io/docs/plugins/syntax-class-properties/)
* [decorators](https://babeljs.io/docs/plugins/syntax-decorators/)
* [do-expressions](https://babeljs.io/docs/plugins/syntax-do-expressions/)
* [dynamic-import](https://babeljs.io/docs/plugins/syntax-dynamic-import/)
* [export-extensions](https://babeljs.io/docs/plugins/syntax-export-extensions/)
* [flow](https://babeljs.io/docs/plugins/syntax-flow/)
* [function-bind](https://babeljs.io/docs/plugins/syntax-function-bind/)
* [function-sent](https://babeljs.io/docs/plugins/syntax-function-sent/)
* [jsx](https://babeljs.io/docs/plugins/syntax-jsx/)
* [object-rest-spread](https://babeljs.io/docs/plugins/syntax-object-rest-spread/)

#### Enabled By Default

* [async-functions](https://babeljs.io/docs/plugins/syntax-async-functions/) (since babylon 6.9.1)
* [exponentiation-operator](https://babeljs.io/docs/plugins/syntax-exponentiation-operator/) (since babylon 6.9.1)
* [trailing-function-commas](https://babeljs.io/docs/plugins/syntax-trailing-function-commas/) (since babylon 6.9.1)
