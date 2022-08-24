In JavaScript we can access the properties of object using dot notation(person.first_name) and bracket notation(person[first_name]).
But what's the difference between these two notations and when to use which one ?
Just stay here with me for another 20 mins and I promise you will never forget this concept.

First we will see what's the issue we will face using dot operator.

```javascript
    let person = {
    	fname:'John',
    	lname:'Doe'
    }
    person.fname // John
    person["fname"] // John

    person[fname] //ReferenceError: fname is not defined
    person."fname" //SyntaxError: Unexpected string
```

Now,

```javascript
let first_name = "fname";
person.first_name; // undefined
person[first_name]; // John
```

Why is it soooooo......
I hope you got at least 2% of clarity from this example !!

lets see one more example and clarification,
when to use dot and when not too.

```javascript
let obj = {
  cat: "meow",
  dog: "woof",
};
let dog = "cat";
console.log(obj.dog); // woof (not as expected ?)

let obj = {
  cat: "meow",
  dog: "woof",
};
let dog = "cat";
console.log(obj[dog]); // meow (the expected result)
```

In the above example,
obj.dog does not evaluate the dog property and it directly denotes the dog property of the obj object, if dog property is present then it return the value otherwise undefined.

in obj[dog], here dog is first evaluated to get the property name. Upon evaluating the value of dog i.e cat is assigned and the final result is obj["cat"] and this will return "meow"

## Why are we looking into these many comparisons ?

Sometimes when we are working in production with some API calls and with JSON data, then their might be the chance to get the key name with spaces, (& that we might don't know being a frontend developer)
then in that case we cannot access it with dot notation.
eg.

```javascript
let obj = {
	"first name" : "John"
}

obj.first name //error
obj['first name"] // John
```

## Lets see some of the important points of dot and bracket notations

**_(obj.x <---- here x is a property identifier)_**

#### To access javascript object properties using dot notation, the

- Property identifiers **can only be** alphanumeric (and `_` and `$`)
- Property identifiers **cannot start** with a number.
- Property identifiers **cannot contain** variables.
- Valid Identifier (**contain** Unicode letters, \$, \_, and digits (0-9), but may **not start** with a digit)
- do **not start** with a digit or hyphen
- **no** spaces
- do **not include** special characters except \$ and \_ (underscore)
- obj.prop_1, obj.prop\$ is correct
- obj.1prop, obj.prop name is incorrect

#### To access javascript object properties using bracket notation, the key should be

- Property identifiers **have to be** a String or a variable that references a String.
- we **can use** variables, spaces, and Strings that start with numbers
- it can be an expression
- obj["1prop"], obj["prop name"] is correct

```javascript
	let temp = "fav"
    let x=2;
    let y=3;
    let obj = {
    	[temp+"game"] : "cricket",
    	[temp] : 'coffee',
    	[x+y]: "some_value"
    }
    obj.temp //undefined
    obj[temp] //coffee
    obj.x+y //NaN
    obj.5 //syntax error
    obj[x+y] // "some value"
    obj.favgame // "cricket"
    obj[temp+"game"] // "cricket"
```

**In Simple words,**
The two most common ways to access properties in JavaScript are with a dot and with square brackets. Both `value.x and value[x]` access a property on value—but not necessarily the same property.
The difference is in how **x** is interpreted. When using a dot, the part after the dot must be a valid variable name, and it directly names the property. When using square brackets, the expression between the brackets is evaluated to get the property name. Whereas value.x fetches the property of value named “x”, value[x] tries to evaluate the expression x and uses the result as the property name.

## Lets see how to assign variable as key of an object in JavaScript

```javascript
let x = "name";
let obj = {
  x: "John",
};

console.log(obj.name); //undefined
console.log(obj.x); //John
```

Why we are getting undefined ?
because we have not assigned the variable as the key of an object in proper way.
To assign variable as key we have to use bracket notation [] as below,

```js
let obj = {
  [x]: "John",
};
console.log(obj.x); //undefined
console.log(obj.name); //John
```

## Dot Notation’s Limitation

if we take this object :

```javascript
const obj = {
  123: 'digit',
  123name: 'start with digit',
  name123: 'does not start with digit',
  $name: '$ sign',
  name-123: 'hyphen',
  NAME: 'upper case',
  name: 'lower case'
};
//source: stackoverflow
```

accessing their proprieties using dot notation

```javascript
obj.123;      // ❌ SyntaxError
obj.123name;  // ❌ SyntaxError
obj.name123;  // ✅ 'does not start with digit'
obj.$name;    // ✅  '$ sign'
obj.name-123;  // ❌ SyntaxError
obj.'name-123';// ❌ SyntaxError
obj.NAME; // ✅ 'upper case'
obj.name; // ✅ 'lower case'

```

But none of this is a problem for the Bracket Notation:

```javascript
obj["123"]; // ✅ 'digit'
obj["123name"]; // ✅ 'start with digit'
obj["name123"]; // ✅ 'does not start with digit'
obj["$name"]; // ✅ '$ sign'
obj["name-123"]; // ✅ 'does not start with digit'
obj["NAME"]; // ✅ 'upper case'
obj["name"]; // ✅ 'lower case'
```

### Some more mind blowing examples of dot and bracket notation in JS object

```javascript
let obj = {
  true: "john",
};
obj[true]; //john
obj[true]; //john
obj[!false]; //john
obj[!0]; //john
obj[1]; //undefined

let obj = {
  undefined: "john",
};
obj.undefined; //john
obj[undefined]; //john
obj[obj.x]; //john
```

Thank you for reading this far. This is a brief introduction of **Difference between accessing object properties using dot and bracket notation in JS** .
If you find this article useful, like and share this article. Someone could find it useful too. If you find anything technically inaccurate please feel free to comment below.
Now you can also play around the objects in JS.

Hope its a nice and informative read for you.
VISIT https://www.capscode.in/blog TO LEARN MORE...

### IF MY ARTICLE HELPED YOU

<a href="https://www.buymeacoffee.com/capscode" target="_blank"><img src="https://cdn.buymeacoffee.com/buttons/default-orange.png" alt="Buy Me A Coffee" height="41" width="174"></a>

Thanks,\
CapsCode
