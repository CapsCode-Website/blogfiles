Hi Devs,

In this article, I will introduce you to find() method of JavaScript Array.

## Table of content

1. [Introduction](#introduction)
    
2. [When find() is useful](#when-find-is-useful)
    
3. [Points to be noted](#points-to-be-noted)
    
4. [Conclusion](#conclusion)
    

## Introduction <a name="introduction"></a>
---
The JavaScript array find() method returns the value from an array that satisfies the condition written in the callback function.

Syntax,

```javascript
arr.find(callbackFunction)

let callbackFunction = (elem, index, arr)=>{
    console.log(elem)
    console.log(index)
    console.log(arr)
}

//OR

arr.find((elem, index, arr)=>{
    console.log(elem)
    console.log(index)
    console.log(arr)
})
```

callbackFunction will be called for each element of an array arr. where,

> elem -- current element of an array arr for which the callback function is currently executing.  
> index -- current index of an array element for which the callback function is currently executing.  
> arr -- the whole array for which the find() method is called upon.

let me explain this with a simple example.

*Example 1*

```javascript
const arr = [1,12,3,100,21,0] 
let result = arr.find((elem)=>{ return elem > 3 })
console.log(result) //12 
```

*Example 2*

```javascript
const arr = [1,12,3,100,21,0] 
let result = arr.find((elem)=>{ return elem == 30 })
console.log(result) //undefined 
```

The output returned by `find()` method in the above example will be `12`.

What have we observed from the above example? This callback function gets executed for each element and `find()` method returns the **first value** which satisfies the condition written in the callback function. If no values satisfy the condition written in the callback function, `undefined` will be returned.

Once `find()` returned something, then the execution of the callback function stopped at that point (so from the above example 1, it won't execute the loop after index 1).

## When find() is useful <a name="when-find-is-useful"></a>
---

let's say we have a big JSON data, and you have a search functionality & you want to filter out the first appearance of that search.

```javascript
var data=[ {country_name:"India",code:"IN"}, {country_name:"United States",code:"US"}, {country_name:"United Kingdom",code:"UK"}, {country_name:"India",code:"IN"}];
//assume someone searched for India 
let result = data.find(d=>d.country_name=="India")
//output will be 
console.log(result) // {country_name: 'India', code: 'IN'} 
```

But using find() you will get the output of the first appearance of India which is at index 0 and not the one which is at index 3,

So, if you want to get all the values that satisfy the condition, you better use the filter() method instead of find(). Make sure that filter() will return an array if the condition is satisfied.

```js
 var data=[
    {country_name:"India",code:"IN"},
    {country_name:"United States",code:"US"},
    {country_name:"United Kingdom",code:"UK"},
    {country_name:"India",code:"IN"}];

//assume someone searched for India
let result = data.filter(d=>d.country_name=="India")

//output will be
console.log(result) // [{country_name: 'India', code: 'IN'},{country_name:"India",code:"IN"}]
```

## Some more points to be noted <a name="points-to-be-noted"></a>
---

find() method does not mutate (or change) the array on which it is called upon. But the function provided to callbackFunction can. If so, the elements processed by find are set before the first invocation of callbackFn. Therefore:

1.callbackFn will not visit any of the elements in arr added to the array arr after the call to `find()` begins.
    
```javascript
let arr = [1,2,5,4,3,6,7,8,9]
let op = arr.find(e=>{ arr.length=0 return e==1; })
console.log(op) //undefined
 ```
    
2.Elements that are assigned to indexes already visited of an array arr, or to indexes outside the range of an array arr, will not be visited by callbackFunction.

```javascript
let arr = [1,2,5,4,3,6,7,8,9]
let op = arr.find((e, index)=>{ 
if(index==2) { 
	arr[0]=10 } 
	return e == 10;
}) 
console.log(op) //undefined 
```
    
3.If an existing, unvisited element of the array arr is changed by callbackFunction, its value passed to the callbackFunction will be the value at the time `find()` visits that element's index.
    
```javascript
let arr = [1,2,5,4,3,6,7,8,9]
let op = arr.find(e=>{ 
	arr[8]=90 
	return e == 90; 
}) 
console.log(op) //90
```
    
4.Elements that are deleted **using the delete operator** from an array arr are still **visited.**
    

```javascript
let arr = [1, 2, 3, 4, 5, 6, 7, 8, 9]
let op = arr.find((e,i,a)=>{ 
    console.log(e) 
    console.log(i) 
    console.log(a)
    if(i==0){ 
        delete myarr[2] 
        console.log(arr) // [1, 2, empty, 5, 6, 7, 8, 9] }
        return e == 3 
    }) 
console.log(op) // undefined 
```

Here, after deleting the element at index 2 using the delete operator, we can see that the index 3 value will become empty and while iterating over an array arr index 3 will still be visited and will print

```javascript
console.log(e) //undefined 
console.log(i) //2 
console.log(a) //[1, 2, empty, 5, 6, 7, 8, 9]
```

and hence there is none of the element with value 3 the line console.log(op) will print `undefined`

Let's see a few more methods of Array methods of JavaScript which work a bit similarly to that of `find()` method,

1. some() 
2. every()
    

The syntax of both of these are same as `find()` but, some and every return boolean values based on the condition of the callback function

1. some(): iterates over all the array elements and check for the condition, if **any elements satisfy** the condition of the callback function then `some()` will return true else it will return false.
    
2. every() iterates over all the array elements and checks for the condition, if **all the elements satisfy** the condition of the callback function then `every()` will return true else it will return false.
    

## Conclusion <a name="conclusion"></a>
---

Thank you for reading this far. This is a brief introduction to How the array find(**) method works in JavaScript**. `find()` method is useful when we want to return the first appearance of an element in an array or JSON data based on the condition written in the callback function.

Hope it's a nice and informative read for you. If you find this article useful, like and share this article. Someone could find it useful too.

If you find anything technically inaccurate, please feel free to reach out to us.

VISIT [https://www.capscode.in/blog](https://www.capscode.in/blog) TO LEARN MORE.

See you in my next Blog article, Take care!!

Thanks, \
CapsCode