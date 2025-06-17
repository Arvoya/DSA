# Using JavaScript

## Modern JavaScript Features

### Arrow Functions

``` js
const echo = () => {...}
```

- These cannot be used as constructors or generators.
- They don't bind the *this* value.
- They don't have an arguments object or a prototype property.

``` js
//NOTE: You can initialize a default value incase one isn't provided 

const test = (s = "oh no") => {
  console.log(s)
}

test()
//prints "oh no"

test("yes")
//prints "yes"

test()
//prints "oh no"
```

### The Spread Operator

`(...)`

```js
const myArray = [3, 1, 4, 1, 5, 9, 2, 6];

const arrayMax = Math.max(...myArray);

console.log(arrayMax);
//prints 9
```

### The Destructuring Statement

```js
let [a, b, c] = [1, 2, 3];
let [x, y, z] = [4, 5, 6];

console.log(a, b, c); // 1 2 3
console.log(x, y, z); // 4 5 6

//NOTE: Swap using destructuring and a temporary array
[a, b, c, x, y, z] = [x, y, z, a, b, c];

console.log(a, b, c); // 4 5 6
console.log(x, y, z); // 1 2 3
```

### Modules

> *Modules* allow you to split code into pieces you can import when needed,
providing a way to package functionality that is easier to understand and maintain.

They come in 2 formats.

1. *CommonJS modules* (an earlier format used in Node.js)
2. *ECMAScript modules* (the latest format, generally used by browsers)

#### CommonJS Modules

```js
//file: add.js
const add = (a, b) => {return a + b};
module.exports = {add};
```

```js
const {add} = require("add.js");
```

#### ECMASscript Modules

```js
export const subtract = (a, b) => {return a - b};
//or 
const subtract = (a, b) => {return a - b};
export {subtract};
```

```js
import {subtract} from "subtract.js"
```

> You can also use ECMAScript import and export statements in Node.js, but only
if you use the **.mjs** extension instead of the **.js** extension, which is
reserved for CommonJS modules.

### Closures and Immediatly Invoked Function Expressions


