# JavaScript Amazing operators

Hello Everyone,
In this tutorial I am going to discuss about **_3 amazing operators_** that is **_very useful_** and **_time saving_** operator that most of beginner developers don't know.
The 3 operator are,

1. Nullish Coalescing Operator (??)
2. Logical Nullish Assignment (??=)
3. Optional Chaining Operator (?.)

We are going to discuss each of these operator one by one with some of the examples for better understanding.

### 1. Nullish Coalescing Operator (??)

> **syntax:**
> a??b
>
> - If **a** is defined then the output will be **a**
> - if **a** is not defined/ Nullish (**NULL or UNDEFINED**) then the output will be **b**
>
> **_In other words, Nullish Coalescing Operator(??) returns the first argument if it is NOT null or undefined. Otherwise returns second argument_**
>
> **Examples:**
>
> ```javascript
> let a = NULL;
> console.log(a ?? 50); //50
> console.log(a); //NULL
> ```
>
> ```javascript
> let a = 10;
> let c = 30;
> console.log(a ?? b ?? c ?? d); //10
> //gives output, the first defined value
> ```

### 2. Logical Nullish Assignment (??=)

> **syntax:**
> a ??= b
> the above syntax is equivalent to **a ?? (a=b)**
>
> - if **a** is **not NULLISH** (Null or Undefined), then output will be **a**
> - if **a** is **NULLISH**, then output will be **b**, and **value of b** is **assigned to a**
>
> **example:**
>
> ```javascript
> let a = NULL;
> console.log((a ??= 50)); //50
> console.log(a); //50
> //compare the output of a from the previous example.
> ```

### 3. Optional Chaining Operator (?.)

> **syntax**:
> obj **?.** prop
>
> - is similar to obj.prop if the value of obj exist,
> - otherwise, if value of obj is undefined or null it returns undefined.
>
> By using **?.** operator with object instead of using only dot (.) operator , JavaScript knows **to implicitly check** to be sure that that obj is **not** null or undefined **before attempting** to access obj.prop  
> **NOTE:** obj can be nested as well like **obj . name ?. firstname**
>
> **example:**
>
> ```javascript
> let obj = {
>   person: {
>     firstName: "John",
>     lastName: "Doe",
>   },
>
>   occupation: {
>     compony: "capscode",
>     position: "developer",
>   },
>   fullName: function () {
>     console.log(
>       "Full Name is: " + this.person.firstName + " >" + this.person.lastName
>     );
>   },
> };
> console.log(obj.person.firstName); //John
> console.log(obj.human.award); //TypeError: Cannot read property 'award' of undefined
> console.log(obj?.human.award); //TypeError: Cannot read property 'award' of undefined
> console.log(obj.human?.award); //undefined
> delete obj?.firstName; // delete obj.firstName if obj exists
> obj.fullName?.(); //logs John Doe
> obj?.fullName(); //logs John Doe
> obj.fullDetails(); // TypeError: obj.fullDetails is not a function
> obj?.fullDetails(); // TypeError: obj.fullDetails is not a function
> obj.fullDetails?.(); //undefined
> ```
>
> summing up these,
> The optional chaining `?.` syntax has three forms:
>
> 1.  `obj?.prop` – returns `obj.prop` if `obj` exists, otherwise `undefined`.
> 2.  `obj?.[prop]` – returns `obj[prop]` if `obj` exists, otherwise `undefined`.
> 3.  `obj.method?.()` – calls `obj.method()` if `obj.method` exists, otherwise returns `undefined`.

Hope you all like this and this post will be informative and helpful for you in your next project.
If you have any query or doubt, fell free to contact us.

Please visit https://www.capscode.in for more info
or
follow us on Instagram https://www.instagram.com/capscode/

### IF MY ARTICLE HELPED YOU

<a href="https://www.buymeacoffee.com/capscode" target="_blank"><img src="https://cdn.buymeacoffee.com/buttons/default-orange.png" alt="Buy Me A Coffee" height="41" width="174"></a>

Thank You,\
CapsCode
