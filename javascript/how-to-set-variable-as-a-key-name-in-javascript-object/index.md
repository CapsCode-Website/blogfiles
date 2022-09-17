Hello Devs,

In this blog you are going to learn a very important and useful concept of JavaScript which you will definitely going to use or might have used in Production application, i.e: `How to make any variable name as key of an object in JS`.

I know you might be thinking when and in which scenario you will have to use the `variable name as a key name in JS`.
Let me take your next 2 mins to explain the scenario.
Let say you have a function and that function is used to add some keys to an object.
The key name which you are going to add in that object is dynamic depending on the button click or something like this, and in the Handler function you are passing the argument which will be used as the new key name.
So how you will make that argument name as a key of an `object` ?

---

### **Solution:**

#### STEP 1:

Make an object

```javascript
let obj = {};
```

#### STEP 2:

```js
let key = "someKey";
```

#### STEP 3:

then use `[]` to set it.

```js
obj[key] = someValue; // this is same as obj.someKey=someValue
```

**but the best way and the recommended way is using spread operator `(...)`**

```js
obj = { ...obj, [key]: someValue };
```

NOTE: if you having any doubt regarding why we are using [] for setting the keys, please have a look at [DOT & BRACKET Notation in Javascript](https://www.capscode.in/blog/dot-and-bracket-notation-in-javascript)

### **Examples:**

lets assume that we have 3 buttons, and there is a `OnClickHandler function`.
On click of buttons we are calling this handler function and passing some `key` and `value` as a argument to this handler function and then we have to set this `key` and `value` in an object.

```html
<button onclick=OnClickHandler("button1", 10)>Click 1</button>
<button onclick=OnClickHandler("button2", 20)>Click 2</button>
<button onclick=OnClickHandler("button3", 30)>Click 3</button>
```

```js
let obj = {};
function OnClickHandler(key, value) {
  obj = { ...obj, [key]: value };
}

console.log(obj); // {button1:10, button2:20, button3:30}
```

#### Other scenarios where this concept is required:

1. while updating `session storage` value.
2. while updating `state` value in reactjs
3. while switching between light and dark mode in any website

Thank you for reading this far. This is a brief introduction on **How to use variable as a key name in JavaScript**.

Hope its a nice and informative read for you.
If you find this article useful, like and share this article. Someone could find it useful too.

If you find anything technically inaccurate please feel free to reach out to us.

VISIT https://www.capscode.in/blog TO LEARN MORE.

See you in my next Blog article, Take care!!

Thanks,\
CapsCode
