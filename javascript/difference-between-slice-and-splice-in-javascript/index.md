## Difference between SLICE & SPLICE in JavaScript

Hello Devs,

In this article, we will discuss what's the difference between the two most important methods of Array in JavaScript (i.e Slice and Splice)

The `splice()` method

- returns the removed items in an array.

The `slice()` method

- returns the selected element(s) in an array, as a new array object.

The `splice()` method

- changes the original array but

`slice()` method

- doesn’t change the original array.

Lets see some of the simple examples to get the small clarification.

```js
let arr1 = [1, 2, 3, 4, 5];
let arr2 = [1, 2, 3, 4, 5];
arr1.splice(1, 3); //returns [2, 3, 4]
console.log(arr1); //[1, 5]

arr2.slice(1, 3); //returns [2, 3]
console.log(arr2); //[1, 2, 3, 4, 5]
```

## Lets discuss these two methods in more details.

### First we will discuss the splice method in detail.

Syntax:

```js
splice(start, deleteCount, item1, item2, ...itemN);
```

where,
**start (required)** -> where you want to start editing the array.

- if start is not provided then empty array is returned and it will not affect the original array
- If start is greater than length of array then start will set to length of an array.
- If negative then it is treated as **array.length-start** and if now the negative value will come then treat it as 0

**deleteCount(optional)** -> number of element you want to delete from **_start_** index

- if it is not provided or greater than or equal to array.length then all the element from start to end of an array is deleted.
- If `deleteCount` is `0` or negative, no elements will be deleted.

- **item1, item2...itemN(optional)** ->The elements to add to the array, beginning from **_start_**.
- If you do not specify any elements, `splice()` will only remove elements from the array.

lets see some of examples.

```js
let a = [1, 2, 3, 4, 5];
a.splice(); //[]
console.log(a); // [1,2,3,4,5]

let a = [1, 2, 3, 4, 5];
a.splice(2); //returns [3,4,5]
console.log(a); //[1,2]

let a = [1, 2, 3, 4, 5];
a.splice(-3); //returns [3,4,5], here start is treated as array.length-start
console.log(a); //[1,2]

let a = [1, 2, 3, 4, 5];
a.splice(-7); //returns [1,2,3,4,5], here start is treated as array.length-start and this is ngative so start will now be treated as 0
console.log(a); //[]
//(an empty array)

let a = [1, 2, 3, 4, 5];
a.splice(2, 9); //returns [3,4,5]
console.log(a); //[1,2]

let a = [1, 2, 3, 4, 5];
a.splice(2, 2, "a", "b", "c", "d"); //returns [3, 4]
console.log(a); //[1, 2, "a", "b", "c", "d", 5]
//slice has removed 2 elements starting from index '2' and added the item1, item2, ...itemN at start positon

//This also very useful when you want to delete a specific element from an array
let arr =[1,3,6,4]
//we want to remove 3 from array
const index = arr.indexOf(3) //returns 1
//NOTE: indexOf returns -1 if element is not present in an array and it returns the index of 1st occurrence of that element and its case-sensitive (useful when we are searching a word in string)
if(index > -1){
  arr.splice(index, 1)
}
console.log(arr) // [1,6,4]
```

### Now lets discuss the slice method.

This method just extract the a part from an array.

Syntax:

```js
slice(start, end);
```

where,
**start(required)** -> starting index from where to start the extraction from an array.

- if the value of start is negative then it is treated as arr.length-1
- if `start` is undefined, `slice` starts from the index `0`.
- if start is greater than length of an array, then an empty array is returned.

**end (optional)**-> denotes till which index (excluding) you want to extract from the start,

- If `end` is omitted, then its treated as array.length
- If end is negative then it is treated as array.length-end
- If end is non-negative & less than start, then empty array is returned
- If end is greater than length of an array, then it is treated as array.length

Lets see some of the examples,

```js
let arr = [1, 2, 3, 4, 5];
arr.slice(); //returns [1,2,3,4,5]
arr.slice(2); //returns [3,4,5]
console.log(arr); //[1,2,3,4,5]

arr.slice(2, 1); //returns []
console.log(arr); //[1,2,3,4,5]

arr.slice(2, -1); //returns [3,4], here end is treated as arr.length-1 which is 4 i.e arr.slice(2,4)
console.log(arr); //[1,2,3,4,5]

arr.slice(2, 9); //[3,4,5]
console.log(arr); //[1,2,3,4,5]
```

Using slice we can also convert an array like objects to an array ?
Syntax:

```
Array.prototype.slice.call(arguments)
```

example,

```js
let array_like_obj = {
  0: "john",
  1: "doe",
  2: "capscode",
  length: 3,
};
console.log(Array.prototype.slice.call(array_like_obj));
//["john", "doe", "capscode"]
```

Thank you for reading this far. This is a brief introduction of **Difference between SLICE & SPLICE method on Array in JS** .
If you find this article useful, like and share this article. Someone could find it useful too. If you find anything technically inaccurate please feel free to comment below.
Now you can also play around the objects in JS.

Hope its a nice and informative read for you.
VISIT https://www.capscode.in/blog TO LEARN MORE...

### IF MY ARTICLE HELPED YOU

<a href="https://www.buymeacoffee.com/capscode" target="_blank"><img src="https://cdn.buymeacoffee.com/buttons/default-orange.png" alt="Buy Me A Coffee" height="41" width="174"></a>

Thanks,\
CapsCode
