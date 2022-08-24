Hello Devs,

In this article i will walk you through one of the important methods of Array in JavaScript i.e Array.flat method.

>

## Table of content

1. [Theory](#theory)
2. [Syntax](#syntax)
3. [Return Value](#return)
4. [Examples](#example)

So without wasting any time lets get into the article

## Theory <a name="theory"></a>

**The flat() method is used to flatten the array of arrays. The process of flatten depends on the depth we want to flattened the array of arrays.**

What this method do is, it takes out the array element from an array of arrays and concat them in the main array.
it will repeat this process till the depth value.

## Syntax <a name="syntax"></a>

```js
Syntax: flat(depth);
// The depth level specifying how deep a nested array structure should be flattened.
// Defaults to 1.
```

## Return Value <a name="return"></a>

```js
return value:
A new array with the sub-array elements concatenated into it.
```

## Examples <a name="example"></a>

**NOTE**: IF YOU WANT TO FLATTEN THE ARRAY UPTO ITS LAST DEPTH THEN PUT `depth` AS `Infinity`

```js
example:
let arr = [1, 2, [3, 4, [5, 6]]];

arr.flat(0) // [1, 2, [3, 4, [5, 6]]];
arr.flat(1) // [1, 2, 3, 4, [5, 6]]
arr.flat(2) // [1, 2, 3, 4, 5, 6]
arr.flat(3) // [1, 2, 3, 4, 5, 6]
arr.flat( ) // [1, 2, 3, 4, [5, 6]]
// if no depth is provided then it will take the default value i.e 1.
arr.flat(Infinity) //[1, 2, 3, 4, 5, 6]


arr.flat(0).length //3
arr.flat(1).length //5
arr.flat(2).length //6

```

Thank you for reading this far. This is a brief introduction of **Array.flat() method in JavaScript** .
If you find this article useful, like and share this article. Someone could find it useful too. If you find anything technically inaccurate please feel free to comment below.

Hope its a nice and informative read for you.
VISIT https://www.capscode.in/blog TO LEARN MORE...
See you in my next Blog article, Take care!!

### IF MY ARTICLE HELPED YOU

<a href="https://www.buymeacoffee.com/capscode" target="_blank"><img src="https://cdn.buymeacoffee.com/buttons/default-orange.png" alt="Buy Me A Coffee" height="41" width="174"></a>

Thanks,\
CapsCode
