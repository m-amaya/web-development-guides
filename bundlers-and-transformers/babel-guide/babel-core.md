# Babel Core

```javascript
var babel = require("babel-core");
import { transform } from 'babel-core';
import * as babel from 'babel-core';
```

All transformations will use your local configurations file (`.babelrc` or `package.json`).

### `transform`

Transforms the passed in `code`.

```javascript
babel.transform(code:<String>, options?:<Object>)
// => { code, map, ast }
```

### `transformFile`

Asynchronously transforms the entire contents of a file.

```javascript
babel.transformFile(filename:<String>, options?:<Object>, callback:<Function(err, result)>);
// => { code, map, ast }
```

### `transformFileSync`

Synchronous version of `babel.transformFile`.

```javascript
babel.transformFileSync(filename:<String>, options?:<Object>);
// => { code, map, ast }
```

### `transformFromAst`

Given an AST, transform it.

```javascript
babel.transformFromAst(ast:<Object>, code?:<String>, options?:<Object>);
// => { code, map, ast }
```
