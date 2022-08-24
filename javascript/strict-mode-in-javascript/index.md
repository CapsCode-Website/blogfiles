It is new feature included in ES5.
It is used to execute the code in **"strict mode"**. we can achieve this by adding 'use strict' in the beginning of your script or function. only the code below the assignment comes under strict mode.

Declaring in the beginning of your script makes it available globally in the code (inside the function as well).
Declaring inside the function make it available locally inside the function.

##Strict mode helps out in a couple ways:

- It catches some common coding bloopers, throwing exceptions.
- Strict mode eliminates some JavaScript silent errors by changing them to throw errors.
- It prevents, or throws errors, when relatively "unsafe" actions are taken (such as gaining access to the global object).
- It disables features that are confusing or poorly thought out.
- Strict mode makes it easier to write “secure” JavaScript.

### List of features

- Disallows global variables(object literal also).

```javascript
x = 20;
```

- Assignment to a reserved keyword (inc eval & arguments) is not allowed

```javascript
var undefined = 5; // throws a TypeError
var Infinity = 5; // throws a TypeError
```

- Writing to a read-only property is not allowed:

```javascript
var obj = {};
Object.defineProperty(obj, "x", { value: 0, writable: false });
obj.x = 3.14; // This will cause an error
```

- Writing to a get-only property is not allowed:

```javascript
var obj = {
  get x() {
    return 0;
  },
};
obj.x = 3.14; // This will cause an error
```

- Deleting a variable, object, function is not allowed

```javascript
delete obj; //SyntaxError: Delete of an unqualified identifier in strict mode
```

- Attempts to delete undeletable properties will throw

```javascript
delete Object.prototype; //throws error
```

- Requires all property names in an object literal to be unique

```javascript
var x = { x1: "1", x1: "2" }; //throws error
```

- Function parameter names must be unique

```javascript
function sum (x, x) {...}//throw error
```

- Octal numeric literals are not allowed:

```javascript
var x = 010; // This will cause an error
```

- with statement is not allowed:

```javascript
with (Math) {
  x = cos(2);
} // This will cause an error
```

- eval in strict mode does not introduce new variables

```javascript
eval("var x = 2");
```

- deleting plain names throws error.

```javascript
var x;
delete x;
```

###SOME EXAMPLES/ OBSERVATIONS

```javascript
function func() {
  "use strict";
  y = 100; //this will not throw an error till the function is not called
}
```

```javascript
"use strict";
function func() {
  y = 100; //this will not throw an error till the function is not called
}
```

```javascript
function func() {
  myGlobal = 5; //this will NOT give error
}

(function () {
  "use strict";
  func();
})();

function func_strict() {
  "use strict";
  myGlobal = 5; //this will give error
}
```

We hope that this post is helpful for you.
If really, Please rate us and let us know your review in the comment.

that's it my dear devs :)

If you like it please give a 👍

Thank you,\
CapsCode\
www.capscode.in
