Here are the 6 different JavaScript functions you can use to add elements to an array:

#### 1. push – Add an element to the end of the array

#### 2. unshift – Insert an element at the beginning of the array

#### 3. spread operator – Adding elements to an array using the new ES6 spread operator

#### 4. concat – This can be used to append an array to another array

#### 5. Using the arrays length property to append an element

#### 6. splice – inserts an element anywhere in an array

## Table of Content

1. The push() method
2. The unshift() method
3. The concat method
4. The spread operator (ES6)
5. Using the array length property
6. The splice method

## 1. The push() method

The `push()` method “pushes” elements to the end of the array.

Add a single element:

```js
let array = ["1", "2", "3"];
array.push("4");
console.log(array); // returns ['1', '2', '3', '4']
```

You can also add multiple elements by using multiple parameters in the push() method:

```js
let array = ["1", "2", "3"];
array.push("4", "5", "6");
console.log(array); // returns ['1', '2', '3', '4', '5', '6']
```

You can append an array to an existing array by using `push.apply()`

```js
let a = ["1", "2", "3"];
let b = ["4", "5", "6"];

a.push.apply(a, b);

console.log(a); // returns ['1', '2', '3', '4', '5', '6']
```

## 2. The unshift() method

The unshift() method inserts elements to the beginning of the array.

Inserting a single element:

```js
let array = ["1", "2", "3"];
array.unshift("0");
console.log(array); // returns ['0', '1', '2', '3']
```

Inserting multiple elements:

```js
let array = ["1", "2", "3"];
array.unshift("-1", "0");
console.log(array); // returns ['-1', '0', '1', '2', '3']
```

## 3. The concat method

The concat() method doesn’t actually append elements to an existing array but instead, creates a brand new array.

This means that the original array won’t change.

Why is this important? Here is an example:

```js
let originalArray = ["1", "2", "3"];
let appendingArray = ["4", "5", "6"];
let newArray = originalArray.concat(appendingArray);
console.log(newArray); // returns ['1', '2', '3', '4', '5', '6']
console.log(originalArray); // returns ['1', '2', '3']
```

As you can see, the original array stays the same.

You are not mutating the original array which means you are not changing it.

This can be useful if you need to use the data from the original array to other stuff.

You can also take an empty array and concat multiple arrays. We do that by adding multiple parameters in the concat method.

Here is an example:

```js
let a = ["1", "2", "3"];
let b = ["4", "5", "6"];

let result = [].concat(a, b);

console.log(result); // returns ['1', '2', '3', '4', '5', '6']
```

## 4. The spread operator (ES6)

With the ES6 syntax, we can use the spread operator. It is similar to concat where we create a new array instead of adding to the existing one.

This is a flexible way of working with arrays and very popular with the “new” JavaScript.

Let’s get started with an example:

```js
let a = ["1", "2", "3"];

let newArray = ["0", ...a, "4"];

console.log(newArray); // returns ['0', '2', '3', '4']
```

As you can see, we are placing the entire array in the middle of the new array declaration. We do this by writing three dots before the variable name. This is the ES6 syntax.

As you can imagine, we can place the array anywhere we want.

We can also use the spread operator together with the push method:

```js
let a = ["1", "2", "3"];
let b = ["4", "5"];

a.push(...b);

console.log(a); // returns ['0', '1', '2', '3', '4', '5']
```

## 5. Using the array length property

You can also append an array by using the arrays length property as an index.

```js
let a = ["1", "2", "3"];
a[a.length] = "4";

console.log(a); // returns ['1', '2', '3', '4']
```

The first element of an array has index number 0.

So in the example above, we have three elements. The elements have index 0, 1 and 2. a.length will return 3 since we have three elements.

Therefore it will append at the end of the array.

You can not insert elements in any other place using this method. If I would set a[1] = '5', it would just change the existing element.

## 6. The splice method

You can insert elements anywhere in the array using the splice method().

The splice method is used in the following way: array.splice(index, how many to delete, element 1, element 2).

The first parameter you define where in the array you want to insert data. The second parameter you define how many elements you want to delete. We only want to insert elements, so we put 0 here. The last parameters are the elements you want to insert.

```js
let a = ["1", "2", "3"];

a.splice(2, 0, "4", "5");

console.log(a); // returns ['0', '2', '4', '5', '3']
```

Thank you for reading this far. This is a brief introduction of **6 Ways to Insert Elements to an Array in JavaScript** .
If you find this article useful, like and share this article. Someone could find it useful too. If you find anything technically inaccurate please feel free to comment below.
Now you can also play around the objects in JS.

Hope its a nice and informative read for you.
VISIT https://www.capscode.in/blog TO LEARN MORE...

Thanks,\
CapsCode
