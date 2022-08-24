Hello everyone,

In this tutorial we are going to explain all the **uses of SPREAD OPERATOR** in JavaScript.

So without wasting much time,, lets get started.
_Below are the uses:_

> - Copying an array

- Concatenating or combining arrays
- Using Math functions
- Using an array as arguments
- Adding elements in array from other array(or pushing array to an array)
- Merging object
- Copying an Object
- Converting HTMLCollections to array
- Converting string to character
- Remove duplicates from an array and create an array of unique elements

### 1. Copying an array

```javascript
var arr = [1, 2, 3, 4, 5, 6, 7];
var copy_arr = arr;
var copy_arr_spread = [...arr];

console.log(arr); //[1, 2, 3, 4, 5, 6, 7]
console.log(copy_arr); //[1, 2, 3, 4, 5, 6, 7]
console.log(copy_arr_spread); //[1, 2, 3, 4, 5, 6, 7]
arr.push(8);

console.log(arr); //[1, 2, 3, 4, 5, 6, 7, 8]
console.log(copy_arr); //[1, 2, 3, 4, 5, 6, 7, 8]
console.log(copy_arr_spread); //[1, 2, 3, 4, 5, 6, 7]
```

### 2. Concatenating or combining arrays

```javascript
var s1 = ["c", "a", "p", "s"];
var s2 = ["c", "o", "d", "e"];
var str = [...s1, ...s2];
console.log(str); //["c", "a", "p", "s", "c", "o", "d", "e"]
```

### 3. Using Math functions

##### How we ccan find min or max in array

```javascript
var find_max = [10, 20, 50, 90, 12];
console.log(Math.max(find_max)); //NaN
console.log(Math.max(...find_max)); //90
```

### 4. Using an array as arguments

```javascript
function TopThree_Skills(a, b, c) {
  console.log(`${a}, ${b}, ${c}`); //c, javascript, reatjs
}

var skills = ["c", "javascript", "reatjs", "java", "python", "sql"];
TopThree_Skills(...skills);
```

### 5. Adding elements in array from other array

```javascript
var a1 = ["c", "o", "d", "e"];
var a2 = ["c", "a", "p", "s", ...a1];
console.log(a2); //["c", "a", "p", "s", "c", "o", "d", "e"]

//some more uses - pushing array to an array
var todo = ["read", "write", "learn"];
var my_todo_list = ["code", "eat", "sleep"];

my_todo_list.push(...todo);
console.log(my_todo_list); //["code", "eat", "sleep", "read", "write", "learn"]
```

### 6. Merging object

```javascript
var obj1 = {
  fname: "John",
  lname: "Doe",
};

var obj2 = {
  comp: "capscode",
  atm_pin: "0000",
};
var obj = { ...obj1, ...obj2 };
console.log(obj); //{fname: "John", lname: "Doe", comp: "capscode", atm_pin: "0000"}
```

### 7. Copying an Object

```javascript
var person = {
  fname: "John",
  lname: "Doe",
};
var myobj_temp = person;
var myobj = { ...person };

person.phone = "1234567890";

console.log(person); //{fname: "John",lname: "Doe", phone: "1234567890"}
console.log(myobj_temp); //{fname: "John",lname: "Doe", phone: "1234567890"}
console.log(myobj); //{fname: "John",lname: "Doe",}
```

### 8. Converiting HTMLCollections to array

```javascript
var doc_arr = [...document.querySelectorAll("div")]; //try by writing this in your console
```

### 9. Converting string to character

```javascript
var comp = "capscode";
var t = [...comp];
console.log(t); // ["c", "a", "p", "s", "c", "o", "d", "e"]
console.log(...comp); //c a p s c o d e
```

### 10. Remove duplicates from an array and create an array of unique elements

```javascript
const list = [1, 3, 1, 3, 3, 2];
const unique = [...new Set(list)];
console.log(unique); //[1,3,2]
```

# if we have missed any point then let us know in the comment.

Hope this post will be helpful for you.
if you liked it, please let us know in the comment and show us your love by hitting 👍

Thank you,\
Team CapsCode
