Hello Devs,

In this article we will learn Destructuring in JavaScript

## Table Of Contents

1. [Array Destructuring in JavaScript](#one)
2. [Additional use of Array Destructuring](#two)
3. [Assigning default values using destructuring assignment](#three)
4. [Destructuring of nested array](#four)
5. [Object Destructuring in JavaScript](#five)
6. [Nested object destructuring](#six)
7. [How to skip values in Array destructuring](#seven)
8. [Combined Array and Object Destructuring](#eight)

Without wasting any time lets get into it,

The destructuring assignment syntax is a JavaScript expression that makes it possible to unpack values from arrays, or properties from objects, into distinct variables.

But why do we need destructuring ?
Lets first see the traditional way of accessing the array elements and object properties,

```js
let arr = [1, 2, 3, 4];
arr[2]; //3

let obj = {
  fname: "john",
  lname: "doe",
};
obj.fname; //john
//or
obj["fname"]; //john
```

Think of accessing elements or properties when the array or object is nested, its little complex.

Now we will see how things gets simpler/ easier using Destructuring concept.

A destructuring assignment looks like this:

**«pattern» = «value»**

## 1. Array Destructuring: <a name="one"></a>

**syntax:**

```js
[a, b, c] = some_array;
```

**Example:**

```js
let arr = ["John", "Doe"];

// older way
let firstName = arr[0];
let lastName = arr[1];
console.log(firstName, lastName); //John Doe

//array destructuring way
let [firstName, lastName] = arr;
console.log(firstName, lastName); //John Doe

//what if there are more values in array
var [fname, lname] = ["john", "doe", "capscode", 26, car];

//we can use rest operator,
var [fname, lname, ...others] = ["john", "doe", "capscode", 26, car];
```

## 2. Some Additional use of Destructuring <a name="two"></a>

```js
//Works with any iterables of JavaScript
String iterable
let [a, b, c] = "abc";
console.log(a) // "a"
console.log(b) // "b"
console.log(c) // "c"

let [first, ...rest] = "Hello";
console.log(first) // "H"
console.log(rest) // ["e", "l", "l", "o"]

//Swap variables trick using array destructuring
let guest = "Jane";
let admin = "Pete";

// Swap values: make guest=Pete, admin=Jane
[guest, admin] = [admin, guest];
```

## 3. we can also assign default values using destructuring assignment <a name="three"></a>

```js
let [firstName, surname] = [];
alert(firstName); // undefined
alert(surname); // undefined

so to get out of this,
// default values
let [name = "Guest", surname = "Anonymous"] = ["Julius"];
alert(name);    // Julius (from array)
alert(surname); // Anonymous (default used)

```

## 4. Destructuring of nested array <a name="four"></a>

```js
const person = ["John", ["capscode", "google", "yahoo"], "Doe"];
const [fname, [comp1, comp2, comp3]] = person;
console.log(comp3); //"yahoo"
```

## 5. Object Destructuring <a name="five"></a>

**Syntax:**

```js
let {var1, var2} = {var1:…, var2:…}
```

**Example:**

```js
let person = {
  fname: "John",
  lname: "Doe",
  company: "capscode",
};

let { fname, lname, company } = person;

//we can also use rest operator
let { fname, ...others } = person;
console.log(others);
console.log(others.lname);
console.log(others.company);
```

what if we will use Destructuring assignment without declaration?

```js
let fname, lname, company;

{fname, lname, company} = {
     fname: "John",
     lname: "Doe",
     company: "capscode"
};
// error in this line
```

The problem is that JavaScript treats `{.....}` in the main code flow (not inside another expression) as a code block.

The parentheses `( ... )` around the assignment statement are required when using object literal destructuring assignment without a declaration.

`{a, b} = {a: 1, b: 2}` is not valid stand-alone syntax, as the `{a, b}` on the left-hand side is considered a block and not an object literal.

```js
// okay now
({ fname, lname, company } = {
  fname: "John",
  lname: "Doe",
  company: "capscode",
});
```

**🔥NOTE:** 🔥Your `(....)` expression needs to be preceded by a semicolon or it may be used to execute a function on the previous line.
I will tell why I am saying like this,
just take a look at the below **2 examples carefully**,

```js
let href, pathname;
({ href } = window.location)(({ pathname } = window.location));
//TypeError: (intermediate value)(intermediate value) is not a function

let href;
somefunc()(({ href } = window.location));
//TypeError: somefunc(...) is not a function
```

🔥 What's happening is, Without the semicolon, when parsing, Javascript engine considers both lines as a single call expression.
**🔥 So if you are using `()` after any `()` then put `;` after first `()` 😅**

## 6.Nested object destructuring <a name="six"></a>

```js
const student = {
  name: "John Doe",
  age: 16,
  scores: {
    maths: 74,
    english: 63,
  },
};

// We define 3 local variables: name, maths, science
const {
  name,
  scores: { maths, science = 50 },
} = student;
console.log(maths); //74
console.log(english); //undefined
```
## 7. How to skip values in Array destructuring <a name="seven"></a>
```js
//IN ARRAY
let arr=[4,1,6]
let [,...op] = arr
console.log(op) //[1, 6]

let [,,op] = arr
console.log(op) //6

let [,op] = arr
console.log(1) //6

```
## 8.Combined Array and Object Destructuring <a name="eight"></a>

**Example,**

```js
const props = [
  { id: 1, name: "John" },
  { id: 2, name: "Saam" },
  { id: 3, name: "Rahul" },
];

const [, , { name }] = props;

console.log(name); // "Rahul"
```

Destructuring values that are not an object, array, or iterable gives you a `TypeError`

```js
let [NaN_] = NaN //TypeError: NaN is not iterable
let [Boolean_] = true // TypeError: true is not iterable
let [Number_] = 10 = TypeError: 10 is not iterable
let [NULL_] = nul //TypeError: null is not iterable
let [undefined_] = undefined //TypeError: undefined is not iterable

// NOTE: String are iterable in JavaScript
let [String_] = "CapsCode" // "C"
```

Thank you for reading this far. This is a brief introduction of **Destructuring Assignment in JavaScript** .
If you find this article useful, like and share this article. Someone could find it useful too. If you find anything technically inaccurate please feel free to comment below.

Hope its a nice and informative read for you.
VISIT https://www.capscode.in/blog TO LEARN MORE...
See you in my next Blog article, Take care!!

Thanks,\
CapsCode
