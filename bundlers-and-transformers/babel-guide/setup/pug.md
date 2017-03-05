# Setup Babel with Pug

## Installation

```bash
$ npm install --save-dev jstransformer-babel
```

## Usage

Now you can use ES6 in your pug templates.
```pug
script
    :babel
        console.log("Hello World !!!");
        class Person {
            constructor(name) {
                this.name = name;
            }

            sayName() {
                console.log(`Hello, my name is ${this.name}`);
            }
        }
        var person = new Person("Apoxx");
        person.sayName();
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
