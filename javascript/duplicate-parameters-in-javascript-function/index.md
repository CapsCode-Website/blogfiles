Hi Devs,

In this article i will introduce you to one of the most confusing and common doubt for every newbie devs, Duplicate parameters in javascript functions

## Table Of Contents

- [duplicating parameter in regular JS function](#chapter-0)
- [duplicating parameter in non strict mode](#chapter-1)
- [duplicating parameter in strict mode](#chapter-2)
- [How do arrow functions treat duplicate parameters](#chapter-3)

## First we will see duplicating parameters in regular JavaScript function. <a name="chapter-0"></a>

```js
//this is syntax of duplicating parameter in js function
function Func(first, second, first) {
  console.log(first, second, first);
}
```

### In **non-strict mode**, regular JavaScript functions allow duplicate named parameters <a name="chapter-1"></a>

```js
function Func(first, second, first) {
  console.log(first, second, first);
}
// first => 1
// second => 2
// first => 3
Func(1, 2, 3); // 3 2 3

// first => 1
// second => 2
// first => undefined
Func(1, 2); //undefined  [undefined, 2, undefined]
```

### Lets check this in **strict mode**,<a name="chapter-2"></a>

```js
function Func(first, second, first) {
  "use strict";
  console.log(first, second, first);
}
//Throws an error because of duplicate parameters (Strict mode)
```

In Strict mode we cannot duplicate the parameter name.

## How do arrow functions treat duplicate parameters? <a name="chapter-3"></a>

Now here is something about arrow functions:

> Unlike regular functions, arrow functions do not allow duplicate parameters, whether in strict or non-strict mode. Duplicate parameters will cause a `Syntax Error` to be thrown.

```js
// Always throws a syntax error
const Func = (first, second, first) => {
  console.log(first, second);
};
```

CONGRATULATIONS, YOU HAVE LEARNT ONE NEW TOPIC TODAY.
VISIT https://www.capscode.in/blog TO LEARN MORE...

Thanks,\
CapsCode
