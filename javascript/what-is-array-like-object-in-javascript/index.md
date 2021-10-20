_Before understanding what is Array like object, lets first have a look at what is an array and what is an object._

**Array**: Array is an indexed collection that can hold data of any type.
They are created with [ ].
Example: let arr = [1, 2, 'capscode', true, null, ,12];
we can access element as arr[2] // 'capscode'

![Alt Text](https://raw.githubusercontent.com/CapsCode-Website/blogfiles/master/javascript/what-is-array-like-object-in-javascript/1.jpg?raw=true)

**Object**: Object are the Keyed Collection that hold the properties in key: value pair.
They are created with { }.
Example:

```javascript
let person = {
  first_name: "John",
  last_name: "Doe",
  company: "capscode",
};
```

we can access property as

```javasript
person.company // 'capscode'
```

or

```javascript
person["company"]; // 'capscode'
```

So far so good.
let now have a look at what is an ARRAY LIKE OBJECT'

**An array-like is an object**
It has indexed access to the elements and a non-negative length property to know the number of elements in it. These are the only similarities it has with an array.
Doesn't have any of the Array methods like, push, pop, join, map, etc.
Objects that have indexed properties and length are called array-like. Such objects may also have other properties and methods, but lack the built-in methods of arrays.

Array like object looks like:

```javascript
var arr_like_obj = {
  0: "we",
  1: "are",
  2: "capscode",
  length: 3,
};
```

this is a object which looks like array.
Some Common examples of Array-like Objects are the **arguments object in functions** and **HTMLCollection** or **NodeList objects** returned from methods like document.getElementsByTagName or document.querySelectorAll

In Array like object we **cannot access properties** like we used to do in object.

```javascript
arr_like_obj.0; //SyntaxError: Unexpected number
```

but

```javascript
arr_like_obj[0]; //'we'
```

you can checkout difference between these two type of object property access [here](https://stackoverflow.com/questions/38933692/why-doesnt-object-dot-notation-work-in-a-for-in-loop)

```javascript
arr_like_obj.length; // 3

Array.isArray(arr_like_obj); // returns false
```

both array and array like are object in javascript:

```javascript
arr_like instanceof Object; // returns, true
[] instanceof Object; // returns, true
```

**LETS HAVE A LOOK ON SOME MORE INTERESTING EXAMPLES OF ARRAY, OBJECT, ARRAY LIKE OBJECT**

```javascript
// simple array
const arr = ["a", "b", "c"];
console.log(Object.keys(arr)); // ['0', '1', '2']

// array-like object
const obj = { 0: "a", 1: "b", 2: "c" };
console.log(Object.keys(obj)); // ['0', '1', '2']

// array-like object with random key ordering
const anObj = { 100: "a", 2: "b", 7: "c" };
console.log(Object.keys(anObj)); // ['2', '7', '100']

const object1 = {
  a: "somestring",
  b: 42,
  c: false,
};

console.log(Object.keys(object1));
// expected output: ["a", "b", "c"]
```

But why do we need them ?
JavaScript HTMLCollection is an Array-like object

```html
<div id="main">
  <ul>
    <ol type="1">
      <li>...</li>
      <li>...</li>
      <li>...</li>
      <li>...</li>
      <li>...</li>
      <li>...</li>
      <li>...</li>
      <li>...</li>
      <li>...</li>
      <li>...</li>
    </ol>
  </ul>
</div>
```

document.getElementsByTagName('li');
the output will be an array like object with the length property in it.

How to convert array like to an array ?
There are three ways to do so.
1: using spread operator

> [...array_like_obj]

2: Using Array.from() method

> Array.from(array_like_obj)

3: Using for...of loop

> for(var i of array_like_obj)
> //this is just used to iterate to each elements not directly convert to array

4: Using Object.values() method

> Object.values(array_like_obj)

**_we will see all these examples one by one with example:
lets have some sample object and function that we will use in our examples._**

```javascript
//object with length property
var obj1 = {
  0: "we",
  1: "are",
  2: "capscode",
  length: 3,
};

//object without length property
var obj2 = {
  0: "we",
  1: "are",
  2: "capscode",
};

//function in which we will arguments property
function func(params) {
  console.log(arguments);
  //here we will do all our operations
  console.log(a);
  console.log(a.push("capscode"));
  console.log(a);
}
```

**1: using spread operator:**
[...array_like_obj]

> for spread operator to work on, the array_like_obj/ (any object) must have iterator i.e it must implement Symbol.iterator()

```javascript
console.log([...obj1]); //obj1 is not iterable

console.log([...obj2]); //obj1 is not iterable

function func(params) {
  console.log(arguments); //outputs below image
  var a = [...arguments];
  console.log(a); //[1, 2, 3, 4, 5, 6, 6]
  a.push("capscode");
  console.log(a); //[1, 2, 3, 4, 5, 6, 6, "capscode"]
}

func(1, 2, 3, 4, 5, 6, 6);
```

![Alt Text](https://dev-to-uploads.s3.amazonaws.com/i/w1cr1ojx040rvlqlmf0o.JPG)

**2: Array.from(array_like_obj)**

> for Array.from() to work on, the array_like_obj/ (any object) must have length property but it can or can not implements Symbol.iterator().

```javascript
var c = Array.from(obj1);
console.log(c); //["we", "are", "capscode"]
c.push("devs");
console.log(c); //["we", "are", "capscode","devs"]

var n = Array.from(obj2);
console.log(n); //[] as length property is not there

function func(params) {
  console.log(arguments); //always outputs same image above, kindly refer that.
  var a = Array.from(arguments);
  console.log(a); //[1, 2, 3, 4, 5, 6, 6]
  a.push("capscode");
  console.log(a); //[1, 2, 3, 4, 5, 6, 6, "capscode"]
}

func(1, 2, 3, 4, 5, 6, 6);
```

**3: Using for...of loop**

> for for..of to work on, the array_like_object must implements Symbol.iterator()
> The Symbol.iterator method is called automatically by for..of, but we also can do it directly.

```javascript
for (var i of obj1) {
  console.log(i); //TypeError: obj1 is not iterable
}

for (var i of obj2) {
  console.log(i); //TypeError: obj2 is not iterable
}

function func(params) {
  var realArray = [];
  for (const element of arguments) {
    realArray.push(element);
  }
  console.log(realArray); //[1, 2, 3, 4, 5, 6, 6]
}
func(1, 2, 3, 4, 5, 6, 6);
```

**4: Using Object.values() method**
Object.values():

> for Object.value to to work on, the length property or Object.iterator() is not must

```javascript
var a = Object.values(obj1);
console.log(a); //["we", "are", "capscode", 3]
a.push("devs");
console.log(a); //["we", "are", "capscode", 3, "devs"]

var b = Object.values(obj2);
console.log(b); //["we", "are", "capscode"]
b.push("devs");
console.log(b); //["we", "are", "capscode", "devs"]

function func(params) {
  //console.log(arguments) //always outputs same as the above image
  var a = Object.values(arguments);
  console.log(a); //[1, 2, 3, 4, 5, 6, 6]
  console.log(a.push("capscode"));
  console.log(a); //[1, 2, 3, 4, 5, 6, 6, "capscode"]
}

func(1, 2, 3, 4, 5, 6, 6);
```

We hope that now Array Like Object is clear to you all.
If really, Please rate us and let us know your review in the comment.

that's it my dear devs :)

we are done with What is Array Like Object, now you can implement it anywhere without any confusions.

If you like it please give a 👍

Thank you,
CapsCode
www.capscode.in
