# 70 JavaScript Interview Questions {.fs-3xl .m:fs-4xl .l:fs-5xl .fw-bold .s:fw-heavy .lh-tight .mb-4 .medium}

## [](#hi-guys-good-day-and-a-happy-new-year-fireworksfireworksfireworks) Hi Guys Good Day and a Happy New Year 🎆🎆🎆!

This is a long one, so bear with me for a second or an hour. In every
answer for every question there's an arrow up **↑** link that lets you
go back to the List of Questions so that you don't waste time scrolling
up and down.

### [](#the-questions) The Questions

- [~1.\\ What's\\ the\\ difference\\ between\\ `undefined`\\ and\\ `null`?~](#1-whats-the-difference-between-undefined-and-null)
- [~2.\\ What\\ does\\ the\\ &&\\ operator\\ do?~](#2-what-does-the-ampamp-operator-do)
- [~3.\\ What\\ does\\ the\\ ||\\ operator\\ do?~](#3-what-does-the-operator-do)
- [~4.\\ Is\\ using\\ the\\ +\\ or\\ unary\\ plus\\ operator\\ the\\ fastest\\ way\\ in\\ converting\\ a\\ string\\ to\\ a\\ number?~](#4-is-using-the-or-unary-plus-operator-the-fastest-way-in-converting-a-string-to-a-number)
- [~5.\\ What\\ is\\ the\\ DOM?~](#5-what-is-the-dom)
- [~6.\\ What\\ is\\ Event\\ Propagation?~](#6-what-is-event-propagation)
- [~7.\\ What's\\ Event\\ Bubbling?~](#7-whats-event-bubbling)
- [~8.\\ What's\\ Event\\ Capturing?~](#8-whats-event-capturing)
- [~9.\\ What's\\ the\\ difference\\ between\\ `event.preventDefault()`\\ and\\ `event.stopPropagation()`\\ methods?~](#9-whats-the-difference-between-eventpreventdefault-and-eventstoppropagation-methods)
- [~10.\\ How\\ to\\ know\\ if\\ the\\ `event.preventDefault()`\\ method\\ was\\ used\\ in\\ an\\ element?~](#10-how-to-know-if-the-eventpreventdefault-method-was-used-in-an-element)
- [~11.\\ Why\\ does\\ this\\ code\\ obj.someprop.x\\ throw\\ an\\ error?~](#11-why-does-this-code-objsomepropx-throw-an-error)
- [~12.\\ What\\ is\\ event.target\\ ?~](#12-what-is-eventtarget-)
- [~13.\\ What\\ is\\ event.currentTarget?~](#13-what-is-eventcurrenttarget)
- [~14.\\ What's\\ the\\ difference\\ between\\ `==`\\ and\\ `===`?~](#14-whats-the-difference-between-and-)
- [~15.\\ Why\\ does\\ it\\ return\\ false\\ when\\ comparing\\ two\\ similar\\ objects\\ in\\ JavaScript?~](#15-why-does-it-return-false-when-comparing-two-similar-objects-in-javascript)
- [~16.\\ What\\ does\\ the\\ `!!`\\ operator\\ do?~](#16-what-does-the-operator-do)
- [~17.\\ How\\ to\\ evaluate\\ multiple\\ expressions\\ in\\ one\\ line?~](#17-how-to-evaluate-multiple-expressions-in-one-line)
- [~18.\\ What\\ is\\ Hoisting?~](#18-what-is-hoisting)
- [~19.\\ What\\ is\\ Scope?~](#19-what-is-scope)
- [~20.\\ What\\ are\\ Closures?~](#20-what-are-closures)
- [~21.\\ What\\ are\\ the\\ falsy\\ values\\ in\\ JavaScript?~](#21-what-are-the-falsy-values-in-javascript)
- [~22.\\ How\\ to\\ check\\ if\\ a\\ value\\ is\\ falsy?~](#22-how-to-check-if-a-value-is-falsy)
- [~23.\\ What\\ does\\ `"use strict"`\\ do?~](#23-what-does-use-strict-do)
- [~24.\\ What's\\ the\\ value\\ of\\ `this`\\ in\\ JavaScript?~](#24-whats-the-value-of-this-in-javascript)
- [~25.\\ What\\ is\\ the\\ `prototype`\\ of\\ an\\ object?~](#25-what-is-the-prototype-of-an-object)
- [~26.\\ What\\ is\\ an\\ IIFE,\\ what\\ is\\ the\\ use\\ of\\ it?~](#26-what-is-an-iife-what-is-the-use-of-it)
- [~27.\\ What\\ is\\ the\\ use\\ `Function.prototype.apply`\\ method?~](#27-what-is-the-use-functionprototypeapply-method)
- [~28.\\ What\\ is\\ the\\ use\\ `Function.prototype.call`\\ method?~](#28-what-is-the-use-functionprototypecall-method)
- [~29.\\ What's\\ the\\ difference\\ between\\ `Function.prototype.apply`\\ and\\ `Function.prototype.call`?~](#29-whats-the-difference-between-functionprototypeapply-and-functionprototypecall)
- [~30.\\ What\\ is\\ the\\ usage\\ of\\ `Function.prototype.bind`?~](#30-what-is-the-usage-of-functionprototypebind)
- [~31.\\ What\\ is\\ Functional\\ Programming\\ and\\ what\\ are\\ the\\ features\\ of\\ JavaScript\\ that\\ makes\\ it\\ a\\ candidate\\ as\\ a\\ functional\\ language?~](#31-what-is-functional-programming-and-what-are-the-features-of-javascript-that-makes-it-a-candidate-as-a-functional-language)
- [~32.\\ What\\ are\\ Higher\\ Order\\ Functions?~](#32-what-are-higher-order-functions)
- [~33.\\ Why\\ are\\ functions\\ called\\ First-class\\ Objects?~](#33-why-are-functions-called-firstclass-objects)
- [~34.\\ Implement\\ the\\ `Array.prototype.map`\\ method\\ by\\ hand.~](#34-implement-the-arrayprototypemap-method-by-hand)
- [~35.\\ Implement\\ the\\ `Array.prototype.filter`\\ method\\ by\\ hand.~](#35-implement-the-arrayprototypefilter-method-by-hand)
- [~36.\\ Implement\\ the\\ `Array.prototype.reduce`\\ method\\ by\\ hand.~](#36-implement-the-arrayprototypereduce-method-by-hand)
- [~37.\\ What\\ is\\ the\\ `arguments`\\ object?~](#37-what-is-the-arguments-object)
- [~38.\\ How\\ to\\ create\\ an\\ object\\ without\\ a\\ **prototype**?~](#38-how-to-create-an-object-without-a-prototype)
- [~39.\\ Why\\ does\\ `b`\\ in\\ this\\ code\\ become\\ a\\ global\\ variable\\ when\\ you\\ call\\ this\\ function?~](#39-why-does-b-in-this-code-become-a-global-variable-when-you-call-this-function)
- [~40.\\ What\\ is\\ **ECMAScript**?~](#40-what-is-ecmascript)
- [~41.\\ What\\ are\\ the\\ new\\ features\\ in\\ **ES6**\\ or\\ **ECMAScript\\ 2015**?~](#41-what-are-the-new-features-in-es6-or-ecmascript-2015)
- [~42.\\ What's\\ the\\ difference\\ between\\ `var`,\\ `let`\\ and\\ `const`\\ keywords?~](#42-whats-the-difference-between-var-let-and-const-keywords)
- [~43.\\ What\\ are\\ **Arrow\\ functions**?~](#43-what-are-arrow-functions)
- [~44.\\ What\\ are\\ **Classes**?~](#44-what-are-classes)
- [~45.\\ What\\ are\\ **Template\\ Literals**?~](#45-what-are-template-literals)
- [~46.\\ What\\ is\\ **Object\\ Destructuring**?~](#46-what-is-object-destructuring)
- [~47.\\ What\\ are\\ `ES6 Modules`?~](#47-what-are-es6-modules)
- [~48.\\ What\\ is\\ the\\ `Set`\\ object\\ and\\ how\\ does\\ it\\ work?~](#48-what-is-the-set-object-and-how-does-it-work)
- [~49.\\ What\\ is\\ a\\ Callback\\ function?~](#49-what-is-a-callback-function)
- [~50.\\ What\\ are\\ **Promises**?~](#50-what-are-promises)
- [~51.\\ What\\ is\\ _async/await_\\ and\\ How\\ does\\ it\\ work?~](#51-what-is-asyncawait-and-how-does-it-work)
- [~52.\\ What's\\ the\\ difference\\ between\\ **Spread\\ operator**\\ and\\ **Rest\\ operator**?~](#52-whats-the-difference-between-spread-operator-and-rest-operator)
- [~53.\\ What\\ are\\ **Default\\ Parameters**?~](#53-what-are-default-parameters)
- [~54.\\ What\\ are\\ **Wrapper\\ Objects**?~](#54-what-are-wrapper-objects)
- [~55.\\ What\\ is\\ the\\ difference\\ between\\ **Implicit**\\ and\\ **Explicit**\\ Coercion?~](#55-what-is-the-difference-between-implicit-and-explicit-coercion)
- [~56.\\ What\\ is\\ `NaN`?\\ and\\ How\\ to\\ check\\ if\\ a\\ value\\ is\\ `NaN`?~](#56-what-is-nan-and-how-to-check-if-a-value-is-nan)
- [~57.\\ How\\ to\\ check\\ if\\ a\\ value\\ is\\ an\\ **Array**?~](#57-how-to-check-if-a-value-is-an-array)
- [~58.\\ How\\ to\\ check\\ if\\ a\\ number\\ is\\ even\\ without\\ using\\ the\\ `%`\\ or\\ modulo\\ operator?~](#58-how-to-check-if-a-number-is-even-without-using-the-or-modulo-operator)
- [~59.\\ How\\ to\\ check\\ if\\ a\\ certain\\ property\\ exists\\ in\\ an\\ object?~](#59-how-to-check-if-a-certain-property-exists-in-an-object)
- [~60.\\ What\\ is\\ **AJAX**?~](#60-what-is-ajax)
- [~61.\\ What\\ are\\ the\\ ways\\ of\\ making\\ objects\\ in\\ JavaScript?~](#61-what-are-the-ways-of-making-objects-in-javascript)
- [~62.\\ What's\\ the\\ difference\\ between\\ `Object.seal`\\ and\\ `Object.freeze`\\ methods?~](#62-whats-the-difference-between-objectseal-and-objectfreeze-methods)
- [~63.\\ What's\\ the\\ difference\\ between\\ the\\ `in`\\ operator\\ and\\ the\\ `hasOwnProperty`\\ method\\ in\\ objects?~](#63-whats-the-difference-between-the-in-operator-and-the-hasownproperty-method-in-objects)
- [~64.\\ What\\ are\\ the\\ ways\\ to\\ deal\\ with\\ **Asynchronous\\ Code**\\ in\\ JavasScript?~](#64-what-are-the-ways-to-deal-with-asynchronous-code-in-javasscript)
- [~65.\\ What's\\ the\\ difference\\ between\\ a\\ **function\\ expression**\\ and\\ **function\\ declaration**?~](#65-whats-the-difference-between-a-function-expression-and-function-declaration)
- [~66.\\ How\\ many\\ ways\\ can\\ a\\ function\\ be\\ _invoked_?~](#66-how-many-ways-can-a-function-be-invoked)
- [~67.\\ What\\ is\\ _memoization_\\ and\\ what's\\ the\\ use\\ it?~](#67-what-is-memoization-and-whats-the-use-it)
- [~68.\\ Implement\\ a\\ memoization\\ helper\\ function.~](#68-implement-a-memoization-helper-function)
- [~69.\\ Why\\ does\\ `typeof null`\\ return\\ `object`?\\ How\\ to\\ check\\ if\\ a\\ value\\ is\\ `null`?~](#69-why-does-typeof-null-return-object-how-to-check-if-a-value-is-null)
- [~70.\\ What\\ does\\ the\\ `new`\\ keyword\\ do?~](#70-what-does-the-new-keyword-do)

### [](#1-whats-the-difference-between-undefined-and-null) 1. What's the difference between `undefined` and `null`?.

[↑](#the-questions) Before understanding the differences between
`undefined` and `null` we must understand the similarities between them.

- They belong to **JavaScript's** 7 primitive types.

```{.highlight .javascript}
 let primitiveTypes = ['string','number','null','undefined','boolean','symbol', 'bigint'];
```

Enter fullscreen mode

Exit fullscreen mode

- They are **falsy** values. Values that evaluated to false when
  converting it to boolean using `Boolean(value)` or `!!value`.

```{.highlight .javascript}
   console.log(!!null); //logs false
   console.log(!!undefined); //logs false

   console.log(Boolean(null)); //logs false
   console.log(Boolean(undefined)); //logs false
```

Enter fullscreen mode

Exit fullscreen mode

Ok, let's talk about the differences.

- `undefined` is the default value of a variable that has not been
  assigned a specific value. Or a function that has no **explicit**
  return value ex. `console.log(1)`. Or a property that does not exist
  in an object. The JavaScript engine does this for us the
  **assigning** of `undefined` value.

```{.highlight .javascript}
  let _thisIsUndefined;
  const doNothing = () => {};
  const someObj = {
    a : "ay",
    b : "bee",
    c : "si"
  };

  console.log(_thisIsUndefined); //logs undefined
  console.log(doNothing()); //logs undefined
  console.log(someObj["d"]); //logs undefined
```

Enter fullscreen mode

Exit fullscreen mode

- `null` is **"a value that represents no value"**. `null` is value
  that has been **explicitly** defined to a variable. In this example
  we get a value of `null` when the `fs.readFile` method does not
  throw an error.

```{.highlight .javascript}
  fs.readFile('path/to/file', (e,data) => {
     console.log(e); //it logs null when no error occurred
     if(e){
       console.log(e);
     }
     console.log(data);
   });
```

Enter fullscreen mode

Exit fullscreen mode

When comparing `null` and `undefined` we get `true` when using `==` and
`false` when using `===`. You can read the reason
[here](#14-whats-the-difference-between-and-).\

```{.highlight .javascript}
   console.log(null == undefined); // logs true
   console.log(null === undefined); // logs false
```

Enter fullscreen mode

Exit fullscreen mode

### [](#2-what-does-the-ampamp-operator-do) 2. What does the `&&` operator do?

[↑](#the-questions) The `&&` or **Logical AND** operator finds the first
_falsy_ expression in its operands and returns it and if it does not
find any _falsy_ expression it returns the last expression. It employs
short-circuiting to prevent unnecessary work. I've used this in the
`catch` block when closing database connection in one of my projects.\

```{.highlight .javascript}
   console.log(false && 1 && []); //logs false
   console.log(" " && true && 5); //logs 5
```

Enter fullscreen mode

Exit fullscreen mode

Using **if** statements.\

```{.highlight .javascript}
  const router: Router = Router();

  router.get('/endpoint', (req: Request, res: Response) => {
     let conMobile: PoolConnection;
     try {
        //do some db operations
     } catch (e) {
     if (conMobile) {
      conMobile.release();
     }
  }
});
```

Enter fullscreen mode

Exit fullscreen mode

Using **&&** operator.\

```{.highlight .javascript}
const router: Router = Router();

router.get('/endpoint', (req: Request, res: Response) => {
  let conMobile: PoolConnection;
  try {
     //do some db operations
  } catch (e) {
    conMobile && conMobile.release()
  }
});
```

Enter fullscreen mode

Exit fullscreen mode

### [](#3-what-does-the-operator-do) 3. What does the `||` operator do?

[↑](#the-questions) The `||` or **Logical OR** operator finds the first
_truthy_ expression in its operands and returns it. This too employs
short-circuiting to prevent unnecessary work. It was used before to
initialize default parameter values IN functions before **ES6 Default
function parameters** was supported.\

```{.highlight .javascript}
console.log(null || 1 || undefined); //logs 1

function logName(name) {
  var n = name || "Mark";
  console.log(n);
}

logName(); //logs "Mark"
```

Enter fullscreen mode

Exit fullscreen mode

### [](#4-is-using-the-or-unary-plus-operator-the-fastest-way-in-converting-a-string-to-a-number) 4. Is using the **+** or unary plus operator the fastest way in converting a string to a number?

[↑](#the-questions) According to [MDN
Documentation](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Operators/Arithmetic_Operators#Unary_plus)
the `+` is the fastest way of converting a string to a number because it
does not perform any operations on the value if it is already a number.

### [](#5-what-is-the-dom) 5. What is the **DOM**?

[↑](#the-questions) **DOM** stands for **Document Object Model** is an
interface (**API**) for HTML and XML documents. When the browser first
reads (_parses_) our HTML document it creates a big object, a really big
object based on the HTML document this is the **DOM**. It is a tree-like
structure that is modeled from the HTML document. The **DOM** is used
for interacting and modifying the **DOM structure** or specific Elements
or Nodes.

Imagine if we have an HTML structure like this.\

```{.highlight .html}
<!DOCTYPE html>
<html lang="en">

<head>
   <meta charset="UTF-8">
   <meta name="viewport" content="width=device-width, initial-scale=1.0">
   <meta http-equiv="X-UA-Compatible" content="ie=edge">
   <title>Document Object Model</title>
</head>

<body>
   <div>
      <p>
         <span></span>
      </p>
      <label></label>
      <input>
   </div>
</body>

</html>
```

Enter fullscreen mode

Exit fullscreen mode

The **DOM** equivalent would be like this.\
 [![DOM
equivalent](https://res.cloudinary.com/practicaldev/image/fetch/s--z_mRQj0_--/c_limit%2Cf_auto%2Cfl_progressive%2Cq_auto%2Cw_880/https://thepracticaldev.s3.amazonaws.com/i/mbqphfbjfie45ynj0teo.png)](https://res.cloudinary.com/practicaldev/image/fetch/s--z_mRQj0_--/c_limit%2Cf_auto%2Cfl_progressive%2Cq_auto%2Cw_880/https://thepracticaldev.s3.amazonaws.com/i/mbqphfbjfie45ynj0teo.png)

The `document` object in **JavaScript** represents the **DOM**. It
provides us many methods that we can use to selecting elements to update
element contents and many more.

### [](#6-what-is-event-propagation) 6. What is **Event Propagation**?

[↑](#the-questions) When an **event** occurs on a **DOM** element, that
**event** does not entirely occur on that just one element. In the
**Bubbling Phase**, the **event** bubbles up or it goes to its parent,
to its grandparents, to its grandparent's parent until it reaches all
the way to the `window` while in the **Capturing Phase** the event
starts from the `window` down to the element that triggered the event or
the `event.target`.

**Event Propagation** has **three** phases.

1.  [Capturing Phase](#8-whats-event-capturing) – the event starts from
    `window` then goes down to every element until it reaches the target
    element.
2.  [Target Phase](#12-what-is-eventtarget-) – the event has reached the
    target element.
3.  [Bubbling Phase](#7-whats-event-bubbling) – the event bubbles up
    from the target element then goes up every element until it reaches
    the `window`.

[![Event
Propagation](https://res.cloudinary.com/practicaldev/image/fetch/s--Azk8KRbD--/c_limit%2Cf_auto%2Cfl_progressive%2Cq_auto%2Cw_880/https://thepracticaldev.s3.amazonaws.com/i/hjayqa99iejfhbsujlqd.png)](https://res.cloudinary.com/practicaldev/image/fetch/s--Azk8KRbD--/c_limit%2Cf_auto%2Cfl_progressive%2Cq_auto%2Cw_880/https://thepracticaldev.s3.amazonaws.com/i/hjayqa99iejfhbsujlqd.png)

### [](#7-whats-event-bubbling) 7. What's **Event Bubbling**?

[↑](#the-questions) When an **event** occurs on a **DOM** element, that
**event** does not entirely occur on that just one element. In the
**Bubbling Phase**, the **event** bubbles up or it goes to its parent,
to its grandparents, to its grandparent's parent until it reaches all
the way to the `window`.

If we have an example markup like this.\

```{.highlight .html}
 <div class="grandparent">
    <div class="parent">
      <div class="child">1</div>
    </div>
  </div>
```

Enter fullscreen mode

Exit fullscreen mode

And our js code.\

```{.highlight .javascript}
function addEvent(el, event, callback, isCapture = false) {
  if (!el || !event || !callback || typeof callback !== 'function') return;
  if (typeof el === 'string') {
    el = document.querySelector(el);
  };
  el.addEventListener(event, callback, isCapture);
}

addEvent(document, 'DOMContentLoaded', () => {
  const child = document.querySelector('.child');
  const parent = document.querySelector('.parent');
  const grandparent = document.querySelector('.grandparent');

  addEvent(child, 'click', function (e) {
    console.log('child');
  });

  addEvent(parent, 'click', function (e) {
    console.log('parent');
  });

  addEvent(grandparent, 'click', function (e) {
    console.log('grandparent');
  });

  addEvent(document, 'click', function (e) {
    console.log('document');
  });

  addEvent('html', 'click', function (e) {
    console.log('html');
  })

  addEvent(window, 'click', function (e) {
    console.log('window');
  })

});
```

Enter fullscreen mode

Exit fullscreen mode

The `addEventListener` method has a third optional parameter
**useCapture** with a default value of `false` the event will occur in
the **Bubbling phase** if `true` the event will occur in the **Capturing
Phase**. If we click on the `child` element it logs
`child`,`parent`,`grandparent`, `html`, `document` and `window`
respectively on the **console**. This is **Event Bubbling**.

### [](#8-whats-event-capturing) 8. What's **Event Capturing**?

[↑](#the-questions) When an **event** occurs on a **DOM** element, that
**event** does not entirely occur on that just one element. In
**Capturing Phase**, the event starts from the `window` all the way down
to the element that triggered the event.

If we have an example markup like this.\

```{.highlight .html}
 <div class="grandparent">
    <div class="parent">
      <div class="child">1</div>
    </div>
  </div>
```

Enter fullscreen mode

Exit fullscreen mode

And our js code.\

```{.highlight .javascript}
function addEvent(el, event, callback, isCapture = false) {
  if (!el || !event || !callback || typeof callback !== 'function') return;
  if (typeof el === 'string') {
    el = document.querySelector(el);
  };
  el.addEventListener(event, callback, isCapture);
}

addEvent(document, 'DOMContentLoaded', () => {
  const child = document.querySelector('.child');
  const parent = document.querySelector('.parent');
  const grandparent = document.querySelector('.grandparent');

  addEvent(child, 'click', function (e) {
    console.log('child');
  }, true);

  addEvent(parent, 'click', function (e) {
    console.log('parent');
  }, true);

  addEvent(grandparent, 'click', function (e) {
    console.log('grandparent');
  }, true);

  addEvent(document, 'click', function (e) {
    console.log('document');
  }, true);

  addEvent('html', 'click', function (e) {
    console.log('html');
  }, true)

  addEvent(window, 'click', function (e) {
    console.log('window');
  }, true)

});
```

Enter fullscreen mode

Exit fullscreen mode

The `addEventListener` method has a third optional parameter
**useCapture** with a default value of `false` the event will occur in
the **Bubbling phase** if `true` the event will occur in the **Capturing
Phase**. If we click on the `child` element it logs
`window`,`document`,`html`, `grandparent` and `parent` and `child`
respectively on the **console**. This is **Event Capturing**.

### [](#9-whats-the-difference-between-eventpreventdefault-and-eventstoppropagation-methods) 9. What's the difference between `event.preventDefault()` and `event.stopPropagation()` methods?

[↑](#the-questions) The `event.preventDefault()` method **prevents** the
default behavior of an element. If used in a `form` element it
**prevents** it from submitting. If used in an `anchor` element it
**prevents** it from navigating. If used in a `contextmenu` it
**prevents** it from showing or displaying. While the
`event.stopPropagation()` method stops the propogation of an event or it
stops the event from occurring in the
[bubbling](#7-whats-event-bubbling) or
[capturing](#8-whats-event-capturing) phase.

### [](#10-how-to-know-if-the-eventpreventdefault-method-was-used-in-an-element) 10. How to know if the `event.preventDefault()` method was used in an element?

[↑](#the-questions) We can use the `event.defaultPrevented` property in
the event object. It returns a `boolean` indicating if the
`event.preventDefault()` was called in a particular element.

### [](#11-why-does-this-code-objsomepropx-throw-an-error) 11. Why does this code `obj.someprop.x` throw an error?

```{.highlight .javascript}
const obj = {};
console.log(obj.someprop.x);
```

Enter fullscreen mode

Exit fullscreen mode

[↑](#the-questions)Obviously, this throws an error due to the reason we
are trying to access a \
 `x` property in the `someprop` property which have an `undefined`
value. Remember **properties** in an object which does not exist in
itself and its **prototype** has a default value of `undefined` and
`undefined` has no property `x`.

### [](#12-what-is-eventtarget-) 12. What is **event.target** ?

[↑](#the-questions) In simplest terms, the **event.target** is the
element on which the event **occurred** or the element that
**triggered** the event.

Sample HTML Markup.\

```{.highlight .html}
<div onclick="clickFunc(event)" style="text-align: center;margin:15px;
border:1px solid red;border-radius:3px;">
    <div style="margin: 25px; border:1px solid royalblue;border-radius:3px;">
        <div style="margin:25px;border:1px solid skyblue;border-radius:3px;">
          <button style="margin:10px">
             Button
          </button>
        </div>
    </div>
  </div>
```

Enter fullscreen mode

Exit fullscreen mode

Sample JavaScript.\

```{.highlight .javascript}
 function clickFunc(event) {
  console.log(event.target);
}
```

Enter fullscreen mode

Exit fullscreen mode

If you click the button it will log the **button** markup even though we
attach the event on the outermost `div` it will always log the
**button** so we can conclude that the **event.target** is the element
that triggered the event.

### [](#13-what-is-eventcurrenttarget) 13. What is **event.currentTarget**?

[↑](#the-questions) The **event.currentTarget** is the element on which
we attach the event handler **explicitly**.

Copying the markup in **Question 12**.\
 Sample HTML Markup.\

```{.highlight .html}
<div onclick="clickFunc(event)" style="text-align: center;margin:15px;
border:1px solid red;border-radius:3px;">
    <div style="margin: 25px; border:1px solid royalblue;border-radius:3px;">
        <div style="margin:25px;border:1px solid skyblue;border-radius:3px;">
          <button style="margin:10px">
             Button
          </button>
        </div>
    </div>
  </div>
```

Enter fullscreen mode

Exit fullscreen mode

And changing our the **JS** a little bit.\

```{.highlight .javascript}
function clickFunc(event) {
  console.log(event.currentTarget);
}
```

Enter fullscreen mode

Exit fullscreen mode

If you click the button it will log the outermost **div** markup even
though we click the button. In this example, we can conclude that the
**event.currentTarget** is the element on which we attach the event
handler.

### [](#14-whats-the-difference-between-and-) 14. What's the difference between `==` and `===` ?

[↑](#the-questions) The difference between `==`**(abstract equality)**
and `===`**(strict equality)** is that the `==` compares by **value**
after _coercion_ and `===` compares by **value** and **type** without
_coercion_.

Let's dig deeper on the `==`. So first let's talk about _coercion_.

_coercion_ is the process of converting a value to another type. As in
this case, the `==` does _implicit coercion_. The `==` has some
conditions to perform before comparing the two values.

Suppose we have to compare `x == y` values.

1.  If `x` and `y` have same type. Then compare them with the `===`
    operator.
2.  If `x` is `null` and `y` is `undefined` then return `true`.
3.  If `x` is `undefined` and `y` is `null` then return `true`.
4.  If `x` is type `number` and `y` is type `string` Then return
    `x == toNumber(y)`.
5.  If `x` is type `string` and `y` is type `number` Then return
    `toNumber(x) == y`.
6.  If `x` is type `boolean` Then return `toNumber(x) == y`.
7.  If `y` is type `boolean` Then return `x == toNumber(y)`.
8.  If `x` is either `string`,`symbol` or `number` and `y` is type
    `object` Then return `x == toPrimitive(y)`.
9.  If `x` is either `object` and `x` is either `string`,`symbol` Then
    return `toPrimitive(x) == y`.
10. Return `false`.

**Note:** `toPrimitive` uses first the `valueOf` method then the
`toString` method in objects to get the primitive value of that object.

Let's have examples.

`x` `y` `x == y`

---

`5` `5` `true`
`1` `'1'` `true`
`null` `undefined` `true`
`0` `false` `true`
`'1,2'` `[1,2]` `true`
`'[object Object]'` `{}` `true`

These examples all return `true`.

The **first example** goes to **condition one** because `x` and `y` have
the same type and value.

The **second example** goes to **condition four** `y` is converted to a
`number` before comparing.

The **third example** goes to **condition two**.

The **fourth example** goes to **condition seven** because `y` is
`boolean`.

The **fifth example** goes to **condition eight**. The array is
converted to a `string` using the `toString()` method which returns
`1,2`.

The **last example** goes to **condition ten**. The object is converted
to a `string` using the `toString()` method which returns
`[object Object]`.

`x` `y` `x === y`

---

`5` `5` `true`
`1` `'1'` `false`
`null` `undefined` `false`
`0` `false` `false`
`'1,2'` `[1,2]` `false`
`'[object Object]'` `{}` `false`

If we use the `===` operator all the comparisons except for the first
example will return `false` because they don't have the same type while
the first example will return `true` because the two have the same type
and value.

### [](#15-why-does-it-return-false-when-comparing-two-similar-objects-in-javascript) 15. Why does it return **false** when comparing two similar objects in JavaScript?

[↑](#the-questions) Suppose we have an example below.\

```{.highlight .javascript}
let a = { a: 1 };
let b = { a: 1 };
let c = a;

console.log(a === b); // logs false even though they have the same property
console.log(a === c); // logs true hmm
```

Enter fullscreen mode

Exit fullscreen mode

**JavaScript** compares _objects_ and _primitives_ differently. In
_primitives_ it compares them by **value** while in _objects_ it
compares them by **reference** or the **address in memory where the
variable is stored**. That's why the first `console.log` statement
returns `false` and the second `console.log` statement returns `true`.
`a` and `c` have the same reference and `a` and `b` are not.

### [](#16-what-does-the-operator-do) 16. What does the **!!** operator do?

[↑](#the-questions) The **Double NOT** operator or **!!** coerces the
value on the right side into a boolean. basically it's a fancy way of
converting a value into a boolean.\

```{.highlight .javascript}
console.log(!!null); //logs false
console.log(!!undefined); //logs false
console.log(!!''); //logs false
console.log(!!0); //logs false
console.log(!!NaN); //logs false
console.log(!!' '); //logs true
console.log(!!{}); //logs true
console.log(!![]); //logs true
console.log(!!1); //logs true
console.log(!![].length); //logs false
```

Enter fullscreen mode

Exit fullscreen mode

### [](#17-how-to-evaluate-multiple-expressions-in-one-line) 17. How to evaluate multiple expressions in one line?

[↑](#the-questions)We can use the `,` or comma operator to evaluate
multiple expressions in one line. It evaluates from left-to-right and
returns the value of the last item on the right or the last operand.\

```{.highlight .javascript}
let x = 5;

x = (x++ , x = addFive(x), x *= 2, x -= 5, x += 10);

function addFive(num) {
  return num + 5;
}
```

Enter fullscreen mode

Exit fullscreen mode

If you log the value of `x` it would be **27**. First, we **increment**
the value of x it would be **6**, then we invoke the function
`addFive(6)` and pass the 6 as a parameter and assign the result to `x`
the new value of `x` would be **11**. After that, we multiply the
current value of `x` to **2** and assign it to `x` the updated value of
`x` would be **22**. Then, we subtract the current value of `x` to 5 and
assign the result to `x` the updated value would be **17**. And lastly,
we increment the value of `x` by 10 and assign the updated value to `x`
now the value of `x` would be **27**.

### [](#18-what-is-hoisting) 18. What is **Hoisting**?

[↑](#the-questions) **Hoisting** is the term used to describe the moving
of _variables_ and _functions_ to the top of their _(global or
function)_ scope on where we define that variable or function.

Ok to understand **Hoisting**, I have to explain the _execution
context_.\
 The **Execution Context** is the "environment of code" that is
currently executing. The **Execution Context** has two phases
_compilation_ and _execution_.

**Compilation** - in this phase it gets all the _function declarations_
and _hoists_ them up to the top of their scope so we can reference them
later and gets all _variables declaration_ **(declare with the var
keyword)** and also _hoists_ them up and give them a default value of
_undefined_.

**Execution** - in this phase it assigns values to the variables
_hoisted_ earlier and it _executes_ or _invokes_ functions **(methods in
objects)**.

**Note:** only **function declarations** and variables declared with the
_var_ keyword are _hoisted_ not **function expressions** or **arrow
functions**, `let` and `const` keywords.

Ok, suppose we have an example code in the _global scope_ below.\

```{.highlight .javascript}
console.log(y);
y = 1;
console.log(y);
console.log(greet("Mark"));

function greet(name){
  return 'Hello ' + name + '!';
}

var y;
```

Enter fullscreen mode

Exit fullscreen mode

This code logs `undefined`,`1`, `Hello Mark!` respectively.

So the _compilation_ phase would look like this.\

```{.highlight .javascript}
function greet(name) {
  return 'Hello ' + name + '!';
}

var y; //implicit "undefined" assignment

//waiting for "compilation" phase to finish

//then start "execution" phase
/*
console.log(y);
y = 1;
console.log(y);
console.log(greet("Mark"));
*/
```

Enter fullscreen mode

Exit fullscreen mode

for example purposes, I commented on the _assignment_ of variable and
_function call_.

After the _compilation_ phase finishes it starts the _execution_ phase
invoking methods and assigns values to variables.\

```{.highlight .javascript}
function greet(name) {
  return 'Hello ' + name + '!';
}

var y;

//start "execution" phase

console.log(y);
y = 1;
console.log(y);
console.log(greet("Mark"));
```

Enter fullscreen mode

Exit fullscreen mode

### [](#19-what-is-scope) 19. What is **Scope**?

[↑](#the-questions) **Scope** in JavaScript is the **area** where we
have valid access to variables or functions. JavaScript has three types
of Scopes. **Global Scope**, **Function Scope**, and **Block
Scope(ES6)**.

- **Global Scope** - variables or functions declared in the global
  namespace are in the global scope and therefore is accessible
  everywhere in our code.

```{.highlight .javascript}
   //global namespace
   var g = "global";

   function globalFunc(){
     function innerFunc(){
          console.log(g); // can access "g" because "g" is a global variable
     }
     innerFunc();
   }
```

Enter fullscreen mode

Exit fullscreen mode

- **Function Scope** - variables,functions and parameters declared
  within a function are accessible inside that function but not
  outside of it.

```{.highlight .javascript}
    function myFavoriteFunc(a) {
       if (true) {
          var b = "Hello " + a;
       }
       return b;
   }
   myFavoriteFunc("World");

   console.log(a); // Throws a ReferenceError "a" is not defined
   console.log(b); // does not continue here
```

Enter fullscreen mode

Exit fullscreen mode

- **Block Scope** - variables **(`let`,`const`)** declared within a
  block `{}` can only be access within it.

```{.highlight .javascript}
 function testBlock(){
   if(true){
     let z = 5;
   }
   return z;
 }

 testBlock(); // Throws a ReferenceError "z" is not defined
```

Enter fullscreen mode

Exit fullscreen mode

**Scope** is also a set of rules for finding variables. If a variable
does not exist in the **current scope** it **look ups** and searches for
a variable in the **outer scope** and if does not exist again it **looks
up** again until it reaches the **global scope** if the variable exists
then we can use it if not it throws an error. It searches for the
**nearest** variable and it stops **searching** or **looking up** once
it finds it. This is called **Scope Chain**.\

```{.highlight .javascript}
   /* Scope Chain
   Inside inner function perspective

   inner's scope -> outer's scope -> global's scope
  */


  //Global Scope
  var variable1 = "Comrades";
  var variable2 = "Sayonara";

  function outer(){
  //outer's scope
    var variable1 = "World";
    function inner(){
    //inner's scope
      var variable2 = "Hello";
      console.log(variable2 + " " + variable1);
    }
    inner();
  }
  outer();
// logs Hello World
// because (variable2 = "Hello") and (variable1 = "World") are the nearest
// variables inside inner's scope.
```

Enter fullscreen mode

Exit fullscreen mode

[![Scope](https://res.cloudinary.com/practicaldev/image/fetch/s--dJFL2g1k--/c_limit%2Cf_auto%2Cfl_progressive%2Cq_auto%2Cw_880/https://thepracticaldev.s3.amazonaws.com/i/l81b3nmdonimex0qsgyr.png)](https://res.cloudinary.com/practicaldev/image/fetch/s--dJFL2g1k--/c_limit%2Cf_auto%2Cfl_progressive%2Cq_auto%2Cw_880/https://thepracticaldev.s3.amazonaws.com/i/l81b3nmdonimex0qsgyr.png)

### [](#20-what-are-closures) 20. What are **Closures**?

[↑](#the-questions) This is probably the hardest question of all these
questions because **Closures** is a controversial topic. So I'm gonna
explain it from what I understand.

**Closures** is simply the ability of a function at the time of
declaration to remember the references of variables and parameters on
its current scope, on its parent function scope, on its parent's parent
function scope until it reaches the global scope with the help of
**Scope Chain**. Basically it is the **Scope** created when the function
was declared.

Examples are a great way to explain closures.\

```{.highlight .javascript}
   //Global's Scope
   var globalVar = "abc";

   function a(){
   //testClosures's Scope
     console.log(globalVar);
   }

   a(); //logs "abc"
   /* Scope Chain
      Inside a function perspective

      a's scope -> global's scope
   */
```

Enter fullscreen mode

Exit fullscreen mode

In this example, when we declare the `a` function the **Global Scope**
is part of `a's` _closure_.

[![a's
closure](https://res.cloudinary.com/practicaldev/image/fetch/s--gbH9Uqec--/c_limit%2Cf_auto%2Cfl_progressive%2Cq_auto%2Cw_880/https://thepracticaldev.s3.amazonaws.com/i/teatokuw4xvgtlzbzhn8.png)](https://res.cloudinary.com/practicaldev/image/fetch/s--gbH9Uqec--/c_limit%2Cf_auto%2Cfl_progressive%2Cq_auto%2Cw_880/https://thepracticaldev.s3.amazonaws.com/i/teatokuw4xvgtlzbzhn8.png)

The reason for the variable `globalVar` which does not have a value in
the image because of the reason that the value of that variable can
change based on **where** and **when** we invoke the `a` function.\
 But in our example above the `globalVar` variable will have the value
of **abc**.

Ok, let's have a complex example.\

```{.highlight .javascript}
var globalVar = "global";
var outerVar = "outer"

function outerFunc(outerParam) {
  function innerFunc(innerParam) {
    console.log(globalVar, outerParam, innerParam);
  }
  return innerFunc;
}

const x = outerFunc(outerVar);
outerVar = "outer-2";
globalVar = "guess"
x("inner");
```

Enter fullscreen mode

Exit fullscreen mode

[![Complex](https://res.cloudinary.com/practicaldev/image/fetch/s--inSFoNQU--/c_limit%2Cf_auto%2Cfl_progressive%2Cq_auto%2Cw_880/https://thepracticaldev.s3.amazonaws.com/i/e4hxm7zvz8eun2ppenwp.png)](https://res.cloudinary.com/practicaldev/image/fetch/s--inSFoNQU--/c_limit%2Cf_auto%2Cfl_progressive%2Cq_auto%2Cw_880/https://thepracticaldev.s3.amazonaws.com/i/e4hxm7zvz8eun2ppenwp.png)\
 This will print "guess outer inner". The explanation for this is that
when we invoke the `outerFunc` function and assigned the returned value
the `innerFunc` function to the variable `x`, the `outerParam` will have
a value of **outer** even though we assign a new value **outer-2** to
the `outerVar` variable because\
 the reassignment happened after the invocation of the `outer` function
and in that time when we invoke the `outerFunc` function it's look up
the value of `outerVar` in the **Scope Chain**, the `outerVar` will have
a value of **"outer"**. Now, when we invoke the `x` variable which have
a reference to the `innerFunc`, the\
 `innerParam` will have a value of **inner** because thats the value we
pass in the invocation and the `globalVar` variable will have a value of
**guess** because before the invocation of the `x` variable we assign a
new value to the `globalVar` and at the time of invocation `x` the value
of `globalVar` in the **Scope Chain** is **guess**.

We have an example that demonstrates a problem of not understanding
closure correctly.\

```{.highlight .javascript}
const arrFuncs = [];
for(var i = 0; i < 5; i++){
  arrFuncs.push(function (){
    return i;
  });
}
console.log(i); // i is 5

for (let i = 0; i < arrFuncs.length; i++) {
  console.log(arrFuncs[i]()); // all logs "5"
}
```

Enter fullscreen mode

Exit fullscreen mode

This code is not working as we expected because of **Closures**.\
 The `var` keyword makes a global variable and when we push a function \
 we return the global variable `i`. So when we call one of those
functions in that array after the loop it logs `5` because we get\
 the current value of `i` which is `5` and we can access it because it's
a global variable. Because **Closures** keeps the **references** of that
variable not its **values** at the time of it's creation. We can solve
this using **IIFES** or changing the `var` keyword to `let` for
block-scoping.

### [](#21-what-are-the-falsy-values-in-javascript) 21. What are the **falsy** values in **JavaScript**?

[↑](#the-questions)\

```{.highlight .javascript}
 const falsyValues = ['', 0, null, undefined, NaN, false];
```

Enter fullscreen mode

Exit fullscreen mode

**falsy** values are values that when converted to boolean becomes
**false**.

### [](#22-how-to-check-if-a-value-is-falsy) 22. How to check if a value is **falsy**?

[↑](#the-questions) Use the **Boolean** function or the Double NOT
operator **[!!](#16-what-does-the-operator-do)**

### [](#23-what-does-use-strict-do) 23. What does `"use strict"` do?

[↑](#the-questions) `"use strict"` is a ES5 feature in **JavaScript**
that makes our code in **Strict Mode** in _functions_ or _entire
scripts_. **Strict Mode** helps us avoid **bugs** early on in our code
and adds restrictions to it.

Restrictions that **Strict Mode** gives us.

- Assigning or Accessing a variable that is not declared.

```{.highlight .javascript}
 function returnY(){
    "use strict";
    y = 123;
    return y;
 }
```

Enter fullscreen mode

Exit fullscreen mode

- Assigning a value to a read-only or non-writable global variable;

```{.highlight .javascript}
   "use strict";
   var NaN = NaN;
   var undefined = undefined;
   var Infinity = "and beyond";
```

Enter fullscreen mode

Exit fullscreen mode

- Deleting an undeletable property.

```{.highlight .javascript}
   "use strict";
   const obj = {};

   Object.defineProperty(obj, 'x', {
      value : '1'
   });

   delete obj.x;
```

Enter fullscreen mode

Exit fullscreen mode

- Duplicate parameter names.

```{.highlight .javascript}
   "use strict";

   function someFunc(a, b, b, c){

   }
```

Enter fullscreen mode

Exit fullscreen mode

- Creating variables with the use of the **eval** function.

```{.highlight .javascript}
 "use strict";

 eval("var x = 1;");

 console.log(x); //Throws a Reference Error x is not defined
```

Enter fullscreen mode

Exit fullscreen mode

- The default value of **this** will be `undefined`.

```{.highlight .javascript}
  "use strict";

  function showMeThis(){
    return this;
  }

  showMeThis(); //returns undefined
```

Enter fullscreen mode

Exit fullscreen mode

There are many more restrictions in **Strict Mode** than these.

### [](#24-whats-the-value-of-this-in-javascript) 24. What's the value of `this` in JavaScript?

[↑](#the-questions) Basically, `this` refers to the value of the object
that is currently executing or invoking the function. I say
**currently** due to the reason that the value of **this** changes
depending on the context on which we use it and where we use it.\

```{.highlight .javascript}
   const carDetails = {
     name: "Ford Mustang",
     yearBought: 2005,
     getName(){
        return this.name;
     },
     isRegistered: true
   };

   console.log(carDetails.getName()); // logs Ford Mustang
```

Enter fullscreen mode

Exit fullscreen mode

This is what we would normally expect because in the **getName** method
we return `this.name`, `this` in this context refers to the object which
is the `carDetails` object that is currently the "owner" object of the
function executing.

Ok, Let's some add some code to make it weird. Below the `console.log`
statement add this three lines of code\

```{.highlight .javascript}
   var name = "Ford Ranger";
   var getCarName = carDetails.getName;

   console.log(getCarName()); // logs Ford Ranger
```

Enter fullscreen mode

Exit fullscreen mode

The second `console.log` statement prints the word **Ford Ranger** which
is weird because in our first `console.log` statement it printed **Ford
Mustang**. The reason to this is that the `getCarName` method has a
different "owner" object that is the `window` object. Declaring
variables with the `var` keyword in the global scope attaches properties
in the `window` object with the same name as the variables. Remember
`this` in the global scope refers to the `window` object when
`"use strict"` is not used.\

```{.highlight .javascript}
  console.log(getCarName === window.getCarName); //logs true
  console.log(getCarName === this.getCarName); // logs true
```

Enter fullscreen mode

Exit fullscreen mode

`this` and `window` in this example refer to the same object.

One way of solving this problem is by using the `apply` and `call`
methods in functions.\

```{.highlight .javascript}
   console.log(getCarName.apply(carDetails)); //logs Ford Mustang
   console.log(getCarName.call(carDetails));  //logs Ford Mustang
```

Enter fullscreen mode

Exit fullscreen mode

The `apply` and `call` methods expects the first parameter to be an
object which would be value of `this` inside that function.

**IIFE** or **Immediately Invoked Function Expression**, Functions that
are declared in the global scope, **Anonymous Functions** and Inner
functions in methods inside an object has a default of **this** which
points to the **window** object.\

```{.highlight .javascript}
   (function (){
     console.log(this);
   })(); //logs the "window" object

   function iHateThis(){
      console.log(this);
   }

   iHateThis(); //logs the "window" object

   const myFavoriteObj = {
     guessThis(){
        function getThis(){
          console.log(this);
        }
        getThis();
     },
     name: 'Marko Polo',
     thisIsAnnoying(callback){
       callback();
     }
   };


   myFavoriteObj.guessThis(); //logs the "window" object
   myFavoriteObj.thisIsAnnoying(function (){
     console.log(this); //logs the "window" object
   });
```

Enter fullscreen mode

Exit fullscreen mode

If we want to get the value of the `name` property which is **Marko
Polo** in the `myFavoriteObj` object there are two ways to solve this.

First, we save the value of `this` in a variable.\

```{.highlight .javascript}
   const myFavoriteObj = {
     guessThis(){
         const self = this; //saves the this value to the "self" variable
         function getName(){
           console.log(self.name);
         }
         getName();
     },
     name: 'Marko Polo',
     thisIsAnnoying(callback){
       callback();
     }
   };
```

Enter fullscreen mode

Exit fullscreen mode

In this image we save the value of `this` which would be the
`myFavoriteObj` object. So we can access it inside the `getName` inner
function.

Second, we use **ES6 [Arrow Functions](#43-what-are-arrow-functions)**.\

```{.highlight .javascript}
   const myFavoriteObj = {
     guessThis(){
         const getName = () => {
           //copies the value of "this" outside of this arrow function
           console.log(this.name);
         }
         getName();
     },
     name: 'Marko Polo',
     thisIsAnnoying(callback){
       callback();
     }
   };
```

Enter fullscreen mode

Exit fullscreen mode

[Arrow Functions](#43-what-are-arrow-functions) does not have its own
`this`. It copies the value of `this` of the enclosing lexical scope or
in this example the value of `this` outside the `getName` inner function
which would be the `myFavoriteObj` object. We can also determine the
value of `this` on [how the function is
invoked](#66-how-many-ways-can-a-function-be-invoked).

### [](#25-what-is-the-prototype-of-an-object) 25. What is the `prototype` of an object?

[↑](#the-questions) A `prototype` in simplest terms is a _blueprint_ of
an object. It is used as a fallback for **properties** and **methods**
if it does exist in the current object. It's the way to share properties
and functionality between objects. It's the core concept around
JavaScript's **Prototypal Inheritance**.\

```{.highlight .javascript}
  const o = {};
  console.log(o.toString()); // logs [object Object]
```

Enter fullscreen mode

Exit fullscreen mode

Even though the `o.toString` method does not exist in the `o` object it
does not throw an error instead returns a string `[object Object]`. When
a property does not exist in the object it looks into its **prototype**
and if it still does not exist it looks into the **prototype's
prototype** and so on until it finds a property with the same in the
**Prototype Chain**. The end of the **Prototype Chain** is the
**Object.prototype**.\

```{.highlight .javascript}
   console.log(o.toString === Object.prototype.toString); // logs true
   // which means we we're looking up the Prototype Chain and it reached
   // the Object.prototype and used the "toString" method.
```

Enter fullscreen mode

Exit fullscreen mode

### [](#26-what-is-an-iife-what-is-the-use-of-it) 26. What is an **IIFE**, what is the use of it?

[↑](#the-questions) An **IIFE** or **Immediately Invoked Function
Expression** is a function that is gonna get invoked or executed after
its creation or declaration. The syntax for creating **IIFE** is that we
wrap the `function (){}` inside a parentheses `()` or the **Grouping
Operator** to treat the function as an expression and after that we
invoke it with another parentheses `()`. So an **IIFE** looks like this
`(function(){})()`.\

```{.highlight .javascript}
(function () {

}());

(function () {

})();

(function named(params) {

})();

(() => {

})();

(function (global) {

})(window);

const utility = (function () {
   return {
      //utilities
   };
})();
```

Enter fullscreen mode

Exit fullscreen mode

These examples are all valid **IIFE**. The second to the last example
shows we can pass arguments to an **IIFE** function. The last example
shows that we can save the result of the **IIFE** to a variable so we
can reference it later.

The best use of **IIFE** is making initialization setup functionalities
and to avoid **naming collisions** with other variables in the global
scope or polluting the global namespace. Let's have an example.\

```{.highlight .html}
<script src="https://cdnurl.com/somelibrary.js"></script>
```

Enter fullscreen mode

Exit fullscreen mode

Suppose we have a link to a library `somelibrary.js` that exposes some
global functions that we use can in our code but this library has two
methods that we don't use `createGraph` and `drawGraph` because these
methods have bugs in them. And we want to implement our own
`createGraph` and `drawGraph` methods.

- One way of solving this is by changing the structure of our scripts.

```{.highlight .html}
<script src="https://cdnurl.com/somelibrary.js"></script>
<script>
   function createGraph() {
      // createGraph logic here
   }
   function drawGraph() {
      // drawGraph logic here
   }
</script>
```

Enter fullscreen mode

Exit fullscreen mode

When we use this solution we are overriding those two methods that the
library gives us.

- Another way of solving this is by changing the name of our own
  helper functions.

```{.highlight .html}
<script src="https://cdnurl.com/somelibrary.js"></script>
<script>
   function myCreateGraph() {
      // createGraph logic here
   }
   function myDrawGraph() {
      // drawGraph logic here
   }
</script>
```

Enter fullscreen mode

Exit fullscreen mode

When we use this solution we will also change those function calls to
the new function names.

- Another way is using an **IIFE**.

```{.highlight .html}
<script src="https://cdnurl.com/somelibrary.js"></script>
<script>
   const graphUtility = (function () {
      function createGraph() {
         // createGraph logic here
      }
      function drawGraph() {
         // drawGraph logic here
      }
      return {
         createGraph,
         drawGraph
      }
   })();
</script>
```

Enter fullscreen mode

Exit fullscreen mode

In this solution, we are making a utility variable that is the result of
**IIFE** which returns an object that contains two methods `createGraph`
and `drawGraph`.

Another problem that **IIFE** solves is in this example.\

```{.highlight .javascript}
var li = document.querySelectorAll('.list-group > li');
for (var i = 0, len = li.length; i < len; i++) {
   li[i].addEventListener('click', function (e) {
      console.log(i);
   })
}
```

Enter fullscreen mode

Exit fullscreen mode

Suppose we have a `ul` element with a class of **list-group** and it has
5 `li` child elements. And we want to `console.log` the value of `i`
when we **click** an individual `li` element. \
 But the behavior we want in this code does not work. Instead, it logs
`5` in any **click** on an `li` element. The problem we're having is due
to how **Closures** work. **Closures** are simply the ability of
functions to remember the references of variables on its current scope,
on its parent function scope and in the global scope. When we declare
variables using the `var` keyword in the global scope, obviously we are
making a global variable `i`. So when we click an `li` element it logs
**5** because that is the value of `i` when we reference it later in the
callback function.

- One solution to this is an **IIFE**.

```{.highlight .javascript}
var li = document.querySelectorAll('.list-group > li');
for (var i = 0, len = li.length; i < len; i++) {
   (function (currentIndex) {
      li[currentIndex].addEventListener('click', function (e) {
         console.log(currentIndex);
      })
   })(i);
}
```

Enter fullscreen mode

Exit fullscreen mode

This solution works because of the reason that the **IIFE** creates a
new scope for every iteration and we capture the value of `i` and pass
it into the `currentIndex` parameter so the value of `currentIndex` is
different for every iteration when we invoke the **IIFE**.

### [](#27-what-is-the-use-functionprototypeapply-method) 27. What is the use `Function.prototype.apply` method?

[↑](#the-questions) The `apply` invokes a function specifying the `this`
or the "owner" object of that function on that time of invocation.\

```{.highlight .javascript}
const details = {
  message: 'Hello World!'
};

function getMessage(){
  return this.message;
}

getMessage.apply(details); // returns 'Hello World!'
```

Enter fullscreen mode

Exit fullscreen mode

This method works like `Function.prototype.call` the only difference is
how we pass arguments. In `apply` we pass arguments as an array.\

```{.highlight .javascript}
const person = {
  name: "Marko Polo"
};

function greeting(greetingMessage) {
  return `${greetingMessage} ${this.name}`;
}

greeting.apply(person, ['Hello']); // returns "Hello Marko Polo!"
```

Enter fullscreen mode

Exit fullscreen mode

### [](#28-what-is-the-use-functionprototypecall-method) 28. What is the use `Function.prototype.call` method?

[↑](#the-questions) The `call` invokes a function specifying the `this`
or the "owner" object of that function on that time of invocation.\

```{.highlight .javascript}
const details = {
  message: 'Hello World!'
};

function getMessage(){
  return this.message;
}

getMessage.call(details); // returns 'Hello World!'
```

Enter fullscreen mode

Exit fullscreen mode

This method works like `Function.prototype.apply` the only difference is
how we pass arguments. In `call` we pass directly the arguments
separating them with a comma `,` for every argument.\

```{.highlight .javascript}
const person = {
  name: "Marko Polo"
};

function greeting(greetingMessage) {
  return `${greetingMessage} ${this.name}`;
}

greeting.call(person, 'Hello'); // returns "Hello Marko Polo!"
```

Enter fullscreen mode

Exit fullscreen mode

### [](#29-whats-the-difference-between-functionprototypeapply-and-functionprototypecall) 29. What's the difference between `Function.prototype.apply` and `Function.prototype.call`?

[↑](#the-questions) The only difference between `apply` and `call` is
how we pass the **arguments** in the function being called. In `apply`
we pass the arguments as an **array** and in `call` we pass the
arguments directly in the argument list.\

```{.highlight .javascript}
const obj1 = {
 result:0
};

const obj2 = {
 result:0
};

function reduceAdd(){
   let result = 0;
   for(let i = 0, len = arguments.length; i < len; i++){
     result += arguments[i];
   }
   this.result = result;
}

reduceAdd.apply(obj1, [1, 2, 3, 4, 5]); // returns 15
reduceAdd.call(obj2, 1, 2, 3, 4, 5); // returns 15
```

Enter fullscreen mode

Exit fullscreen mode

### [](#30-what-is-the-usage-of-functionprototypebind) 30. What is the usage of `Function.prototype.bind`?

[↑](#the-questions) The `bind` method returns a new function that is
_bound_ \
 to a specific `this` value or the "owner" object, So we can use it
later in our code. The `call`,`apply` methods invokes the function
immediately instead of returning a new function like the `bind` method.\

```{.highlight .javascript}
import React from 'react';

class MyComponent extends React.Component {
     constructor(props){
          super(props);
          this.state = {
             value : ""
          }
          this.handleChange = this.handleChange.bind(this);
          // Binds the "handleChange" method to the "MyComponent" component
     }

     handleChange(e){
       //do something amazing here
     }

     render(){
        return (
              <>
                <input type={this.props.type}
                        value={this.state.value}
                     onChange={this.handleChange}
                  />
              </>
        )
     }
}
```

Enter fullscreen mode

Exit fullscreen mode

### [](#31-what-is-functional-programming-and-what-are-the-features-of-javascript-that-makes-it-a-candidate-as-a-functional-language) 31. What is **Functional Programming** and what are the features of **JavaScript** that makes it a candidate as a **functional language**?

[↑](#the-questions) **Functional Programming** is a **declarative**
programming paradigm or pattern on how we build our applications with
**functions** using **expressions** that calculates a value without
mutating or changing the arguments that are passed to it.

JavaScript **Array** has **map**, **filter**, **reduce** methods which
are the most famous functions in the functional programming world
because of their usefulness and because they don't mutate or change the
array which makes these functions **pure** and JavaScript supports
**Closures** and **Higher Order Functions** which are a characteristic
of a **Functional Programming Language**.

- The **map** method creates a new array with the results of calling a
  provided callback function on every element in the array.

```{.highlight .javascript}
const words = ["Functional", "Procedural", "Object-Oriented"];

const wordsLength = words.map(word => word.length);
```

Enter fullscreen mode

Exit fullscreen mode

- The **filter** method creates a new array with all elements that
  pass the test in the callback function.

```{.highlight .javascript}
const data = [
  { name: 'Mark', isRegistered: true },
  { name: 'Mary', isRegistered: false },
  { name: 'Mae', isRegistered: true }
];

const registeredUsers = data.filter(user => user.isRegistered);
```

Enter fullscreen mode

Exit fullscreen mode

- The **reduce** method applies a function against an accumulator and
  each element in the array (from left to right) to reduce it to a
  single value.

```{.highlight .javascript}
const strs = ["I", " ", "am", " ", "Iron", " ", "Man"];
const result = strs.reduce((acc, currentStr) => acc + currentStr, "");
```

Enter fullscreen mode

Exit fullscreen mode

### [](#32-what-are-higher-order-functions) 32. What are **Higher Order Functions**?

[↑](#the-questions) **Higher-Order Function** are functions that can
return a function or receive argument or arguments which have a value of
a function.\

```{.highlight .javascript}
function higherOrderFunction(param,callback){
    return callback(param);
}
```

Enter fullscreen mode

Exit fullscreen mode

### [](#33-why-are-functions-called-firstclass-objects) 33. Why are functions called **First-class Objects**?

[↑](#the-questions)**Functions** in JavaScript are **First-class
Objects** because they are treated as any other value in the language.
They can be assigned to **variables**, they can be **properties of an
object** which are called **methods**, they can be an **item in array**,
they can be **passed as arguments to a function**, and they can be
**returned as values of a function**. The only difference between a
function and any other value in **JavaScript** is that **functions** can
be invoked or called.

### [](#34-implement-the-arrayprototypemap-method-by-hand) 34. Implement the `Array.prototype.map` method by hand.

[↑](#the-questions)\

```{.highlight .javascript}
function map(arr, mapCallback) {
  // First, we check if the parameters passed are right.
  if (!Array.isArray(arr) || !arr.length || typeof mapCallback !== 'function') {
    return [];
  } else {
    let result = [];
    // We're making a results array every time we call this function
    // because we don't want to mutate the original array.
    for (let i = 0, len = arr.length; i < len; i++) {
      result.push(mapCallback(arr[i], i, arr));
      // push the result of the mapCallback in the 'result' array
    }
    return result; // return the result array
  }
}
```

Enter fullscreen mode

Exit fullscreen mode

As the MDN description of the `Array.prototype.map` method.

**The map() method creates a new array with the results of calling a
provided function on every element in the calling array.**

### [](#35-implement-the-arrayprototypefilter-method-by-hand) 35. Implement the `Array.prototype.filter` method by hand.

[↑](#the-questions)\

```{.highlight .javascript}
function filter(arr, filterCallback) {
  // First, we check if the parameters passed are right.
  if (!Array.isArray(arr) || !arr.length || typeof filterCallback !== 'function')
  {
    return [];
  } else {
    let result = [];
    // We're making a results array every time we call this function
    // because we don't want to mutate the original array.
    for (let i = 0, len = arr.length; i < len; i++) {
      // check if the return value of the filterCallback is true or "truthy"
      if (filterCallback(arr[i], i, arr)) {
      // push the current item in the 'result' array if the condition is true
        result.push(arr[i]);
      }
    }
    return result; // return the result array
  }
}
```

Enter fullscreen mode

Exit fullscreen mode

As the MDN description of the `Array.prototype.filter` method.

**The filter() method creates a new array with all elements that pass
the test implemented by the provided function.**

### [](#36-implement-the-arrayprototypereduce-method-by-hand) 36. Implement the `Array.prototype.reduce` method by hand.

[↑](#the-questions)\

```{.highlight .javascript}
function reduce(arr, reduceCallback, initialValue) {
  // First, we check if the parameters passed are right.
  if (!Array.isArray(arr) || !arr.length || typeof reduceCallback !== 'function')
  {
    return [];
  } else {
    // If no initialValue has been passed to the function we're gonna use the
    let hasInitialValue = initialValue !== undefined;
    let value = hasInitialValue ? initialValue : arr[0];
    // first array item as the initialValue

    // Then we're gonna start looping at index 1 if there is no
    // initialValue has been passed to the function else we start at 0 if
    // there is an initialValue.
    for (let i = hasInitialValue ? 0 : 1, len = arr.length; i < len; i++) {
      // Then for every iteration we assign the result of the
      // reduceCallback to the variable value.
      value = reduceCallback(value, arr[i], i, arr);
    }
    return value;
  }
}
```

Enter fullscreen mode

Exit fullscreen mode

As the MDN description of the `Array.prototype.reduce` method.

**The reduce() method executes a reducer function (that you provide) on
each element of the array, resulting in a single output value.**

### [](#37-what-is-the-arguments-object) 37. What is the **arguments** object?

[↑](#the-questions) The **arguments** object is a collection of
parameter values pass in a function. It's an **Array-like** object
because it has a **length** property and we can access individual values
using array indexing notation `arguments[1]` but it does not have the
built-in methods in an array `forEach`,`reduce`,`filter` and `map`.\
 It helps us know the number of arguments pass in a function.

We can convert the `arguments` object into an array using the
`Array.prototype.slice`.\

```{.highlight .javascript}
function one() {
  return Array.prototype.slice.call(arguments);
}
```

Enter fullscreen mode

Exit fullscreen mode

Note: **the `arguments` object does not work on ES6 arrow functions.**\

```{.highlight .javascript}
function one() {
  return arguments;
}
const two = function () {
  return arguments;
}
const three = function three() {
  return arguments;
}

const four = () => arguments;

four(); // Throws an error  - arguments is not defined
```

Enter fullscreen mode

Exit fullscreen mode

When we invoke the function `four` it throws a
`ReferenceError: arguments is not defined` error. We can solve this
problem if your enviroment supports the **rest syntax**.\

```{.highlight .javascript}
const four = (...args) => args;
```

Enter fullscreen mode

Exit fullscreen mode

This puts all parameter values in an array automatically.

### [](#38-how-to-create-an-object-without-a-prototype) 38. How to create an object without a **prototype**?

[↑](#the-questions) We can create an object without a _prototype_ using
the `Object.create` method.\

```{.highlight .javascript}
   const o1 = {};
   console.log(o1.toString());
   // logs [object Object] get this method to the Object.prototype

   const o2 = Object.create(null);
   // the first parameter is the prototype of the object "o2" which in this
   // case will be null specifying we don't want any prototype
   console.log(o2.toString());
   // throws an error o2.toString is not a function
```

Enter fullscreen mode

Exit fullscreen mode

### [](#39-why-does-b-in-this-code-become-a-global-variable-when-you-call-this-function) 39. Why does `b` in this code become a global variable when you call this function?

[↑](#the-questions)\

```{.highlight .javascript}
function myFunc() {
  let a = b = 0;
}

myFunc();
```

Enter fullscreen mode

Exit fullscreen mode

The reason for this is that **assignment operator** or **=** has
right-to-left **associativity** or **evaluation**. What this means is
that when multiple assignment operators appear in a single expression
they evaluated from right to left. So our code becomes likes this.\

```{.highlight .javascript}
function myFunc() {
  let a = (b = 0);
}

myFunc();
```

Enter fullscreen mode

Exit fullscreen mode

First, the expression `b = 0` evaluated and in this example `b` is not
declared. So, The JS Engine makes a global variable `b` outside this
function after that the return value of the expression `b = 0` would be
0 and it's assigned to the new local variable `a` with a `let` keyword.

We can solve this problem by declaring the variables first before
assigning them with value.\

```{.highlight .javascript}
function myFunc() {
  let a,b;
  a = b = 0;
}
myFunc();
```

Enter fullscreen mode

Exit fullscreen mode

### [](#40-what-is-ecmascript) 40. What is **ECMAScript**?

[↑](#the-questions) **ECMAScript** is a standard for making scripting
languages which means that **JavaScript** follows the specification
changes in **ECMAScript** standard because it is the **blueprint** of
**JavaScript**.

### [](#41-what-are-the-new-features-in-es6-or-ecmascript-2015) 41. What are the new features in **ES6** or **ECMAScript 2015**?

[↑](#the-questions)

- [Arrow Functions](#43-what-are-arrow-functions)

- [Classes](#44-what-are-classes)

- [Template Strings](#45-what-are-template-literals)

- **Enhanced Object literals**

- [Object Destructuring](#46-what-is-object-destructuring)

- [Promises](#50-what-are-promises)

- **Generators**

- [Modules](#47-what-are-es6-modules)

- Symbol

- **Proxies**

- [Sets](#48-what-is-the-set-object-and-how-does-it-work)

- [Default Function parameters](#53-what-are-default-parameters)

- [Rest and
  Spread](#52-whats-the-difference-between-spread-operator-and-rest-operator)

- [Block Scoping with `let` and
  `const`](#42-whats-the-difference-between-var-let-and-const-keywords)

### [](#42-whats-the-difference-between-var-let-and-const-keywords) 42. What's the difference between `var`, `let` and `const` keywords?

[↑](#the-questions) Variables declared with `var` keyword are _function
scoped_.\
 What this means that variables can be accessed across that function
even if we declare that variable inside a block.\

```{.highlight .javascript}
function giveMeX(showX) {
  if (showX) {
    var x = 5;
  }
  return x;
}

console.log(giveMeX(false));
console.log(giveMeX(true));
```

Enter fullscreen mode

Exit fullscreen mode

The first `console.log` statement logs `undefined`\
 and the second `5`. We can access the `x` variable due\
 to the reason that it gets _hoisted_ at the top of the function scope.
So our function code is intepreted like this.\

```{.highlight .javascript}
function giveMeX(showX) {
  var x; // has a default value of undefined
  if (showX) {
    x = 5;
  }
  return x;
}
```

Enter fullscreen mode

Exit fullscreen mode

If you are wondering why it logs `undefined` in the first `console.log`
statement remember variables declared without an initial value has a
default value of `undefined`.

Variables declared with `let` and `const` keyword are _block scoped_.
What this means that variable can only be accessed on that block `{}` on
where we declare it.\

```{.highlight .javascript}
function giveMeX(showX) {
  if (showX) {
    let x = 5;
  }
  return x;
}


function giveMeY(showY) {
  if (showY) {
    let y = 5;
  }
  return y;
}
```

Enter fullscreen mode

Exit fullscreen mode

If we call this functions with an argument of `false` it throws a
`Reference Error` because we can't access the `x` and `y` variables
outside that block and those variables are not _hoisted_.

There is also a difference between `let` and `const` we can assign new
values using `let` but we can't in `const` but `const` are mutable
meaning. What this means is if the value that we assign to a `const` is
an object we can change the values of those properties but can't
reassign a new value to that variable.

### [](#43-what-are-arrow-functions) 43. What are **Arrow functions**?

[↑](#the-questions) **Arrow Functions** are a new way of making
functions in JavaScript. **Arrow Functions** takes a little time in
making functions and has a cleaner syntax than a **function expression**
because we omit the `function` keyword in making them.\

```{.highlight .javascript}
//ES5 Version
var getCurrentDate = function (){
  return new Date();
}

//ES6 Version
const getCurrentDate = () => new Date();
```

Enter fullscreen mode

Exit fullscreen mode

In this example, in the ES5 Version have `function(){}` declaration and
`return` keyword needed to make a function and return a value
respectively. In the **Arrow Function** version we only need the `()`
parentheses and we don't need a `return` statement because **Arrow
Functions** have a implicit return if we have only one expression or
value to return.\

```{.highlight .javascript}
//ES5 Version
function greet(name) {
  return 'Hello ' + name + '!';
}

//ES6 Version
const greet = (name) => `Hello ${name}`;
const greet2 = name => `Hello ${name}`;
```

Enter fullscreen mode

Exit fullscreen mode

We can also parameters in **Arrow functions** the same as the **function
expressions** and **function declarations**. If we have one parameter in
an **Arrow Function** we can omit the parentheses it is also valid.\

```{.highlight .javascript}
const getArgs = () => arguments

const getArgs2 = (...rest) => rest
```

Enter fullscreen mode

Exit fullscreen mode

**Arrow functions** don't have access to the `arguments` object. So
calling the first `getArgs` func will throw an Error. Instead we can use
the **rest parameters** to get all the arguments passed in an arrow
function.\

```{.highlight .javascript}
const data = {
  result: 0,
  nums: [1, 2, 3, 4, 5],
  computeResult() {
    // "this" here refers to the "data" object
    const addAll = () => {
      // arrow functions "copies" the "this" value of
      // the lexical enclosing function
      return this.nums.reduce((total, cur) => total + cur, 0)
    };
    this.result = addAll();
  }
};
```

Enter fullscreen mode

Exit fullscreen mode

**Arrow functions** don't have their own `this` value. It captures or
gets the `this` value of lexically enclosing function or in this
example, the `addAll` function copies the `this` value of the
`computeResult` method and if we declare an arrow function in the global
scope the value of `this` would be the `window` object.

### [](#44-what-are-classes) 44. What are **Classes**?

[↑](#the-questions) **Classes** is the new way of writing _constructor
functions_ in **JavaScript**. It is _syntactic sugar_ for using
_constructor functions_, it still uses **prototypes** and
**Prototype-Based Inheritance** under the hood.\

```{.highlight .javascript}
   //ES5 Version
   function Person(firstName, lastName, age, address){
      this.firstName = firstName;
      this.lastName = lastName;
      this.age = age;
      this.address = address;
   }

   Person.self = function(){
     return this;
   }

   Person.prototype.toString = function(){
     return "[object Person]";
   }

   Person.prototype.getFullName = function (){
     return this.firstName + " " + this.lastName;
   }

   //ES6 Version
   class Person {
        constructor(firstName, lastName, age, address){
            this.lastName = lastName;
            this.firstName = firstName;
            this.age = age;
            this.address = address;
        }

        static self() {
           return this;
        }

        toString(){
           return "[object Person]";
        }

        getFullName(){
           return `${this.firstName} ${this.lastName}`;
        }
   }
```

Enter fullscreen mode

Exit fullscreen mode

**Overriding Methods** and **Inheriting from another class**.\

```{.highlight .javascript}
//ES5 Version
Employee.prototype = Object.create(Person.prototype);

function Employee(firstName, lastName, age, address, jobTitle, yearStarted) {
  Person.call(this, firstName, lastName, age, address);
  this.jobTitle = jobTitle;
  this.yearStarted = yearStarted;
}

Employee.prototype.describe = function () {
  return `I am ${this.getFullName()} and I have a position of ${this.jobTitle} and I started at ${this.yearStarted}`;
}

Employee.prototype.toString = function () {
  return "[object Employee]";
}

//ES6 Version
class Employee extends Person { //Inherits from "Person" class
  constructor(firstName, lastName, age, address, jobTitle, yearStarted) {
    super(firstName, lastName, age, address);
    this.jobTitle = jobTitle;
    this.yearStarted = yearStarted;
  }

  describe() {
    return `I am ${this.getFullName()} and I have a position of ${this.jobTitle} and I started at ${this.yearStarted}`;
  }

  toString() { // Overriding the "toString" method of "Person"
    return "[object Employee]";
  }
}
```

Enter fullscreen mode

Exit fullscreen mode

So how do we know that it uses _prototypes_ under the hood?\

```{.highlight .javascript}
   class Something {

   }

   function AnotherSomething(){

   }
   const as = new AnotherSomething();
   const s = new Something();

   console.log(typeof Something); // logs "function"
   console.log(typeof AnotherSomething); // logs "function"
   console.log(as.toString()); // logs "[object Object]"
   console.log(as.toString()); // logs "[object Object]"
   console.log(as.toString === Object.prototype.toString);
   console.log(s.toString === Object.prototype.toString);
   // both logs return true indicating that we are still using
   // prototypes under the hoods because the Object.prototype is
   // the last part of the Prototype Chain and "Something"
   // and "AnotherSomething" both inherit from Object.prototype
```

Enter fullscreen mode

Exit fullscreen mode

### [](#45-what-are-template-literals) 45. What are **Template Literals**?

[↑](#the-questions) **Template Literals** are a new way of making
**strings** in JavaScript. We can make **Template Literal** by using the
backtick or back-quote symbol.\

```{.highlight .javascript}
//ES5 Version
var greet = 'Hi I\'m Mark';

//ES6 Version
let greet = `Hi I'm Mark`;
```

Enter fullscreen mode

Exit fullscreen mode

In the ES5 version, we need to escape the `'` using the `\` to _escape_
the normal functionality of that symbol which in this case is to finish
that string value. In Template Literals, we don't need to do that.\

```{.highlight .javascript}
//ES5 Version
var lastWords = '\n'
  + '   I  \n'
  + '   Am  \n'
  + 'Iron Man \n';


//ES6 Version
let lastWords = `
    I
    Am
  Iron Man
`;
```

Enter fullscreen mode

Exit fullscreen mode

In the ES5 version, we need to add this `\n` to have a new line in our
string. In Template Literals, we don't need to do that.\

```{.highlight .javascript}
//ES5 Version
function greet(name) {
  return 'Hello ' + name + '!';
}


//ES6 Version
const greet = name => {
  return `Hello ${name} !`;
}
```

Enter fullscreen mode

Exit fullscreen mode

In the ES5 version, If we need to add an expression or value in a string
we need to use the `+` or string concatenation operator. In Template
Literals, we can embed an expression using `${expr}` which makes it
cleaner than the ES5 version.

### [](#46-what-is-object-destructuring) 46. What is **Object Destructuring**?

[↑](#the-questions) **Object Destructuring** is a new and cleaner way of
**getting** or **extracting** values from an object or an array.

Suppose we have an object that looks like this.\

```{.highlight .javascript}
const employee = {
  firstName: "Marko",
  lastName: "Polo",
  position: "Software Developer",
  yearHired: 2017
};
```

Enter fullscreen mode

Exit fullscreen mode

The old way of getting properties from an object is we make a variable
that has the same name as the object property. This way is a hassle
because we're making a new variable for every property. Imagine we have
a big object with lots of properties and methods using this way in
extracting properties will be irritating.\

```{.highlight .javascript}
var firstName = employee.firstName;
var lastName = employee.lastName;
var position = employee.position;
var yearHired = employee.yearHired;
```

Enter fullscreen mode

Exit fullscreen mode

If we use **object destructuring** it looks cleaner and takes a little
time than the old way. The syntax for object destructuring is that if we
are getting properties in an object we use the `{}` and inside that, we
specify the properties we want to extract and if we are getting data
from an array we use the `[]`.\

```{.highlight .javascript}
let { firstName, lastName, position, yearHired } = employee;
```

Enter fullscreen mode

Exit fullscreen mode

If we want to change the variable name we want to extract we use the
`propertyName:newName` syntax. In this example the value of `fName`
variable will hold the value of the `firstName` property and `lName`
variable will hold the value of the `lastName` property.\

```{.highlight .javascript}
let { firstName: fName, lastName: lName, position, yearHired } = employee;
```

Enter fullscreen mode

Exit fullscreen mode

We can also have default values when destructuring. In this example, if
the `firstName` property holds an `undefined` value in the object then
when we destructure the `firstName` variable will hold a default of
`"Mark"`.\

```{.highlight .javascript}
let { firstName = "Mark", lastName: lName, position, yearHired } = employee;
```

Enter fullscreen mode

Exit fullscreen mode

### [](#47-what-are-es6-modules) 47. What are `ES6 Modules`?

[↑](#the-questions) **Modules** lets us split our code base to multiple
files for more maintainability and this lets us avoid putting all of our
code in one big file (yucksss). Before ES6 has supported Modules there
were two popular module systems that were used for Code Maintainability
in **JavaScript**.

- CommonJS - **Nodejs**
- AMD (Asynchronous Module Definition) - **Browsers**

Basically, the sytanx for using modules are straightforward, \
 `import` is used for _getting_ functionality from another file or
several functionalities or values while \
 `export` is used for _exposing_ functionality from a file or several
functionalities or values.

**Exporting functionalites in a File or Named Exports**

_Using ES5 (CommonJS)_\

```{.highlight .javascript}
// Using ES5 CommonJS - helpers.js
exports.isNull = function (val) {
  return val === null;
}

exports.isUndefined = function (val) {
  return val === undefined;
}

exports.isNullOrUndefined = function (val) {
  return exports.isNull(val) || exports.isUndefined(val);
}
```

Enter fullscreen mode

Exit fullscreen mode

_Using ES6 Modules_\

```{.highlight .javascript}
// Using ES6 Modules - helpers.js
export function isNull(val){
  return val === null;
}

export function isUndefined(val) {
  return val === undefined;
}

export function isNullOrUndefined(val) {
  return isNull(val) || isUndefined(val);
}

```

Enter fullscreen mode

Exit fullscreen mode

**Importing functionalites in another File**\

```{.highlight .javascript}
// Using ES5 (CommonJS) - index.js
const helpers = require('./helpers.js'); // helpers is an object
const isNull = helpers.isNull;
const isUndefined = helpers.isUndefined;
const isNullOrUndefined = helpers.isNullOrUndefined;

// or if your environment supports Destructuring
const { isNull, isUndefined, isNullOrUndefined } = require('./helpers.js');
```

Enter fullscreen mode

Exit fullscreen mode

```{.highlight .javascript}
// ES6 Modules - index.js
import * as helpers from './helpers.js'; // helpers is an object

// or

import { isNull, isUndefined, isNullOrUndefined as isValid } from './helpers.js';

// using "as" for renaming named exports
```

Enter fullscreen mode

Exit fullscreen mode

**Exporting a Single Functionality in a File or Default Exports**

_Using ES5 (CommonJS)_\

```{.highlight .javascript}
// Using ES5 (CommonJS) - index.js
class Helpers {
  static isNull(val) {
    return val === null;
  }

  static isUndefined(val) {
    return val === undefined;
  }

  static isNullOrUndefined(val) {
    return this.isNull(val) || this.isUndefined(val);
  }
}


module.exports = Helpers;
```

Enter fullscreen mode

Exit fullscreen mode

_Using ES6 Modules_\

```{.highlight .javascript}
// Using ES6 Modules - helpers.js
class Helpers {
  static isNull(val) {
    return val === null;
  }

  static isUndefined(val) {
    return val === undefined;
  }

  static isNullOrUndefined(val) {
    return this.isNull(val) || this.isUndefined(val);
  }
}

export default Helpers
```

Enter fullscreen mode

Exit fullscreen mode

**Importing a Single Functionality from another File**

_Using ES5 (CommonJS)_\

```{.highlight .javascript}
// Using ES5 (CommonJS) - index.js
const Helpers = require('./helpers.js');
console.log(Helpers.isNull(null));
```

Enter fullscreen mode

Exit fullscreen mode

_Using ES6 Modules_\

```{.highlight .javascript}
import Helpers from '.helpers.js'
console.log(Helpers.isNull(null));
```

Enter fullscreen mode

Exit fullscreen mode

This is the basics of using **ES6 Modules**. I won't explain all about
Modules because it's a broad topic and my Post is now really long.

### [](#48-what-is-the-set-object-and-how-does-it-work) 48. What is the `Set` object and how does it work?

[↑](#the-questions) The **Set** object is an **ES6** feature that lets
you store unique values, **primitives** or **object references**. A
value in a Set can only occur **once**. It checks if a value exists in
the set object using the **SameValueZero** algorithm.

We can make `Set` instance using `Set` constructor and we can optionally
pass an `Iterable` as the initial value.\

```{.highlight .javascript}
const set1 = new Set();
const set2 = new Set(["a","b","c","d","d","e"]);
```

Enter fullscreen mode

Exit fullscreen mode

We can add a new value into the `Set` instance using the `add` method
and since the `add` returns the `Set` object we can chain `add` calls.
If a value already exists in `Set` object it will not be added again.\

```{.highlight .javascript}
set2.add("f");
set2.add("g").add("h").add("i").add("j").add("k").add("k");
// the last "k" will not be added to the set object because it already exists
```

Enter fullscreen mode

Exit fullscreen mode

We can remove a value from the `Set` instance using the `delete` method,
this method returns a `boolean` indicating `true` if a value exists in
the `Set` object and `false` indicating that value does not exist.\

```{.highlight .javascript}
set2.delete("k") // returns true because "k" exists in the set object
set2.delete("z") // returns false because "z" does not exists in the set object
```

Enter fullscreen mode

Exit fullscreen mode

We can check if a specific value exists in the `Set` instance using the
`has` method.\

```{.highlight .javascript}
set2.has("a") // returns true because "a" exists in the set object
set2.has("z") // returns false because "z" does not exists in the set object
```

Enter fullscreen mode

Exit fullscreen mode

We can get the length of the `Set` instance using the `size` property.\

```{.highlight .javascript}
set2.size // returns 10
```

Enter fullscreen mode

Exit fullscreen mode

We can delete or remove all the elements in the `Set` instance using the
`clear`.\

```{.highlight .javascript}
set2.clear(); // clears the set data
```

Enter fullscreen mode

Exit fullscreen mode

We can use the `Set` object for removing duplicate elements in an
array.\

```{.highlight .javascript}
const numbers = [1, 2, 3, 4, 5, 6, 6, 7, 8, 8, 5];
const uniqueNums = [...new Set(numbers)]; // has a value of [1,2,3,4,5,6,7,8]
```

Enter fullscreen mode

Exit fullscreen mode

### [](#49-what-is-a-callback-function) 49. What is a Callback function?

[↑](#the-questions) A **Callback** function is a function that is gonna
get called at a later point in time.\

```{.highlight .javascript}
const btnAdd = document.getElementById('btnAdd');

btnAdd.addEventListener('click', function clickCallback(e) {
    // do something useless
});
```

Enter fullscreen mode

Exit fullscreen mode

In this example, we wait for the `click event` in the element with an id
of **btnAdd**, if it is `clicked`, the `clickCallback` function is
executed. A **Callback** function adds some functionality to some data
or event. The `reduce`, `filter` and `map` methods in **Array** expects
a callback as a parameter. A good analogy for a callback is when you
call someone and if they don't answer you leave a message and you expect
them to **callback**. The act of calling someone or leaving a
**message** is the **event or data** and the **callback** is the
**action that you expect to occur later**.

### [](#50-what-are-promises) 50. What are **Promises**?

[↑](#the-questions) **Promises** are one way in handling asynchronous
operations in **JavaScript**. It represents the value of an asynchronous
operation. **Promises** was made to solve the problem of doing and
dealing with async code before promises we're using callbacks.\

```{.highlight .javascript}
fs.readFile('somefile.txt', function (e, data) {
  if (e) {
    console.log(e);
  }
  console.log(data);
});
```

Enter fullscreen mode

Exit fullscreen mode

The problem with this approach if we have another async operation inside
the callback and another. We will have a code that is messy and
unreadable. This code is called **Callback Hell**.\

```{.highlight .javascript}
//Callback Hell yucksss
fs.readFile('somefile.txt', function (e, data) {
  //your code here
  fs.readdir('directory', function (e, files) {
    //your code here
    fs.mkdir('directory', function (e) {
      //your code here
    })
  })
})
```

Enter fullscreen mode

Exit fullscreen mode

If we use promises in this code it will be more readable and easy to
understand and easy to maintain.\

```{.highlight .javascript}
promReadFile('file/path')
  .then(data => {
    return promReaddir('directory');
  })
  .then(data => {
    return promMkdir('directory');
  })
  .catch(e => {
    console.log(e);
  })
```

Enter fullscreen mode

Exit fullscreen mode

Promises have 3 different states.

**Pending** - The initial state of a promise. The promise's outcome has
not yet been known because the operation has not been completed yet.

**Fulfilled** - The async operation is completed and successful with the
resulting value.

**Rejected** - The async operation has failed and has a _reason_ on why
it failed.

**Settled** - If the promise has been either **Fulfilled** or
**Rejected**.

The **Promise** constructor has two parameters which are functions
`resolve` and `reject` respectively.\
 If the async operation has been completed without errors call the
`resolve` function to resolve the promise or if an error occurred \
 call the `reject` function and pass the error or reason to it.\
 We can access the result of the fulfilled promise using the `.then`\
 method and we catch errors in the `.catch` method. We chain multiple
async promise operations in the `.then` method because the `.then`
method returns a **Promise** just like the example in the imag e above.\

```{.highlight .javascript}
const myPromiseAsync = (...args) => {
  return new Promise((resolve, reject) => {
    doSomeAsync(...args, (error, data) => {
      if (error) {
        reject(error);
      } else {
        resolve(data);
      }
    })
  })
}

myPromiseAsync()
  .then(result => {
    console.log(result);
  })
  .catch(reason => {
    console.log(reason);
  })
```

Enter fullscreen mode

Exit fullscreen mode

We can make a helper func that converts an async operation with a
callback to promise. It works like the **promisify** utility function
from the node core module `util`.\

```{.highlight .javascript}
const toPromise = (asyncFuncWithCallback) => {
  return (...args) => {
    return new Promise((res, rej) => {
      asyncFuncWithCallback(...args, (e, result) => {
        return e ? rej(e) : res(result);
      });
    });
  }
}

const promReadFile = toPromise(fs.readFile);

promReadFile('file/path')
  .then((data) => {
    console.log(data);
  })
  .catch(e => console.log(e));
```

Enter fullscreen mode

Exit fullscreen mode

### [](#51-what-is-asyncawait-and-how-does-it-work) 51. What is _async/await_ and How does it work?

[↑](#the-questions) _async/await_ is the new way of writing asynchronous
or non-blocking code in **JavaScript's**. It is built on top of
**Promises**. It makes writing asynchronous code more readable and
cleaner than \
 **[Promises](#50-what-are-promises)** and
**[Callbacks](#49-what-is-a-callback-function)**. But you must learn the
basics of **Promises** before using this feature because as I said
earlier it is built on top of **Promises** which means is still uses
**Promises** under the hood.

Using Promises.\

```{.highlight .javascript}
function callApi() {
  return fetch("url/to/api/endpoint")
    .then(resp => resp.json())
    .then(data => {
      //do something with "data"
    }).catch(err => {
      //do something with "err"
    });
}
```

Enter fullscreen mode

Exit fullscreen mode

Using Async/Await.

**Note**: We're using the old _try/catch_ statement to **catch** any
errors that happened in any of those async operations inside the _try_
statement.\

```{.highlight .javascript}
async function callApi() {
  try {
    const resp = await fetch("url/to/api/endpoint");
    const data = await resp.json();
    //do something with "data"
  } catch (e) {
    //do something with "err"
  }
}
```

Enter fullscreen mode

Exit fullscreen mode

**Note**: The _async_ keyword before the function declaration makes the
function return _implicitly_ a **Promise**.\

```{.highlight .javascript}
const giveMeOne = async () => 1;

giveMeOne()
  .then((num) => {
    console.log(num); // logs 1
  });
```

Enter fullscreen mode

Exit fullscreen mode

**Note**: The _await_ keyword can **only** be used inside an **async
function**. Using _await_ keyword in any other function which is not an
**async function** will throw an error. The _await_ keyword **awaits**
the right-hand side expression (presumably a **Promise**) to return
before executing the next line of code.\

```{.highlight .javascript}
const giveMeOne = async () => 1;

function getOne() {
  try {
    const num = await giveMeOne();
    console.log(num);
  } catch (e) {
    console.log(e);
  }
}

//Throws a Compile-Time Error = Uncaught SyntaxError: await is only valid in an async function

async function getTwo() {
  try {
    const num1 = await giveMeOne(); //finishes this async operation first before going to
    const num2 = await giveMeOne(); //this line
    return num1 + num2;
  } catch (e) {
    console.log(e);
  }
}

await getTwo(); // returns 2
```

Enter fullscreen mode

Exit fullscreen mode

### [](#52-whats-the-difference-between-spread-operator-and-rest-operator) 52. What's the difference between **Spread operator** and **Rest operator**?

[↑](#the-questions) The **Spread operator** and **Rest paremeters** have
the same operator `...` the difference between is that the **Spread
operator** we **give** or **spread** individual data of an array to
another data while the **Rest parameters** is used in a function or an
array to **get** all the arguments or values and put them in an array or
**extract** some pieces of them.\

```{.highlight .javascript}
function add(a, b) {
  return a + b;
};

const nums = [5, 6];
const sum = add(...nums);
console.log(sum);
```

Enter fullscreen mode

Exit fullscreen mode

In this example, we're using the **Spread Operator** when we call the
`add` function we are **spreading** the `nums` array. So the value of
parameter `a` will be **5** and the value of `b` will be **6**. So the
sum will be **11**.\

```{.highlight .javascript}
function add(...rest) {
  return rest.reduce((total,current) => total + current);
};

console.log(add(1, 2)); // logs 3
console.log(add(1, 2, 3, 4, 5)); // logs 15
```

Enter fullscreen mode

Exit fullscreen mode

In this example, we have a function `add` that accepts any number of
arguments and adds them all and return the total.\

```{.highlight .javascript}
const [first, ...others] = [1, 2, 3, 4, 5];
console.log(first); //logs 1
console.log(others); //logs [2,3,4,5]
```

Enter fullscreen mode

Exit fullscreen mode

In this another example, we are using the **Rest operator** to extract
all the remaining array values and put them in array `others` except the
first item.

### [](#53-what-are-default-parameters) 53. What are **Default Parameters**?

[↑](#the-questions) **Default Parameters** is a new way of defining
default variables in **JavaScript** it is available in the **ES6** or
**ECMAScript 2015** Version.\

```{.highlight .javascript}
//ES5 Version
function add(a,b){
  a = a || 0;
  b = b || 0;
  return a + b;
}

//ES6 Version
function add(a = 0, b = 0){
  return a + b;
}
//If we don't pass any argument for 'a' or 'b' then
// it's gonna use the "default parameter" value which is 0
add(1); // returns 1
```

Enter fullscreen mode

Exit fullscreen mode

We can also use **[Destructuring](#46-what-is-object-destructuring)** in
**Default Paremeters**.\

```{.highlight .javascript}
function getFirst([first, ...rest] = [0, 1]) {
  return first;
}

getFirst();  // returns 0
getFirst([10,20,30]);  // returns 10

function getArr({ nums } = { nums: [1, 2, 3, 4] }){
    return nums;
}

getArr(); // returns [1, 2, 3, 4]
getArr({nums:[5,4,3,2,1]}); // returns [5,4,3,2,1]
```

Enter fullscreen mode

Exit fullscreen mode

We can also use the parameters defined first to the parameters defined
after them.\

```{.highlight .javascript}
function doSomethingWithValue(value = "Hello World", callback = () => { console.log(value) }) {
  callback();
}
doSomethingWithValue(); //logs "Hello World"
```

Enter fullscreen mode

Exit fullscreen mode

### [](#54-what-are-wrapper-objects) 54. What are **Wrapper Objects**?

[↑](#the-questions) **Primitive Values** like `string`,`number` and
`boolean` with the exception of `null` and `undefined` have properties
and methods even though they are not `objects`.\

```{.highlight .javascript}
let name = "marko";

console.log(typeof name); // logs  "string"
console.log(name.toUpperCase()); // logs  "MARKO"
```

Enter fullscreen mode

Exit fullscreen mode

`name` is a `primitive string` value that has no properties and methods
but in this example we are calling a `toUpperCase()` method which does
not throw an error but returns `MARKO`.

The reason for this is that the `primitive` value is temporarily
converted or _coerce_ to an `object` so the `name` variable behaves like
an `object`. Every `primitive` except `null` and `undefined` have
**Wrapper Objects**. The Wrapper Objects are
`String`,`Number`,`Boolean`,`Symbol` and `BigInt`. In this case, the
`name.toUpperCase()` invocation, behind the scenes it looks like this.\

```{.highlight .javascript}
console.log(new String(name).toUpperCase()); // logs  "MARKO"
```

Enter fullscreen mode

Exit fullscreen mode

The newly created object is immediately discarded after we finished
accessing a property or calling a method.

### [](#55-what-is-the-difference-between-implicit-and-explicit-coercion) 55. What is the difference between **Implicit** and **Explicit** Coercion?

[↑](#the-questions) **Implicit** Coercion is a way of converting values
to another type without us programmer doing it directly or by hand.

Suppose we have an example below.\

```{.highlight .javascript}
console.log(1 + '6');
console.log(false + true);
console.log(6 * '2');
```

Enter fullscreen mode

Exit fullscreen mode

The **first** `console.log` statement logs `16`. In other languages this
would throw a compile time error but in **JavaScript** the `1` is
converted to a `string` then concatenated with the `+` operator. We did
not do anything, yet it was converted automatically by **JavaScript**
for us. \
 The **second** `console.log` statement logs `1`, it converts the
`false` to a `boolean` which will result to a `0` and the `true` will be
`1` hence the result is `1`. \
 The **third** `console.log` statement logs `12`, it converts the `'2'`
to a `number` before multiplying `6 * 2` hence the result `12`.\
 [JavaScript Coercion
Rules](https://delapouite.com/ramblings/javascript-coercion-rules.html)

While **Explicit** Coercion is the way of converting values to another
type where we (_programmers_) **explicitly** do it.\

```{.highlight .javascript}
console.log(1 + parseInt('6'));
```

Enter fullscreen mode

Exit fullscreen mode

In this example, we use the `parseInt` function to convert the `'6'` to
a `number` then adding the `1` and `6` using the `+` operator.

### [](#56-what-is-nan-and-how-to-check-if-a-value-is-nan) 56. What is `NaN`? and How to check if a value is `NaN`?

[↑](#the-questions) `NaN` means **"Not A Number"** is a value in
**JavaScript** that is a result in converting or performing an operation
to a number to non-number value hence results to `NaN`.\

```{.highlight .javascript}
let a;

console.log(parseInt('abc'));
console.log(parseInt(null));
console.log(parseInt(undefined));
console.log(parseInt(++a));
console.log(parseInt({} * 10));
console.log(parseInt('abc' - 2));
console.log(parseInt(0 / 0));
console.log(parseInt('10a' * 10));
```

Enter fullscreen mode

Exit fullscreen mode

**JavaScript** has a built-in method `isNaN` that tests if value is
`isNaN` value. But this function has a weird behaviour.\

```{.highlight .javascript}
console.log(isNaN()); //logs true
console.log(isNaN(undefined)); //logs true
console.log(isNaN({})); //logs true
console.log(isNaN(String('a'))); //logs true
console.log(isNaN(() => { })); //logs true
```

Enter fullscreen mode

Exit fullscreen mode

All these `console.log` statements return `true` even though those
values we pass are not `NaN`.

In **ES6** or **ECMAScript 2015**, it is recommended that we use
`Number.isNaN` method because it really checks the value if it really is
`NaN` or we can make our own helper function that check for this problem
because in **JavaScript** `NaN` is the only value that is not equal to
itself.\

```{.highlight .javascript}
function checkIfNaN(value) {
  return value !== value;
}
```

Enter fullscreen mode

Exit fullscreen mode

### [](#57-how-to-check-if-a-value-is-an-array) 57. How to check if a value is an **Array**?

[↑](#the-questions) We can check if a value is an **Array** by using the
`Array.isArray` method available from the **Array** global object. It
returns true when the parameter pass to it is an **Array** otherwise
false.\

```{.highlight .javascript}
console.log(Array.isArray(5));  //logs false
console.log(Array.isArray("")); //logs false
console.log(Array.isArray()); //logs false
console.log(Array.isArray(null)); //logs false
console.log(Array.isArray({ length: 5 })); //logs false

console.log(Array.isArray([])); //logs true
```

Enter fullscreen mode

Exit fullscreen mode

If your environment does not support this method you can use the
polyfill implementation.\

```{.highlight .javascript}
   function isArray(value){
     return Object.prototype.toString.call(value) === "[object Array]"
   }
```

Enter fullscreen mode

Exit fullscreen mode

### [](#58-how-to-check-if-a-number-is-even-without-using-the-or-modulo-operator) 58. How to check if a number is even without using the `%` or modulo operator?

[↑](#the-questions) We can use the **bitwise AND**`&` operator for this
problem. The `&` operates on its operand and treats them as binary
values and performs the **AND** operation.\

```{.highlight .javascript}
function isEven(num) {
  if (num & 1) {
    return false;
  } else {
    return true;
  }
};
```

Enter fullscreen mode

Exit fullscreen mode

`0` in binary is **000**.\
 `1` in binary is **001**.\
 `2` in binary is **010**.\
 `3` in binary is **011**.\
 `4` in binary is **100**.\
 `5` in binary is **101**.\
 `6` in binary is **110**.\
 `7` in binary is **111**.\
 and so on...

`a` `b` `a & b`

---

0 0 0
0 1 0
1 0 0
1 1 1

So when we `console.log` this expression `5 & 1` it returns `1`. Ok,
first the `&` operator converts both numbers to binary so `5` turns to
**101** and `1` turns to **001**. \
 Then it compares every bit **(0's and 1's)** using the bitwise **AND**
operator. **101** `&` **001**. As we can see from the table the result
can be only `1` if `a` **AND** `b` are `1`.

`101 & 001`

---

101
001
**001**

- So first we compare the left most bit ` 1``&``0 ` the result should be
  `0`.
- Then we compare the middle bit ` 0``&``0 ` the result should be `0`.
- Then we compare the last bit ` 1``&``1 ` the result should be `1`.
- Then the binary result `001` will be converted to a decimal number
  which will be `1`.

If we `console.log` this expression `4 & 1` it will return `0`. Knowing
the last bit of `4` is `0` and `0 & 1` will be `0`. If you have a hard
time understand this we could use a **recursive** function to solve this
problem.\

```{.highlight .javascript}
function isEven(num) {
  if (num < 0 || num === 1) return false;
  if (num == 0) return true;
  return isEven(num - 2);
}
```

Enter fullscreen mode

Exit fullscreen mode

### [](#59-how-to-check-if-a-certain-property-exists-in-an-object) 59. How to check if a certain property exists in an object?

[↑](#the-questions) There are three possible ways to check if a property
exists in an object.

First , using the `in` operator. The syntax for using the `in` operator
is like this `propertyname in object`. It returns `true` if the property
exists otherwise it returns `false`.\

```{.highlight .javascript}
const o = {
  "prop" : "bwahahah",
  "prop2" : "hweasa"
};

console.log("prop" in o); //This logs true indicating the property "prop" is in "o" object
console.log("prop1" in o); //This logs false indicating the property "prop" is not in  "o" object
```

Enter fullscreen mode

Exit fullscreen mode

Second, using the `hasOwnProperty` method in objects. This method is
available on all objects in JavaScript. It returns `true` if the
property exists otherwise it returns `false`.\

```{.highlight .javascript}
//Still using the o object in the first example.
console.log(o.hasOwnProperty("prop2")); // This logs true
console.log(o.hasOwnProperty("prop1")); // This logs false
```

Enter fullscreen mode

Exit fullscreen mode

Third, using the bracket notation `obj["prop"]`. If the property exists
it returns the value of that property otherwise this will return
`undefined`.\

```{.highlight .javascript}
//Still using the o object in the first example.
console.log(o["prop"]); // This logs "bwahahah"
console.log(o["prop1"]); // This logs undefined
```

Enter fullscreen mode

Exit fullscreen mode

### [](#60-what-is-ajax) 60. What is **AJAX**?

[↑](#the-questions) **AJAX** stands for **Asynchronous JavaScript and
XML**. It is a group of related technologies used to display data
asynchronously. What this means is that we can send data to the server
and get data from the server without reloading the web page.

Technologies use for **AJAX**.

- **HTML** - web page structure
- **CSS** - the styling for the webpage
- **JavaScript** - the behaviour of the webpage and updates to the
  **DOM**
- **XMLHttpRequest API** - used to send and retrieve data from the
  server
- **PHP,Python,Nodejs** - Some Server-Side language

### [](#61-what-are-the-ways-of-making-objects-in-javascript) 61. What are the ways of making objects in JavaScript?

[↑](#the-questions) Using **Object Literal**.\

```{.highlight .javascript}
  const o = {
   name: "Mark",
   greeting() {
      return `Hi, I'm ${this.name}`;
   }
  };

  o.greeting(); //returns "Hi, I'm Mark"
```

Enter fullscreen mode

Exit fullscreen mode

Using **Constructor Functions**.\

```{.highlight .javascript}
function Person(name) {
   this.name = name;
}

Person.prototype.greeting = function () {
   return `Hi, I'm ${this.name}`;
}

const mark = new Person("Mark");

mark.greeting(); //returns "Hi, I'm Mark"
```

Enter fullscreen mode

Exit fullscreen mode

Using **Object.create** method.\

```{.highlight .javascript}
const n = {
   greeting() {
      return `Hi, I'm ${this.name}`;
   }
};

const o = Object.create(n); // sets the prototype of "o" to be "n"

o.name = "Mark";

console.log(o.greeting()); // logs "Hi, I'm Mark"

```

Enter fullscreen mode

Exit fullscreen mode

### [](#62-whats-the-difference-between-objectseal-and-objectfreeze-methods) 62. What's the difference between `Object.seal` and `Object.freeze` methods?

[↑](#the-questions) The difference between these two methods is that
when we use the `Object.freeze` method to an object, that object's
properties are immutable meaning we can't change or edit the values of
those properties. While in the `Object.seal` method we can change those
existing properties but we cannot add new properties to the object.

### [](#63-whats-the-difference-between-the-in-operator-and-the-hasownproperty-method-in-objects) 63. What's the difference between the `in` operator and the `hasOwnProperty` method in objects?

[↑](#the-questions) As you know both of these features check if a
property exists in an object. It will return `true`false. The difference
between them is that the `in` operator also checks the objects'
**Prototype Chain** if the property was not found in the current object
while the `hasOwnProperty` method just checks if the property exists in
the current object ignoring the **Prototype Chain**.\

```{.highlight .javascript}
// We'll still use the object in the previous question.
console.log("prop" in o); // This logs true;
console.log("toString" in o); // This logs true, the toString method is available in this object's prototype which is the Object.prototype


console.log(o.hasOwnProperty("prop")); // This logs true
console.log(o.hasOwnProperty("toString")); // This logs false, does not check the object's prototype
```

Enter fullscreen mode

Exit fullscreen mode

### [](#64-what-are-the-ways-to-deal-with-asynchronous-code-in-javasscript) 64. What are the ways to deal with **Asynchronous Code** in JavasScript?

[↑](#the-questions)

- [Callbacks](#49-what-is-a-callback-function)
- [Promises](#50-what-are-promises)
- [async/await](#51-what-is-asyncawait-and-how-does-it-work)
- Libraries like [async.js](https://caolan.github.io/async/v3/),
  [bluebird](http://bluebirdjs.com/docs/getting-started.html),
  [q](http://documentup.com/kriskowal/q/),
  [co](https://www.npmjs.com/package/co)

### [](#65-whats-the-difference-between-a-function-expression-and-function-declaration) 65. What's the difference between a **function expression** and **function declaration**?

[↑](#the-questions) Suppose we have an example below.\

```{.highlight .javascript}
hoistedFunc();
notHoistedFunc();

function hoistedFunc(){
  console.log("I am hoisted");
}

var notHoistedFunc = function(){
  console.log("I will not be hoisted!");
}
```

Enter fullscreen mode

Exit fullscreen mode

The `notHoistedFunc` call throws an error while the `hoistedFunc` call
does not because the `hoistedFunc` is _hoisted_ while the
`notHoistedFunc` is not. \
 Read **Hoisting** [here](#18-what-is-hoisting).

### [](#66-how-many-ways-can-a-function-be-invoked) 66. How many ways can a function be _invoked_?

[↑](#the-questions) There are 4 ways that a function can be _invoked_ in
**JavaScript**. The **invocation** determines the value of `this` or the
"owner" object of that function.

- **Invocation as a function** - If a function isn't invoked as a
  method, as a constructor or with the `apply`, `call` methods then it
  is **invoked as a function**. The "owner" object of this function
  will be the `window` object.

```{.highlight .javascript}
  //Global Scope

  function add(a,b){
    console.log(this);
    return a + b;
  }

  add(1,5); // logs the "window" object and returns 6

  const o = {
    method(callback){
      callback();
    }
  }

  o.method(function (){
      console.log(this); // logs the "window" object
  });
```

Enter fullscreen mode

Exit fullscreen mode

- **Invocation as a method** - If a property of an object has a value
  of a function we call it a **method**. When that **method** is
  _invoked_ the `this` value of that method will be that object.

```{.highlight .javascript}
   const details = {
     name : "Marko",
     getName(){
       return this.name;
     }
   }

   details.getName(); // returns Marko
   // the "this" value inside "getName" method will be the "details" object
```

Enter fullscreen mode

Exit fullscreen mode

- **Invocation as a constructor** - If a function was _invoked_ with a
  `new` keyword before it then it's called a `function constructor`.
  An empty object will be created and `this` will point to that
  object.

```{.highlight .javascript}
function Employee(name, position, yearHired) {
  // creates an empty object {}
  // then assigns the empty object to the "this" keyword
  // this = {};
  this.name = name;
  this.position = position;
  this.yearHired = yearHired;
  // inherits from Employee.prototype
  // returns the "this" value implicitly if no
  // explicit return statement is specified
};

const emp = new Employee("Marko Polo", "Software Developer", 2017);
```

Enter fullscreen mode

Exit fullscreen mode

- **Invocation with the `apply` and `call` methods** - If we want to
  _explicitly_ specify the `this` value or the "owner" object of a
  function we can use these methods. These methods are available for
  all functions.

```{.highlight .javascript}
const obj1 = {
 result:0
};

const obj2 = {
 result:0
};


function reduceAdd(){
   let result = 0;
   for(let i = 0, len = arguments.length; i < len; i++){
     result += arguments[i];
   }
   this.result = result;
}


reduceAdd.apply(obj1, [1, 2, 3, 4, 5]);  //the "this" object inside the "reduceAdd" function will be "obj1"
reduceAdd.call(obj2, 1, 2, 3, 4, 5); //the "this" object inside the "reduceAdd" function will be "obj2"
```

Enter fullscreen mode

Exit fullscreen mode

### [](#67-what-is-memoization-and-whats-the-use-it) 67. What is _memoization_ and what's the use it?

[↑](#the-questions) _memoization_ is a process of building a function
that is capable of **remembering** it's previously computed results or
values. \
 The use of making a _memoization_ function is that we avoid the
computation of that function if it was already performed in the last
calculations with the same arguments. This saves time but has a downside
that we will consume more memory for saving the previous results.

### [](#68-implement-a-memoization-helper-function) 68. Implement a memoization helper function.

[↑](#the-questions)\

```{.highlight .javascript}
function memoize(fn) {
  const cache = {};
  return function (param) {
    if (cache[param]) {
      console.log('cached');
      return cache[param];
    } else {
      let result = fn(param);
      cache[param] = result;
      console.log(`not cached`);
      return result;
    }
  }
}

const toUpper = (str ="")=> str.toUpperCase();

const toUpperMemoized = memoize(toUpper);

toUpperMemoized("abcdef");
toUpperMemoized("abcdef");
```

Enter fullscreen mode

Exit fullscreen mode

This _memoize_ helper function only works on a function that accepts one
_argument_. We need to make a _memoize_ helper function that accepts
multiple _arguments_.\

```{.highlight .javascript}
const slice = Array.prototype.slice;
function memoize(fn) {
  const cache = {};
  return (...args) => {
    const params = slice.call(args);
    console.log(params);
    if (cache[params]) {
      console.log('cached');
      return cache[params];
    } else {
      let result = fn(...args);
      cache[params] = result;
      console.log(`not cached`);
      return result;
    }
  }
}
const makeFullName = (fName, lName) => `${fName} ${lName}`;
const reduceAdd = (numbers, startingValue = 0) => numbers.reduce((total, cur) => total + cur, startingValue);

const memoizedMakeFullName = memoize(makeFullName);
const memoizedReduceAdd = memoize(reduceAdd);

memoizedMakeFullName("Marko", "Polo");
memoizedMakeFullName("Marko", "Polo");

memoizedReduceAdd([1, 2, 3, 4, 5], 5);
memoizedReduceAdd([1, 2, 3, 4, 5], 5);
```

Enter fullscreen mode

Exit fullscreen mode

### [](#69-why-does-typeof-null-return-object-how-to-check-if-a-value-is-null) 69. Why does `typeof null` return `object`? How to check if a value is `null`?

[↑](#the-questions) `typeof null == 'object'` will always return `true`
because this was the implementation of `null` since the birth of
**JavaScript**. A fix was proposed to change `typeof null == 'object'`
to `typeof null == 'null'` but was
[rejected](https://web.archive.org/web/20160331031419/http://wiki.ecmascript.org:80/doku.php?id=harmony:typeof_null)
because it will lead to more bugs.

We can use the `===` or **strict equality** operator to check if a value
is `null`.\

```{.highlight .javascript}
  function isNull(value){
    return value === null;
  }
```

Enter fullscreen mode

Exit fullscreen mode

### [](#70-what-does-the-new-keyword-do) 70. What does the `new` keyword do?

[↑](#the-questions) The `new` keyword is used with _constructor_
functions to make objects \
 in **JavaScript**.

Suppose we have an example code below.\

```{.highlight .javascript}
function Employee(name, position, yearHired) {
  this.name = name;
  this.position = position;
  this.yearHired = yearHired;
};

const emp = new Employee("Marko Polo", "Software Developer", 2017);
```

Enter fullscreen mode

Exit fullscreen mode

The `new` keyword does 4 things.

- Creates an empty object.
- Assigns that empty object to the `this` value.
- The function will _inherit_ from
  **functionName.[prototype](#25-what-is-the-prototype-of-an-object)**.
- Returns the `this` if no Explicit `return` statement is used.

In the above image, it will first create an empty object `{}` then \
 it will the `this` value to that empty object `this = {}` and add
properties to that `this` object. Because we don't have a explicit
`return` statement it automatically returns the `this` for us.

## [](#thanks-guys-for-reading-this-post) Thanks guys for reading this post.

# [](#have-a-nice-day-smiley-and-a-happy-new-year-fireworksfireworksfireworks) Have a Nice Day 😃 and a Happy New Year 🎆🎆🎆.

## Discussion (94) {.crayons-subtitle-1}

Subscribe

![pic](https://res.cloudinary.com/practicaldev/image/fetch/s--RmY55OKL--/c_limit,f_auto,fl_progressive,q_auto,w_256/https://practicaldev-herokuapp-com.freetls.fastly.net/assets/devlogo-pwa-512.png)

Upload image

Templates

[](/p/editor_guide "Markdown Guide")

Editor guide

Personal

Moderator

![loading](https://dev.to/assets/loading-ellipsis-b714cf681fd66c853ff6f03dd161b77aa3c80e03cdc06f478b695f42770421e9.svg)

[Create template](/settings/response-templates)

Templates let you quickly answer FAQs or store snippets for re-use.

Submit

Preview

[Dismiss](/404.html)

Collapse

Expand

[![sebbdk profile
image](https://res.cloudinary.com/practicaldev/image/fetch/s--3WpRI1to--/c_fill,f_auto,fl_progressive,h_50,q_auto,w_50/https://dev-to-uploads.s3.amazonaws.com/uploads/user/profile_image/162707/ec9d10df-acbb-4827-816e-6e4706275a32.png)](https://dev.to/sebbdk)

[Sebastian Vargr](https://dev.to/sebbdk)

Sebastian Vargr

[![](https://res.cloudinary.com/practicaldev/image/fetch/s--SVCa3-iN--/c_fill,f_auto,fl_progressive,h_90,q_auto,w_90/https://dev-to-uploads.s3.amazonaws.com/uploads/user/profile_image/162707/ec9d10df-acbb-4827-816e-6e4706275a32.png)
Sebastian Vargr](/sebbdk)

I find broken' code and fix it. Sometimes it even works after i am done.

Follow

- Work
  McGuffin maker, Senior team lead, rubber duck
- Location
  Hiding in your closet
- Joined
  May 1, 2019

• [Jan 3 '20 • Edited on Jan 3](https://dev.to/sebbdk/comment/jkg9)

Dropdown menu

- [Copy link](https://dev.to/sebbdk/comment/jkg9)
- - [Hide](#)

---

It's funny how interviews often focus on memorization these kind of
things, which are the easiest things to look up when you need them.

Half of these things i encountered and used without' having to know the
right name for what i was doing, so whats the value?

Very rarely do i get asked about my thoughts on MVC, component
orchestration, function vs Class based programming, what
over-engineering is, interesting problems i have solved and how, or just
maybe how i handle differences of opinion in PR's.

Comparatively speaking, having those kinds of discussions seem much more
relevant than whether or not i have memorized all the latest programmer
pop culture and random terms one might use once every blue moon.

---

That being said.

This is a nice list to memorize if you wanna play the default interview
game.\
 Which i might in the future, so thanks! :)

Favorite heart outline button

Favorite heart outline button

19 likes

[](#/macmacky/70-javascript-interview-questions-5gfi/comments/new/jkg9)

Comment button

Reply

Collapse

Expand

[![macmacky profile
image](https://res.cloudinary.com/practicaldev/image/fetch/s--ip3rQvUF--/c_fill,f_auto,fl_progressive,h_50,q_auto,w_50/https://dev-to-uploads.s3.amazonaws.com/uploads/user/profile_image/201157/3607fd1f-3a5f-4fdf-8421-01debc8523b7.jpg)](https://dev.to/macmacky)

[Mark A](https://dev.to/macmacky)

Author

Mark A

[![](https://res.cloudinary.com/practicaldev/image/fetch/s--11luy8FC--/c_fill,f_auto,fl_progressive,h_90,q_auto,w_90/https://dev-to-uploads.s3.amazonaws.com/uploads/user/profile_image/201157/3607fd1f-3a5f-4fdf-8421-01debc8523b7.jpg)
Mark A](/macmacky)

a Full-Stack developer who likes reading Tom Clancy's books and loves
talking with dogs.

Follow

- Work
  Software Engineer
- Location
  Cebu City
- Education
  Bachelor's Degree in Computer Engineering
- Joined
  Jul 24, 2019

Author

• [Jan 3 '20](https://dev.to/macmacky/comment/jko1)

Dropdown menu

- [Copy link](https://dev.to/macmacky/comment/jko1)
- - [Hide](#)

---

I feel you man but most of the time memorizing or knowing this things
are not about answering an Interview problem or problems but solving a
problem you are having with JavaScript and btw Glad you like it!!!

Favorite heart outline button

Favorite heart outline button

7 likes

[](#/macmacky/70-javascript-interview-questions-5gfi/comments/new/jko1)

Comment button

Reply

Collapse

Expand

[![greatgraphicdesign profile
image](https://res.cloudinary.com/practicaldev/image/fetch/s--CicAvgy9--/c_fill,f_auto,fl_progressive,h_50,q_auto,w_50/https://dev-to-uploads.s3.amazonaws.com/uploads/user/profile_image/308059/d96ff35d-3f2a-4ddd-974e-0337d35b9bd3.jpeg)](https://dev.to/greatgraphicdesign)

[Alek Vila](https://dev.to/greatgraphicdesign)

Alek Vila

[![](https://res.cloudinary.com/practicaldev/image/fetch/s--zRvuJGPs--/c_fill,f_auto,fl_progressive,h_90,q_auto,w_90/https://dev-to-uploads.s3.amazonaws.com/uploads/user/profile_image/308059/d96ff35d-3f2a-4ddd-974e-0337d35b9bd3.jpeg)
Alek Vila](/greatgraphicdesign)

Art Director, Graphic Designer, Front End Web-Developer

Follow

- Location
  Bellingham, WA
- Joined
  Jan 4, 2020

• [May 1 '20](https://dev.to/greatgraphicdesign/comment/ocmd)

Dropdown menu

- [Copy link](https://dev.to/greatgraphicdesign/comment/ocmd)
- - [Hide](#)

---

Regarding Question 24, I want to really understand "this" so I tested
each example in the Console. I found a different result than what you
shared for this line...

`myFavoriteObj.guessThis();`

You wrote that it logs the window object; however, I'm seeing that in
normal mode it logs nothing and in strict mode it throws an error. Maybe
it is working differently on your browser? I'm using Chrome 81 on Mac.

By the way, I am enjoying studying this post. Thank you!

Favorite heart outline button

Favorite heart outline button

8 likes

[](#/macmacky/70-javascript-interview-questions-5gfi/comments/new/ocmd)

Comment button

Reply

Collapse

Expand

[![macmacky profile
image](https://res.cloudinary.com/practicaldev/image/fetch/s--ip3rQvUF--/c_fill,f_auto,fl_progressive,h_50,q_auto,w_50/https://dev-to-uploads.s3.amazonaws.com/uploads/user/profile_image/201157/3607fd1f-3a5f-4fdf-8421-01debc8523b7.jpg)](https://dev.to/macmacky)

[Mark A](https://dev.to/macmacky)

Author

Mark A

[![](https://res.cloudinary.com/practicaldev/image/fetch/s--11luy8FC--/c_fill,f_auto,fl_progressive,h_90,q_auto,w_90/https://dev-to-uploads.s3.amazonaws.com/uploads/user/profile_image/201157/3607fd1f-3a5f-4fdf-8421-01debc8523b7.jpg)
Mark A](/macmacky)

a Full-Stack developer who likes reading Tom Clancy's books and loves
talking with dogs.

Follow

- Work
  Software Engineer
- Location
  Cebu City
- Education
  Bachelor's Degree in Computer Engineering
- Joined
  Jul 24, 2019

Author

• [May 2 '20](https://dev.to/macmacky/comment/od11)

Dropdown menu

- [Copy link](https://dev.to/macmacky/comment/od11)
- - [Hide](#)

---

Thanks, for finding my mistake. I edited it just now. No problem man,
glad you like it.

Favorite heart outline button

Favorite heart outline button

2 likes

[](#/macmacky/70-javascript-interview-questions-5gfi/comments/new/od11)

Comment button

Reply

Collapse

Expand

[![greatgraphicdesign profile
image](https://res.cloudinary.com/practicaldev/image/fetch/s--CicAvgy9--/c_fill,f_auto,fl_progressive,h_50,q_auto,w_50/https://dev-to-uploads.s3.amazonaws.com/uploads/user/profile_image/308059/d96ff35d-3f2a-4ddd-974e-0337d35b9bd3.jpeg)](https://dev.to/greatgraphicdesign)

[Alek Vila](https://dev.to/greatgraphicdesign)

Alek Vila

[![](https://res.cloudinary.com/practicaldev/image/fetch/s--zRvuJGPs--/c_fill,f_auto,fl_progressive,h_90,q_auto,w_90/https://dev-to-uploads.s3.amazonaws.com/uploads/user/profile_image/308059/d96ff35d-3f2a-4ddd-974e-0337d35b9bd3.jpeg)
Alek Vila](/greatgraphicdesign)

Art Director, Graphic Designer, Front End Web-Developer

Follow

- Location
  Bellingham, WA
- Joined
  Jan 4, 2020

• [May 2 '20](https://dev.to/greatgraphicdesign/comment/od14)

Dropdown menu

- [Copy link](https://dev.to/greatgraphicdesign/comment/od14)
- - [Hide](#)

---

Believe it or not, I'm still going through your list and taking notes.
This is a very cool post.

By the way, I've cleared my browser cache the graphic is the same. Maybe
it's cached on the server side?

Favorite heart outline button

Favorite heart outline button

2 likes

Thread

Thread

[![macmacky profile
image](https://res.cloudinary.com/practicaldev/image/fetch/s--ip3rQvUF--/c_fill,f_auto,fl_progressive,h_50,q_auto,w_50/https://dev-to-uploads.s3.amazonaws.com/uploads/user/profile_image/201157/3607fd1f-3a5f-4fdf-8421-01debc8523b7.jpg)](https://dev.to/macmacky)

[Mark A](https://dev.to/macmacky)

Author

Mark A

[![](https://res.cloudinary.com/practicaldev/image/fetch/s--11luy8FC--/c_fill,f_auto,fl_progressive,h_90,q_auto,w_90/https://dev-to-uploads.s3.amazonaws.com/uploads/user/profile_image/201157/3607fd1f-3a5f-4fdf-8421-01debc8523b7.jpg)
Mark A](/macmacky)

a Full-Stack developer who likes reading Tom Clancy's books and loves
talking with dogs.

Follow

- Work
  Software Engineer
- Location
  Cebu City
- Education
  Bachelor's Degree in Computer Engineering
- Joined
  Jul 24, 2019

Author

• [May 2 '20](https://dev.to/macmacky/comment/od1d)

Dropdown menu

- [Copy link](https://dev.to/macmacky/comment/od1d)
- - [Hide](#)

---

I've changed the object.

It looks like this now.\

```{.highlight .javascript}
 const myFavoriteObj = {
     guessThis(){
        function getThis(){
          console.log(this);
        }
        getThis();
     },
     name: 'Marko Polo',
     thisIsAnnoying(callback){
       callback();
     }
   };
```

\
 \`

Thanks

Favorite heart outline button

Favorite heart outline button

2 likes

Thread

Thread

[![greatgraphicdesign profile
image](https://res.cloudinary.com/practicaldev/image/fetch/s--CicAvgy9--/c_fill,f_auto,fl_progressive,h_50,q_auto,w_50/https://dev-to-uploads.s3.amazonaws.com/uploads/user/profile_image/308059/d96ff35d-3f2a-4ddd-974e-0337d35b9bd3.jpeg)](https://dev.to/greatgraphicdesign)

[Alek Vila](https://dev.to/greatgraphicdesign)

Alek Vila

[![](https://res.cloudinary.com/practicaldev/image/fetch/s--zRvuJGPs--/c_fill,f_auto,fl_progressive,h_90,q_auto,w_90/https://dev-to-uploads.s3.amazonaws.com/uploads/user/profile_image/308059/d96ff35d-3f2a-4ddd-974e-0337d35b9bd3.jpeg)
Alek Vila](/greatgraphicdesign)

Art Director, Graphic Designer, Front End Web-Developer

Follow

- Location
  Bellingham, WA
- Joined
  Jan 4, 2020

• [May 2 '20](https://dev.to/greatgraphicdesign/comment/od1f)

Dropdown menu

- [Copy link](https://dev.to/greatgraphicdesign/comment/od1f)
- - [Hide](#)

---

Ah, I see the change now. You removed `.name` from where it used to say
`console.log(this.name);` Thank you!

Favorite heart outline button

Favorite heart outline button

2 likes

Thread

Thread

[![macmacky profile
image](https://res.cloudinary.com/practicaldev/image/fetch/s--ip3rQvUF--/c_fill,f_auto,fl_progressive,h_50,q_auto,w_50/https://dev-to-uploads.s3.amazonaws.com/uploads/user/profile_image/201157/3607fd1f-3a5f-4fdf-8421-01debc8523b7.jpg)](https://dev.to/macmacky)

[Mark A](https://dev.to/macmacky)

Author

Mark A

[![](https://res.cloudinary.com/practicaldev/image/fetch/s--11luy8FC--/c_fill,f_auto,fl_progressive,h_90,q_auto,w_90/https://dev-to-uploads.s3.amazonaws.com/uploads/user/profile_image/201157/3607fd1f-3a5f-4fdf-8421-01debc8523b7.jpg)
Mark A](/macmacky)

a Full-Stack developer who likes reading Tom Clancy's books and loves
talking with dogs.

Follow

- Work
  Software Engineer
- Location
  Cebu City
- Education
  Bachelor's Degree in Computer Engineering
- Joined
  Jul 24, 2019

Author

• [May 2 '20](https://dev.to/macmacky/comment/od1h)

Dropdown menu

- [Copy link](https://dev.to/macmacky/comment/od1h)
- - [Hide](#)

---

Your welcome. Thanks, again for finding my mistake.

Favorite heart outline button

Favorite heart outline button

1 like

Thread

Thread

[![kuncheriakuruvilla profile
image](https://res.cloudinary.com/practicaldev/image/fetch/s--ZycSdFYW--/c_fill,f_auto,fl_progressive,h_50,q_auto,w_50/https://dev-to-uploads.s3.amazonaws.com/uploads/user/profile_image/316502/e0d2b6b0-2bc9-40e5-a9d6-dcd3896778a9.jpeg)](https://dev.to/kuncheriakuruvilla)

[Kuncheria Kuruvilla](https://dev.to/kuncheriakuruvilla)

Kuncheria Kuruvilla

[![](https://res.cloudinary.com/practicaldev/image/fetch/s---cfcEl3O--/c_fill,f_auto,fl_progressive,h_90,q_auto,w_90/https://dev-to-uploads.s3.amazonaws.com/uploads/user/profile_image/316502/e0d2b6b0-2bc9-40e5-a9d6-dcd3896778a9.jpeg)
Kuncheria Kuruvilla](/kuncheriakuruvilla)

Follow

- Work
  Software Engineer at [Key Value Systems](https://keyvalue.systems/)
- Location
  India
- Joined
  Jan 13, 2020

• [Oct 15 '20 • Edited on Oct
15](https://dev.to/kuncheriakuruvilla/comment/16o6j)

Dropdown menu

- [Copy link](https://dev.to/kuncheriakuruvilla/comment/16o6j)
- - [Hide](#)

---

Hey , even now i think there is a problem.\
 Shouldn't it be \
 `this.name = "Ford Ranger";`

rather than \
 `var name = "Ford Ranger";`

for question number 24 ?

Favorite heart outline button

Favorite heart outline button

1 like

[](#/macmacky/70-javascript-interview-questions-5gfi/comments/new/16o6j)

Comment button

Reply

Collapse

Expand

[![weeb profile
image](https://res.cloudinary.com/practicaldev/image/fetch/s--ihL6_i4y--/c_fill,f_auto,fl_progressive,h_50,q_auto,w_50/https://dev-to-uploads.s3.amazonaws.com/uploads/user/profile_image/274584/0e942183-5ce0-4a45-b52d-55d83a0b2554.png)](https://dev.to/weeb)

[Patrik Kiss](https://dev.to/weeb)

Patrik Kiss

[![](https://res.cloudinary.com/practicaldev/image/fetch/s--gTz8Q8Sh--/c_fill,f_auto,fl_progressive,h_90,q_auto,w_90/https://dev-to-uploads.s3.amazonaws.com/uploads/user/profile_image/274584/0e942183-5ce0-4a45-b52d-55d83a0b2554.png)
Patrik Kiss](/weeb)

a short bio.

Follow

- Location
  Hungary
- Education
  Software developer
- Joined
  Nov 18, 2019

• [Jan 3 '20 • Edited on Jan 3](https://dev.to/weeb/comment/jk55)

Dropdown menu

- [Copy link](https://dev.to/weeb/comment/jk55)
- - [Hide](#)

---

Great article, well done! 👏

If I was asked any of these at a job interview, I couldn't answer a
single one 👍

Favorite heart outline button

Favorite heart outline button

9 likes

[](#/macmacky/70-javascript-interview-questions-5gfi/comments/new/jk55)

Comment button

Reply

Collapse

Expand

[![macmacky profile
image](https://res.cloudinary.com/practicaldev/image/fetch/s--ip3rQvUF--/c_fill,f_auto,fl_progressive,h_50,q_auto,w_50/https://dev-to-uploads.s3.amazonaws.com/uploads/user/profile_image/201157/3607fd1f-3a5f-4fdf-8421-01debc8523b7.jpg)](https://dev.to/macmacky)

[Mark A](https://dev.to/macmacky)

Author

Mark A

[![](https://res.cloudinary.com/practicaldev/image/fetch/s--11luy8FC--/c_fill,f_auto,fl_progressive,h_90,q_auto,w_90/https://dev-to-uploads.s3.amazonaws.com/uploads/user/profile_image/201157/3607fd1f-3a5f-4fdf-8421-01debc8523b7.jpg)
Mark A](/macmacky)

a Full-Stack developer who likes reading Tom Clancy's books and loves
talking with dogs.

Follow

- Work
  Software Engineer
- Location
  Cebu City
- Education
  Bachelor's Degree in Computer Engineering
- Joined
  Jul 24, 2019

Author

• [Jan 3 '20](https://dev.to/macmacky/comment/jk7k)

Dropdown menu

- [Copy link](https://dev.to/macmacky/comment/jk7k)
- - [Hide](#)

---

Thanks Kiss 😁

Favorite heart outline button

Favorite heart outline button

1 like

[](#/macmacky/70-javascript-interview-questions-5gfi/comments/new/jk7k)

Comment button

Reply

Collapse

Expand

[![mvasigh profile
image](https://res.cloudinary.com/practicaldev/image/fetch/s--tVHJCLGn--/c_fill,f_auto,fl_progressive,h_50,q_auto,w_50/https://dev-to-uploads.s3.amazonaws.com/uploads/user/profile_image/121627/59829a58-6568-4329-a922-7e120607b58b.png)](https://dev.to/mvasigh)

[Mehdi Vasigh](https://dev.to/mvasigh)

Mehdi Vasigh

[![](https://res.cloudinary.com/practicaldev/image/fetch/s--5FAIKA5K--/c_fill,f_auto,fl_progressive,h_90,q_auto,w_90/https://dev-to-uploads.s3.amazonaws.com/uploads/user/profile_image/121627/59829a58-6568-4329-a922-7e120607b58b.png)
Mehdi Vasigh](/mvasigh)

Software Engineer @Arundo, Instructor @GA

Follow

- Work
  Senior Software Engineer at [Arundo
  Analytics](https://www.arundo.com/)
- Location
  Houston, TX
- Joined
  Dec 13, 2018

• [Jan 3 '20](https://dev.to/mvasigh/comment/jl2c)

Dropdown menu

- [Copy link](https://dev.to/mvasigh/comment/jl2c)
- - [Hide](#)

---

Nice work! Most of these are pretty good. If you're a hiring manager
reading this though, I'd caution against asking questions like "is using
the + or unary plus operator the fastest way in converting a string to a
number?" because it really doesn't matter and you shouldn't make hiring
decisions based on one's knowledge of that.

Favorite heart outline button

Favorite heart outline button

6 likes

[](#/macmacky/70-javascript-interview-questions-5gfi/comments/new/jl2c)

Comment button

Reply

Collapse

Expand

[![cytrowski profile
image](https://res.cloudinary.com/practicaldev/image/fetch/s--62Pc_Wya--/c_fill,f_auto,fl_progressive,h_50,q_auto,w_50/https://dev-to-uploads.s3.amazonaws.com/uploads/user/profile_image/64901/aca69251-c314-40eb-a32c-3b325ecb3179.jpg)](https://dev.to/cytrowski)

[Bartosz Cytrowski](https://dev.to/cytrowski)

Bartosz Cytrowski

[![](https://res.cloudinary.com/practicaldev/image/fetch/s--AGrPF0Gm--/c_fill,f_auto,fl_progressive,h_90,q_auto,w_90/https://dev-to-uploads.s3.amazonaws.com/uploads/user/profile_image/64901/aca69251-c314-40eb-a32c-3b325ecb3179.jpg)
Bartosz Cytrowski](/cytrowski)

Follow

- Joined
  Mar 29, 2018

• [Jan 6 '20](https://dev.to/cytrowski/comment/jod4)

Dropdown menu

- [Copy link](https://dev.to/cytrowski/comment/jod4)
- - [Hide](#)

---

Great set of questions :) I want to clarify one thing though: "What does
the && operator do?" - It does not return last "truthy" or "falsy"
value. It returns the last value it has to calculate to determine the
truthiness of the whole expression, eg. `0 || 0 || 0` - will return `0`
and `1 && 1 && 1` - will return `1`. So the statement in the article is
not 100% accurate :) Can't wait to see the update ;)

Favorite heart outline button

Favorite heart outline button

4 likes

[](#/macmacky/70-javascript-interview-questions-5gfi/comments/new/jod4)

Comment button

Reply

Collapse

Expand

[![kotikspb profile
image](https://res.cloudinary.com/practicaldev/image/fetch/s--m_ozwibT--/c_fill,f_auto,fl_progressive,h_50,q_auto,w_50/https://dev-to-uploads.s3.amazonaws.com/uploads/user/profile_image/363726/4b55153b-7c7d-47d3-8100-593941b33482.png)](https://dev.to/kotikspb)

[kotik-spb](https://dev.to/kotikspb)

kotik-spb

[![](https://res.cloudinary.com/practicaldev/image/fetch/s--TD84FF5K--/c_fill,f_auto,fl_progressive,h_90,q_auto,w_90/https://dev-to-uploads.s3.amazonaws.com/uploads/user/profile_image/363726/4b55153b-7c7d-47d3-8100-593941b33482.png)
kotik-spb](/kotikspb)

Follow

- Location
  Russia, Saint-Petersburg
- Joined
  Apr 9, 2020

• [Apr 9 '20](https://dev.to/kotikspb/comment/nhab)

Dropdown menu

- [Copy link](https://dev.to/kotikspb/comment/nhab)
- - [Hide](#)

---

Hi! Many thanks for the article, it's really very useful)))\
 And one thing in Question 31:\
 const result = strs.reduce((acc, currentStr) =\> acc + str, "");\
 I suppose you mean "currentStr" instead of "str" ;)

Favorite heart outline button

Favorite heart outline button

3 likes

[](#/macmacky/70-javascript-interview-questions-5gfi/comments/new/nhab)

Comment button

Reply

Collapse

Expand

[![macmacky profile
image](https://res.cloudinary.com/practicaldev/image/fetch/s--ip3rQvUF--/c_fill,f_auto,fl_progressive,h_50,q_auto,w_50/https://dev-to-uploads.s3.amazonaws.com/uploads/user/profile_image/201157/3607fd1f-3a5f-4fdf-8421-01debc8523b7.jpg)](https://dev.to/macmacky)

[Mark A](https://dev.to/macmacky)

Author

Mark A

[![](https://res.cloudinary.com/practicaldev/image/fetch/s--11luy8FC--/c_fill,f_auto,fl_progressive,h_90,q_auto,w_90/https://dev-to-uploads.s3.amazonaws.com/uploads/user/profile_image/201157/3607fd1f-3a5f-4fdf-8421-01debc8523b7.jpg)
Mark A](/macmacky)

a Full-Stack developer who likes reading Tom Clancy's books and loves
talking with dogs.

Follow

- Work
  Software Engineer
- Location
  Cebu City
- Education
  Bachelor's Degree in Computer Engineering
- Joined
  Jul 24, 2019

Author

• [Apr 9 '20](https://dev.to/macmacky/comment/nhgd)

Dropdown menu

- [Copy link](https://dev.to/macmacky/comment/nhgd)
- - [Hide](#)

---

I edited it just now. Thanks.

Favorite heart outline button

Favorite heart outline button

1 like

[](#/macmacky/70-javascript-interview-questions-5gfi/comments/new/nhgd)

Comment button

Reply

Collapse

Expand

[![bgauryy profile
image](https://res.cloudinary.com/practicaldev/image/fetch/s--D_g3kP7A--/c_fill,f_auto,fl_progressive,h_50,q_auto,w_50/https://dev-to-uploads.s3.amazonaws.com/uploads/user/profile_image/301986/5663711c-abcf-48d9-a54c-d793819cc3f4.png)](https://dev.to/bgauryy)

[bgauryy](https://dev.to/bgauryy)

bgauryy

[![](https://res.cloudinary.com/practicaldev/image/fetch/s--UV6itSIL--/c_fill,f_auto,fl_progressive,h_90,q_auto,w_90/https://dev-to-uploads.s3.amazonaws.com/uploads/user/profile_image/301986/5663711c-abcf-48d9-a54c-d793819cc3f4.png)
bgauryy](/bgauryy)

Software Engineer, Innovation-driven , Web development expert, Web
Security researcher, code enthusiast, and a drummer!

Follow

- Work
  Tech Lead at PerimeterX
- Location
  Tel Aviv
- Joined
  Dec 27, 2019

• [Apr 11 '20](https://dev.to/bgauryy/comment/nj10)

Dropdown menu

- [Copy link](https://dev.to/bgauryy/comment/nj10)
- - [Hide](#)

---

Great !

Personally, I think that good interviews should be focused on data flows
and performance optimization, and asking about certain API's should be
only for choosing the right question as an interviewer.\
 Also, interviewers should understand the difference between someone who
is not knowing something, to someone who is not capable of learning
something new.

Good luck for everyone :)

Favorite heart outline button

Favorite heart outline button

3 likes

[](#/macmacky/70-javascript-interview-questions-5gfi/comments/new/nj10)

Comment button

Reply

Collapse

Expand

[![sashaokey profile
image](https://res.cloudinary.com/practicaldev/image/fetch/s--7bWJVtZ_--/c_fill,f_auto,fl_progressive,h_50,q_auto,w_50/https://dev-to-uploads.s3.amazonaws.com/uploads/user/profile_image/404908/c76779af-a5e3-4628-b4fa-f709dd53435b.jpg)](https://dev.to/sashaokey)

[Alecc](https://dev.to/sashaokey)

Alecc

[![](https://res.cloudinary.com/practicaldev/image/fetch/s--Ok7gY4tV--/c_fill,f_auto,fl_progressive,h_90,q_auto,w_90/https://dev-to-uploads.s3.amazonaws.com/uploads/user/profile_image/404908/c76779af-a5e3-4628-b4fa-f709dd53435b.jpg)
Alecc](/sashaokey)

Follow

- Work
  Front End Developer
- Joined
  Jun 8, 2020

• [Jun 9 '20](https://dev.to/sashaokey/comment/104kc)

Dropdown menu

- [Copy link](https://dev.to/sashaokey/comment/104kc)
- - [Hide](#)

---

Mark, you did a grate job. I am finding this list very useful. In a way,
it even helped me to make the list of questions for our small
organisation(I have even sent it to some of our HRs))) So, believe it or
not ..It is used now in practical way in the eastern EU))))If being
completely serious, I would recommend more Typescript questions. I know
this is the JavaScript Int. Q. I really thing \< that using of
typescript is growing tremendously. Anyway , great Job, Mark. Thank you.

Favorite heart outline button

Favorite heart outline button

2 likes

[](#/macmacky/70-javascript-interview-questions-5gfi/comments/new/104kc)

Comment button

Reply

Collapse

Expand

[![macmacky profile
image](https://res.cloudinary.com/practicaldev/image/fetch/s--ip3rQvUF--/c_fill,f_auto,fl_progressive,h_50,q_auto,w_50/https://dev-to-uploads.s3.amazonaws.com/uploads/user/profile_image/201157/3607fd1f-3a5f-4fdf-8421-01debc8523b7.jpg)](https://dev.to/macmacky)

[Mark A](https://dev.to/macmacky)

Author

Mark A

[![](https://res.cloudinary.com/practicaldev/image/fetch/s--11luy8FC--/c_fill,f_auto,fl_progressive,h_90,q_auto,w_90/https://dev-to-uploads.s3.amazonaws.com/uploads/user/profile_image/201157/3607fd1f-3a5f-4fdf-8421-01debc8523b7.jpg)
Mark A](/macmacky)

a Full-Stack developer who likes reading Tom Clancy's books and loves
talking with dogs.

Follow

- Work
  Software Engineer
- Location
  Cebu City
- Education
  Bachelor's Degree in Computer Engineering
- Joined
  Jul 24, 2019

Author

• [Jun 9 '20 • Edited on Jun 9](https://dev.to/macmacky/comment/104kf)

Dropdown menu

- [Copy link](https://dev.to/macmacky/comment/104kf)
- - [Hide](#)

---

Hi Alecc, I'm really glad that you like it. That's a nice suggestion.
I've been using typescript for over two years now and it's really great
it makes your JavaScript code more readable and maintainable. I'll make
some questions in the future. Thanks and God bless.

Favorite heart outline button

Favorite heart outline button

5 likes

[](#/macmacky/70-javascript-interview-questions-5gfi/comments/new/104kf)

Comment button

Reply

Collapse

Expand

[![sashaokey profile
image](https://res.cloudinary.com/practicaldev/image/fetch/s--7bWJVtZ_--/c_fill,f_auto,fl_progressive,h_50,q_auto,w_50/https://dev-to-uploads.s3.amazonaws.com/uploads/user/profile_image/404908/c76779af-a5e3-4628-b4fa-f709dd53435b.jpg)](https://dev.to/sashaokey)

[Alecc](https://dev.to/sashaokey)

Alecc

[![](https://res.cloudinary.com/practicaldev/image/fetch/s--Ok7gY4tV--/c_fill,f_auto,fl_progressive,h_90,q_auto,w_90/https://dev-to-uploads.s3.amazonaws.com/uploads/user/profile_image/404908/c76779af-a5e3-4628-b4fa-f709dd53435b.jpg)
Alecc](/sashaokey)

Follow

- Work
  Front End Developer
- Joined
  Jun 8, 2020

• [Jun 9 '20](https://dev.to/sashaokey/comment/104l4)

Dropdown menu

- [Copy link](https://dev.to/sashaokey/comment/104l4)
- - [Hide](#)

---

Yes,m Mark, that is amazing how fast the Typescript "cases" grow. I mean
, two years ago I have the project, where I had one TS file and I do not
even remember why. But now. My team just received a source , There were
no JS file extension. TS, TSx). I am, actually, just starting with
Typescript.

Favorite heart outline button

Favorite heart outline button

5 likes

[](#/macmacky/70-javascript-interview-questions-5gfi/comments/new/104l4)

Comment button

Reply

Collapse

Expand

[![amirhe profile
image](https://res.cloudinary.com/practicaldev/image/fetch/s--os40s1Ut--/c_fill,f_auto,fl_progressive,h_50,q_auto,w_50/https://dev-to-uploads.s3.amazonaws.com/uploads/user/profile_image/93665/826a5e81-0e25-40ca-a0c4-aba9ee6e4aa0.png)](https://dev.to/amirhe)

[Amir.H Ebrahimi](https://dev.to/amirhe)

Amir.H Ebrahimi

[![](https://res.cloudinary.com/practicaldev/image/fetch/s--OCNuKLrd--/c_fill,f_auto,fl_progressive,h_90,q_auto,w_90/https://dev-to-uploads.s3.amazonaws.com/uploads/user/profile_image/93665/826a5e81-0e25-40ca-a0c4-aba9ee6e4aa0.png)
Amir.H Ebrahimi](/amirhe)

Follow

- Joined
  Aug 17, 2018

• [Jul 22 '20](https://dev.to/amirhe/comment/12c2h)

Dropdown menu

- [Copy link](https://dev.to/amirhe/comment/12c2h)
- - [Hide](#)

---

actually Implement the `Array.prototype.map` is not too precise for what
really wanted to be implemented.\

```{.highlight .javascript}
[,1,2,3,].map(console.log)
//  [empty, undefined, undefined, undefined]

map([,1,2,3,], console.log)
// [undefined, undefined, undefined, undefined]
```

Favorite heart outline button

Favorite heart outline button

1 like

[](#/macmacky/70-javascript-interview-questions-5gfi/comments/new/12c2h)

Comment button

Reply

Collapse

Expand

[![talantbekov123 profile
image](https://res.cloudinary.com/practicaldev/image/fetch/s--qFVZUDQY--/c_fill,f_auto,fl_progressive,h_50,q_auto,w_50/https://dev-to-uploads.s3.amazonaws.com/uploads/user/profile_image/446531/203c1a32-9c71-45fe-a945-d3fdb63fbdbb.jpeg)](https://dev.to/talantbekov123)

[Kairat Talantbekov](https://dev.to/talantbekov123)

Kairat Talantbekov

[![](https://res.cloudinary.com/practicaldev/image/fetch/s--HE3Nk7gT--/c_fill,f_auto,fl_progressive,h_90,q_auto,w_90/https://dev-to-uploads.s3.amazonaws.com/uploads/user/profile_image/446531/203c1a32-9c71-45fe-a945-d3fdb63fbdbb.jpeg)
Kairat Talantbekov](/talantbekov123)

I'm the developer with an entrepreneurial spirit who wants to do social
good.

Follow

- Work
  Front end developer at Freelance
- Location
  Kyrgyzstan, Bishkek
- Joined
  Aug 4, 2020

• [Aug 4 '20](https://dev.to/talantbekov123/comment/134p9)

Dropdown menu

- [Copy link](https://dev.to/talantbekov123/comment/134p9)
- - [Hide](#)

---

Great content! My name is Kairat, I'm a freelance self tough js
developer. I'm planning to get a job as a Front end developer instead of
freelancing.

Question: This article is very helpful for my theoretical knowledge. I'm
just curious will I use these terms in my daily job? Seems like
preparation for the exam and I will not use this knowledge in work. Or
use very rarely.

Favorite heart outline button

Favorite heart outline button

2 likes

[](#/macmacky/70-javascript-interview-questions-5gfi/comments/new/134p9)

Comment button

Reply

Collapse

Expand

[![droutback profile
image](https://res.cloudinary.com/practicaldev/image/fetch/s--ZXnbSAw5--/c_fill,f_auto,fl_progressive,h_50,q_auto,w_50/https://dev-to-uploads.s3.amazonaws.com/uploads/user/profile_image/189687/b74c0e5b-11a1-40a1-b36d-866ec6f63e6e.png)](https://dev.to/droutback)

[DrOutback](https://dev.to/droutback)

DrOutback

[![](https://res.cloudinary.com/practicaldev/image/fetch/s--96t27FM2--/c_fill,f_auto,fl_progressive,h_90,q_auto,w_90/https://dev-to-uploads.s3.amazonaws.com/uploads/user/profile_image/189687/b74c0e5b-11a1-40a1-b36d-866ec6f63e6e.png)
DrOutback](/droutback)

Follow

- Joined
  Jul 3, 2019

• [Jan 4 '20](https://dev.to/droutback/comment/jlfh)

Dropdown menu

- [Copy link](https://dev.to/droutback/comment/jlfh)
- - [Hide](#)

---

“let x = 5;

x = (x++ , x = addFive(x), x \*= 2, x -= 5, x += 10);

function addFive(num) {\
 return num + 5;\
 }\
 If you log the value of x it would be 27. First, we increment the value
of x it would be 6, then we invoke the function incrementBy5(6) and pass
the 6 as a parameter”

Do you mean addFive(6)?

I’m new to js, so I’m probably wrong.

Favorite heart outline button

Favorite heart outline button

1 like

[](#/macmacky/70-javascript-interview-questions-5gfi/comments/new/jlfh)

Comment button

Reply

Collapse

Expand

[![macmacky profile
image](https://res.cloudinary.com/practicaldev/image/fetch/s--ip3rQvUF--/c_fill,f_auto,fl_progressive,h_50,q_auto,w_50/https://dev-to-uploads.s3.amazonaws.com/uploads/user/profile_image/201157/3607fd1f-3a5f-4fdf-8421-01debc8523b7.jpg)](https://dev.to/macmacky)

[Mark A](https://dev.to/macmacky)

Author

Mark A

[![](https://res.cloudinary.com/practicaldev/image/fetch/s--11luy8FC--/c_fill,f_auto,fl_progressive,h_90,q_auto,w_90/https://dev-to-uploads.s3.amazonaws.com/uploads/user/profile_image/201157/3607fd1f-3a5f-4fdf-8421-01debc8523b7.jpg)
Mark A](/macmacky)

a Full-Stack developer who likes reading Tom Clancy's books and loves
talking with dogs.

Follow

- Work
  Software Engineer
- Location
  Cebu City
- Education
  Bachelor's Degree in Computer Engineering
- Joined
  Jul 24, 2019

Author

• [Jan 4 '20](https://dev.to/macmacky/comment/jljk)

Dropdown menu

- [Copy link](https://dev.to/macmacky/comment/jljk)
- - [Hide](#)

---

Thanks for telling me this little problem 😁

Favorite heart outline button

Favorite heart outline button

1 like

[](#/macmacky/70-javascript-interview-questions-5gfi/comments/new/jljk)

Comment button

Reply

Collapse

Expand

[![droutback profile
image](https://res.cloudinary.com/practicaldev/image/fetch/s--ZXnbSAw5--/c_fill,f_auto,fl_progressive,h_50,q_auto,w_50/https://dev-to-uploads.s3.amazonaws.com/uploads/user/profile_image/189687/b74c0e5b-11a1-40a1-b36d-866ec6f63e6e.png)](https://dev.to/droutback)

[DrOutback](https://dev.to/droutback)

DrOutback

[![](https://res.cloudinary.com/practicaldev/image/fetch/s--96t27FM2--/c_fill,f_auto,fl_progressive,h_90,q_auto,w_90/https://dev-to-uploads.s3.amazonaws.com/uploads/user/profile_image/189687/b74c0e5b-11a1-40a1-b36d-866ec6f63e6e.png)
DrOutback](/droutback)

Follow

- Joined
  Jul 3, 2019

• [Jan 4 '20](https://dev.to/droutback/comment/jlk2)

Dropdown menu

- [Copy link](https://dev.to/droutback/comment/jlk2)
- - [Hide](#)

---

Thanks for writing the article. I’m enjoying it.

Also,

reduce.apply(obj1, [1, 2, 3, 4, 5]); // returns 15\
 reduce.apply(obj2, 1, 2, 3, 4, 5); // returns 15

Did you mean reduce.call obj2, 1, 2, 3, 4, 5); ?

Favorite heart outline button

Favorite heart outline button

3 likes

Thread

Thread

[![macmacky profile
image](https://res.cloudinary.com/practicaldev/image/fetch/s--ip3rQvUF--/c_fill,f_auto,fl_progressive,h_50,q_auto,w_50/https://dev-to-uploads.s3.amazonaws.com/uploads/user/profile_image/201157/3607fd1f-3a5f-4fdf-8421-01debc8523b7.jpg)](https://dev.to/macmacky)

[Mark A](https://dev.to/macmacky)

Author

Mark A

[![](https://res.cloudinary.com/practicaldev/image/fetch/s--11luy8FC--/c_fill,f_auto,fl_progressive,h_90,q_auto,w_90/https://dev-to-uploads.s3.amazonaws.com/uploads/user/profile_image/201157/3607fd1f-3a5f-4fdf-8421-01debc8523b7.jpg)
Mark A](/macmacky)

a Full-Stack developer who likes reading Tom Clancy's books and loves
talking with dogs.

Follow

- Work
  Software Engineer
- Location
  Cebu City
- Education
  Bachelor's Degree in Computer Engineering
- Joined
  Jul 24, 2019

Author

• [Jan 4 '20](https://dev.to/macmacky/comment/jlme)

Dropdown menu

- [Copy link](https://dev.to/macmacky/comment/jlme)
- - [Hide](#)

---

Thanks again 😁

Favorite heart outline button

Favorite heart outline button

1 like

[](#/macmacky/70-javascript-interview-questions-5gfi/comments/new/jlme)

Comment button

Reply

Collapse

Expand

[![udit1994 profile
image](https://res.cloudinary.com/practicaldev/image/fetch/s--34fTIrtY--/c_fill,f_auto,fl_progressive,h_50,q_auto,w_50/https://dev-to-uploads.s3.amazonaws.com/uploads/user/profile_image/443938/fb2ef5a9-2a31-4191-9913-6653a93914d5.jpeg)](https://dev.to/udit1994)

[Udit Kaushik](https://dev.to/udit1994)

Udit Kaushik

[![](https://res.cloudinary.com/practicaldev/image/fetch/s--jgiVJ1-P--/c_fill,f_auto,fl_progressive,h_90,q_auto,w_90/https://dev-to-uploads.s3.amazonaws.com/uploads/user/profile_image/443938/fb2ef5a9-2a31-4191-9913-6653a93914d5.jpeg)
Udit Kaushik](/udit1994)

Frontend Developer

Follow

- Work
  Developer
- Joined
  Jul 30, 2020

• [Jul 31 '20](https://dev.to/udit1994/comment/12pog)

Dropdown menu

- [Copy link](https://dev.to/udit1994/comment/12pog)
- - [Hide](#)

---

Great article. Very informative. For the question 34, 35 and 36. The
implementation might not be quite accurate. You might wanna re-check.
For example, to map(), we just pass the `callback` function. While in
your implementation above, you are passing both `array` and `callback`
to the map(). The array will be available as `this` inside the map().
Please do correct me if i am wrong.

Favorite heart outline button

Favorite heart outline button

1 like

[](#/macmacky/70-javascript-interview-questions-5gfi/comments/new/12pog)

Comment button

Reply

Collapse

Expand

[![ziizium profile
image](https://res.cloudinary.com/practicaldev/image/fetch/s--cuKtxcc---/c_fill,f_auto,fl_progressive,h_50,q_auto,w_50/https://dev-to-uploads.s3.amazonaws.com/uploads/user/profile_image/140071/3054d913-f87e-485e-b015-5a65049d1311.jpg)](https://dev.to/ziizium)

[Habdul Hazeez](https://dev.to/ziizium)

Habdul Hazeez

[![](https://res.cloudinary.com/practicaldev/image/fetch/s--zHCr5PJD--/c_fill,f_auto,fl_progressive,h_90,q_auto,w_90/https://dev-to-uploads.s3.amazonaws.com/uploads/user/profile_image/140071/3054d913-f87e-485e-b015-5a65049d1311.jpg)
Habdul Hazeez](/ziizium)

I teach and write code with interests in Web Development, Computer
Security, and Artificial Intelligence.

Follow

- Work
  Web Developer
- Location
  Nigeria
- Education
  B.Sc. Computer Science
- Joined
  Feb 25, 2019

• [Jan 3 '20 • Edited on Jan 3](https://dev.to/ziizium/comment/jkbn)

Dropdown menu

- [Copy link](https://dev.to/ziizium/comment/jkbn)
- - [Hide](#)

---

> Thanks guys for reading this post.

Thank you for the effort.

**EDIT:** In [Question
5](https://dev.to/macmacky/70-javascript-interview-questions-5gfi#5-what-is-the-dom)
you wrote:

> Image if we have an HTML structure like this.

Did you intend to use the word **Imagine** instead of **Image**?

Favorite heart outline button

Favorite heart outline button

2 likes

[](#/macmacky/70-javascript-interview-questions-5gfi/comments/new/jkbn)

Comment button

Reply

Collapse

Expand

[![affiction profile
image](https://res.cloudinary.com/practicaldev/image/fetch/s--Xm2Xvzoz--/c_fill,f_auto,fl_progressive,h_50,q_auto,w_50/https://dev-to-uploads.s3.amazonaws.com/uploads/user/profile_image/308438/5c4e7377-f839-4f38-8e50-e94a79eafbfd.png)](https://dev.to/affiction)

[Maxim](https://dev.to/affiction)

Maxim

[![](https://res.cloudinary.com/practicaldev/image/fetch/s--H-Loi8ZD--/c_fill,f_auto,fl_progressive,h_90,q_auto,w_90/https://dev-to-uploads.s3.amazonaws.com/uploads/user/profile_image/308438/5c4e7377-f839-4f38-8e50-e94a79eafbfd.png)
Maxim](/affiction)

Follow

- Work
  Sr. JavaScript Developer
- Location
  Ukraine
- Joined
  Jan 4, 2020

• [Jan 4 '20](https://dev.to/affiction/comment/jlni)

Dropdown menu

- [Copy link](https://dev.to/affiction/comment/jlni)
- - [Hide](#)

---

Question \#26\

```{.highlight .javascript}
var li = document.querySelector('.list-group > li');
```

Probably here should be **querySelectorAll** instead of
**querySelector**🙂

Favorite heart outline button

Favorite heart outline button

2 likes

[](#/macmacky/70-javascript-interview-questions-5gfi/comments/new/jlni)

Comment button

Reply

Collapse

Expand

[![macmacky profile
image](https://res.cloudinary.com/practicaldev/image/fetch/s--ip3rQvUF--/c_fill,f_auto,fl_progressive,h_50,q_auto,w_50/https://dev-to-uploads.s3.amazonaws.com/uploads/user/profile_image/201157/3607fd1f-3a5f-4fdf-8421-01debc8523b7.jpg)](https://dev.to/macmacky)

[Mark A](https://dev.to/macmacky)

Author

Mark A

[![](https://res.cloudinary.com/practicaldev/image/fetch/s--11luy8FC--/c_fill,f_auto,fl_progressive,h_90,q_auto,w_90/https://dev-to-uploads.s3.amazonaws.com/uploads/user/profile_image/201157/3607fd1f-3a5f-4fdf-8421-01debc8523b7.jpg)
Mark A](/macmacky)

a Full-Stack developer who likes reading Tom Clancy's books and loves
talking with dogs.

Follow

- Work
  Software Engineer
- Location
  Cebu City
- Education
  Bachelor's Degree in Computer Engineering
- Joined
  Jul 24, 2019

Author

• [Jan 4 '20](https://dev.to/macmacky/comment/jlp2)

Dropdown menu

- [Copy link](https://dev.to/macmacky/comment/jlp2)
- - [Hide](#)

---

Thanks 😁, my bad.

Favorite heart outline button

Favorite heart outline button

2 likes

[](#/macmacky/70-javascript-interview-questions-5gfi/comments/new/jlp2)

Comment button

Reply

Collapse

Expand

[![mohammedasker profile
image](https://res.cloudinary.com/practicaldev/image/fetch/s--Rd8jvqJl--/c_fill,f_auto,fl_progressive,h_50,q_auto,w_50/https://dev-to-uploads.s3.amazonaws.com/uploads/user/profile_image/188020/344fc4a8-8d96-4588-95bf-58354c61db80.jpeg)](https://dev.to/mohammedasker)

[Mohammed Asker](https://dev.to/mohammedasker)

Mohammed Asker

[![](https://res.cloudinary.com/practicaldev/image/fetch/s--6ZaNhgJL--/c_fill,f_auto,fl_progressive,h_90,q_auto,w_90/https://dev-to-uploads.s3.amazonaws.com/uploads/user/profile_image/188020/344fc4a8-8d96-4588-95bf-58354c61db80.jpeg)
Mohammed Asker](/mohammedasker)

Frontend developer, Freelancer & Blogger. I document my journey in tech
and share my wins, failures, tips, and things I wish I knew.

Follow

- Work
  Front-end developer
- Location
  Hargeisa, Somaliland
- Education
  Admas University
- Joined
  Jun 29, 2019

• [Jan 3 '20](https://dev.to/mohammedasker/comment/jkj9)

Dropdown menu

- [Copy link](https://dev.to/mohammedasker/comment/jkj9)
- - [Hide](#)

---

I think this is the longest read time I ever see on the internet. Thank
you for the article. I'd bookmark for future references.

Favorite heart outline button

Favorite heart outline button

3 likes

[](#/macmacky/70-javascript-interview-questions-5gfi/comments/new/jkj9)

Comment button

Reply

Collapse

Expand

[![hoangph271 profile
image](https://res.cloudinary.com/practicaldev/image/fetch/s--nO6WUhsH--/c_fill,f_auto,fl_progressive,h_50,q_auto,w_50/https://dev-to-uploads.s3.amazonaws.com/uploads/user/profile_image/159599/29a66355-a7d1-4f94-878d-129f83af983d.png)](https://dev.to/hoangph271)

[Huy Hoàng Phan](https://dev.to/hoangph271)

Huy Hoàng Phan

[![](https://res.cloudinary.com/practicaldev/image/fetch/s--4CL9Kj2G--/c_fill,f_auto,fl_progressive,h_90,q_auto,w_90/https://dev-to-uploads.s3.amazonaws.com/uploads/user/profile_image/159599/29a66355-a7d1-4f94-878d-129f83af983d.png)
Huy Hoàng Phan](/hoangph271)

Follow

- Joined
  Apr 23, 2019

• [Jan 3 '20 • Edited on Jan 3](https://dev.to/hoangph271/comment/jk71)

Dropdown menu

- [Copy link](https://dev.to/hoangph271/comment/jk71)
- - [Hide](#)

---

I think there're a mistake here...!\

```{.highlight .javascript}
function myFunc() {
  let a = b;
  a = b = 0;
}
myFunc();
```

Isn't this invalid syntax...?\
 It should be:\

```{.highlight .javascript}
let a, b;
```

Favorite heart outline button

Favorite heart outline button

2 likes

[](#/macmacky/70-javascript-interview-questions-5gfi/comments/new/jk71)

Comment button

Reply

Collapse

Expand

[![macmacky profile
image](https://res.cloudinary.com/practicaldev/image/fetch/s--ip3rQvUF--/c_fill,f_auto,fl_progressive,h_50,q_auto,w_50/https://dev-to-uploads.s3.amazonaws.com/uploads/user/profile_image/201157/3607fd1f-3a5f-4fdf-8421-01debc8523b7.jpg)](https://dev.to/macmacky)

[Mark A](https://dev.to/macmacky)

Author

Mark A

[![](https://res.cloudinary.com/practicaldev/image/fetch/s--11luy8FC--/c_fill,f_auto,fl_progressive,h_90,q_auto,w_90/https://dev-to-uploads.s3.amazonaws.com/uploads/user/profile_image/201157/3607fd1f-3a5f-4fdf-8421-01debc8523b7.jpg)
Mark A](/macmacky)

a Full-Stack developer who likes reading Tom Clancy's books and loves
talking with dogs.

Follow

- Work
  Software Engineer
- Location
  Cebu City
- Education
  Bachelor's Degree in Computer Engineering
- Joined
  Jul 24, 2019

Author

• [Jan 3 '20](https://dev.to/macmacky/comment/jk7j)

Dropdown menu

- [Copy link](https://dev.to/macmacky/comment/jk7j)
- - [Hide](#)

---

Thanks man, I totally miss that one, hahaha

Favorite heart outline button

Favorite heart outline button

1 like

[](#/macmacky/70-javascript-interview-questions-5gfi/comments/new/jk7j)

Comment button

Reply

Collapse

Expand

[![thedotnetweekly profile
image](https://res.cloudinary.com/practicaldev/image/fetch/s--TOBFDAyt--/c_fill,f_auto,fl_progressive,h_50,q_auto,w_50/https://dev-to-uploads.s3.amazonaws.com/uploads/user/profile_image/133022/48d81c34-e936-4b23-ad31-0e87184412ec.jpg)](https://dev.to/thedotnetweekly)

[The DotNET Weekly](https://dev.to/thedotnetweekly)

The DotNET Weekly

[![](https://res.cloudinary.com/practicaldev/image/fetch/s--XjrEqkP8--/c_fill,f_auto,fl_progressive,h_90,q_auto,w_90/https://dev-to-uploads.s3.amazonaws.com/uploads/user/profile_image/133022/48d81c34-e936-4b23-ad31-0e87184412ec.jpg)
The DotNET Weekly](/thedotnetweekly)

Bi-Weekly posts about dotnet.

Follow

- Joined
  Jan 30, 2019

• [Jan 3 '20](https://dev.to/thedotnetweekly/comment/jk1o)

Dropdown menu

- [Copy link](https://dev.to/thedotnetweekly/comment/jk1o)
- - [Hide](#)

---

Nice list, my favorite one is what is hoisting :)

Favorite heart outline button

Favorite heart outline button

2 likes

[](#/macmacky/70-javascript-interview-questions-5gfi/comments/new/jk1o)

Comment button

Reply

Collapse

Expand

[![macmacky profile
image](https://res.cloudinary.com/practicaldev/image/fetch/s--ip3rQvUF--/c_fill,f_auto,fl_progressive,h_50,q_auto,w_50/https://dev-to-uploads.s3.amazonaws.com/uploads/user/profile_image/201157/3607fd1f-3a5f-4fdf-8421-01debc8523b7.jpg)](https://dev.to/macmacky)

[Mark A](https://dev.to/macmacky)

Author

Mark A

[![](https://res.cloudinary.com/practicaldev/image/fetch/s--11luy8FC--/c_fill,f_auto,fl_progressive,h_90,q_auto,w_90/https://dev-to-uploads.s3.amazonaws.com/uploads/user/profile_image/201157/3607fd1f-3a5f-4fdf-8421-01debc8523b7.jpg)
Mark A](/macmacky)

a Full-Stack developer who likes reading Tom Clancy's books and loves
talking with dogs.

Follow

- Work
  Software Engineer
- Location
  Cebu City
- Education
  Bachelor's Degree in Computer Engineering
- Joined
  Jul 24, 2019

Author

• [Jan 3 '20](https://dev.to/macmacky/comment/jk7n)

Dropdown menu

- [Copy link](https://dev.to/macmacky/comment/jk7n)
- - [Hide](#)

---

Thanks, yea Hoisting is pretty fun to learn

Favorite heart outline button

Favorite heart outline button

1 like

[](#/macmacky/70-javascript-interview-questions-5gfi/comments/new/jk7n)

Comment button

Reply

Collapse

Expand

[![techdebtor profile
image](https://res.cloudinary.com/practicaldev/image/fetch/s--7UFY8zWq--/c_fill,f_auto,fl_progressive,h_50,q_auto,w_50/https://dev-to-uploads.s3.amazonaws.com/uploads/user/profile_image/115393/1094e249-f3db-4ec2-b942-992dee26b7d1.jpg)](https://dev.to/techdebtor)

[sam](https://dev.to/techdebtor)

sam

[![](https://res.cloudinary.com/practicaldev/image/fetch/s--ad7F58fI--/c_fill,f_auto,fl_progressive,h_90,q_auto,w_90/https://dev-to-uploads.s3.amazonaws.com/uploads/user/profile_image/115393/1094e249-f3db-4ec2-b942-992dee26b7d1.jpg)
sam](/techdebtor)

software engineer in SF (they/them)

Follow

- Work
  Software Engineer at Shippo
- Location
  San Francisco
- Education
  UT Austin
- Joined
  Nov 17, 2018

• [Jan 3 '20](https://dev.to/techdebtor/comment/jk1f)

Dropdown menu

- [Copy link](https://dev.to/techdebtor/comment/jk1f)
- - [Hide](#)

---

These are great, thanks for sharing!

Favorite heart outline button

Favorite heart outline button

2 likes

[](#/macmacky/70-javascript-interview-questions-5gfi/comments/new/jk1f)

Comment button

Reply

Collapse

Expand

[![macmacky profile
image](https://res.cloudinary.com/practicaldev/image/fetch/s--ip3rQvUF--/c_fill,f_auto,fl_progressive,h_50,q_auto,w_50/https://dev-to-uploads.s3.amazonaws.com/uploads/user/profile_image/201157/3607fd1f-3a5f-4fdf-8421-01debc8523b7.jpg)](https://dev.to/macmacky)

[Mark A](https://dev.to/macmacky)

Author

Mark A

[![](https://res.cloudinary.com/practicaldev/image/fetch/s--11luy8FC--/c_fill,f_auto,fl_progressive,h_90,q_auto,w_90/https://dev-to-uploads.s3.amazonaws.com/uploads/user/profile_image/201157/3607fd1f-3a5f-4fdf-8421-01debc8523b7.jpg)
Mark A](/macmacky)

a Full-Stack developer who likes reading Tom Clancy's books and loves
talking with dogs.

Follow

- Work
  Software Engineer
- Location
  Cebu City
- Education
  Bachelor's Degree in Computer Engineering
- Joined
  Jul 24, 2019

Author

• [Jan 3 '20](https://dev.to/macmacky/comment/jk7o)

Dropdown menu

- [Copy link](https://dev.to/macmacky/comment/jk7o)
- - [Hide](#)

---

No problem man, and btw Thanks 😁

Favorite heart outline button

Favorite heart outline button

1 like

[](#/macmacky/70-javascript-interview-questions-5gfi/comments/new/jk7o)

Comment button

Reply

Collapse

Expand

[![danieltareke profile
image](https://res.cloudinary.com/practicaldev/image/fetch/s--e-LymDcj--/c_fill,f_auto,fl_progressive,h_50,q_auto,w_50/https://dev-to-uploads.s3.amazonaws.com/uploads/user/profile_image/301787/22afc80f-da8a-44ec-b9e6-ec3fc42d7ede.png)](https://dev.to/danieltareke)

[Daniel](https://dev.to/danieltareke)

Daniel

[![](https://res.cloudinary.com/practicaldev/image/fetch/s--UgSZDYGR--/c_fill,f_auto,fl_progressive,h_90,q_auto,w_90/https://dev-to-uploads.s3.amazonaws.com/uploads/user/profile_image/301787/22afc80f-da8a-44ec-b9e6-ec3fc42d7ede.png)
Daniel](/danieltareke)

Follow

- Joined
  Dec 27, 2019

• [Jan 5 '20 • Edited on Jan
5](https://dev.to/danieltareke/comment/jme5)

Dropdown menu

- [Copy link](https://dev.to/danieltareke/comment/jme5)
- - [Hide](#)

---

Well done, it is helpful

Favorite heart outline button

Favorite heart outline button

2 likes

[](#/macmacky/70-javascript-interview-questions-5gfi/comments/new/jme5)

Comment button

Reply

Collapse

Expand

[![macmacky profile
image](https://res.cloudinary.com/practicaldev/image/fetch/s--ip3rQvUF--/c_fill,f_auto,fl_progressive,h_50,q_auto,w_50/https://dev-to-uploads.s3.amazonaws.com/uploads/user/profile_image/201157/3607fd1f-3a5f-4fdf-8421-01debc8523b7.jpg)](https://dev.to/macmacky)

[Mark A](https://dev.to/macmacky)

Author

Mark A

[![](https://res.cloudinary.com/practicaldev/image/fetch/s--11luy8FC--/c_fill,f_auto,fl_progressive,h_90,q_auto,w_90/https://dev-to-uploads.s3.amazonaws.com/uploads/user/profile_image/201157/3607fd1f-3a5f-4fdf-8421-01debc8523b7.jpg)
Mark A](/macmacky)

a Full-Stack developer who likes reading Tom Clancy's books and loves
talking with dogs.

Follow

- Work
  Software Engineer
- Location
  Cebu City
- Education
  Bachelor's Degree in Computer Engineering
- Joined
  Jul 24, 2019

Author

• [Jan 5 '20](https://dev.to/macmacky/comment/jmmk)

Dropdown menu

- [Copy link](https://dev.to/macmacky/comment/jmmk)
- - [Hide](#)

---

Thanks 😁

Favorite heart outline button

Favorite heart outline button

1 like

[](#/macmacky/70-javascript-interview-questions-5gfi/comments/new/jmmk)

Comment button

Reply

Collapse

Expand

[![armw4 profile
image](https://res.cloudinary.com/practicaldev/image/fetch/s--FlC-s5Dc--/c_fill,f_auto,fl_progressive,h_50,q_auto,w_50/https://dev-to-uploads.s3.amazonaws.com/uploads/user/profile_image/280348/8d8c7844-b689-4fe7-aaf1-a1e908897f7d.png)](https://dev.to/armw4)

[Antwan R. Wimberly](https://dev.to/armw4)

Antwan R. Wimberly

[![](https://res.cloudinary.com/practicaldev/image/fetch/s--picUq_IH--/c_fill,f_auto,fl_progressive,h_90,q_auto,w_90/https://dev-to-uploads.s3.amazonaws.com/uploads/user/profile_image/280348/8d8c7844-b689-4fe7-aaf1-a1e908897f7d.png)
Antwan R. Wimberly](/armw4)

SeNike Software Engineer 👨🏻‍💻 Nigeria 🇳🇬 you are loved Quality over
quantity Clarity is greater than clever be noble - ☮️

Follow

- Work
  Senior Software Engineer at N/A
- Location
  The Texas Triangle
- Education
  Bachelor of Science in Computer Science
- Joined
  Nov 26, 2019

• [Jan 7 '20](https://dev.to/armw4/comment/joek)

Dropdown menu

- [Copy link](https://dev.to/armw4/comment/joek)
- - [Hide](#)

---

Awesome!!! 👏🏿 \
 Gratitude 🙏🏿 \
 Stars ✨

Favorite heart outline button

Favorite heart outline button

2 likes

[](#/macmacky/70-javascript-interview-questions-5gfi/comments/new/joek)

Comment button

Reply

Collapse

Expand

[![jsgoupil profile
image](https://res.cloudinary.com/practicaldev/image/fetch/s--SfMt5cTi--/c_fill,f_auto,fl_progressive,h_50,q_auto,w_50/https://dev-to-uploads.s3.amazonaws.com/uploads/user/profile_image/280350/ae5d3aae-7c48-4748-8231-7f90d9a8d1b3.jpeg)](https://dev.to/jsgoupil)

[Jean-Sébastien Goupil](https://dev.to/jsgoupil)

Jean-Sébastien Goupil

[![](https://res.cloudinary.com/practicaldev/image/fetch/s--RJAP8VjM--/c_fill,f_auto,fl_progressive,h_90,q_auto,w_90/https://dev-to-uploads.s3.amazonaws.com/uploads/user/profile_image/280350/ae5d3aae-7c48-4748-8231-7f90d9a8d1b3.jpeg)
Jean-Sébastien Goupil](/jsgoupil)

Follow

- Work
  Web Architect Consultant
- Location
  Seattle, WA
- Joined
  Nov 26, 2019

• [Jan 7 '20](https://dev.to/jsgoupil/comment/jpea)

Dropdown menu

- [Copy link](https://dev.to/jsgoupil/comment/jpea)
- - [Hide](#)

---

I like this article, quite the refresher.\
 However, I think people forget quite a bit about the method bind that
can do partially applied function! And it's not mentioned here.

Favorite heart outline button

Favorite heart outline button

2 likes

[](#/macmacky/70-javascript-interview-questions-5gfi/comments/new/jpea)

Comment button

Reply

Collapse

Expand

[![camfilho profile
image](https://res.cloudinary.com/practicaldev/image/fetch/s--VVj5bspD--/c_fill,f_auto,fl_progressive,h_50,q_auto,w_50/https://dev-to-uploads.s3.amazonaws.com/uploads/user/profile_image/243811/ce415a5a-7093-4e2f-945a-7c9be08be17d.jpeg)](https://dev.to/camfilho)

[Carlos Augusto M. Filho](https://dev.to/camfilho)

Carlos Augusto M. Filho

[![](https://res.cloudinary.com/practicaldev/image/fetch/s--wTqXQpAg--/c_fill,f_auto,fl_progressive,h_90,q_auto,w_90/https://dev-to-uploads.s3.amazonaws.com/uploads/user/profile_image/243811/ce415a5a-7093-4e2f-945a-7c9be08be17d.jpeg)
Carlos Augusto M. Filho](/camfilho)

2B||\~2B? Software Developer

Follow

- Location
  Brazil
- Education
  Software Developer
- Joined
  Oct 6, 2019

• [Jan 7 '20](https://dev.to/camfilho/comment/jofo)

Dropdown menu

- [Copy link](https://dev.to/camfilho/comment/jofo)
- - [Hide](#)

---

Thanks!

Favorite heart outline button

Favorite heart outline button

2 likes

[](#/macmacky/70-javascript-interview-questions-5gfi/comments/new/jofo)

Comment button

Reply

Collapse

Expand

[![jetsondavis profile
image](https://res.cloudinary.com/practicaldev/image/fetch/s--Zq6RVtqm--/c_fill,f_auto,fl_progressive,h_50,q_auto,w_50/https://dev-to-uploads.s3.amazonaws.com/uploads/user/profile_image/177923/01df47af-40ae-41ee-982b-a0fe00905557.png)](https://dev.to/jetsondavis)

[Jeff Davidson](https://dev.to/jetsondavis)

Jeff Davidson

[![](https://res.cloudinary.com/practicaldev/image/fetch/s--bL5nLAHC--/c_fill,f_auto,fl_progressive,h_90,q_auto,w_90/https://dev-to-uploads.s3.amazonaws.com/uploads/user/profile_image/177923/01df47af-40ae-41ee-982b-a0fe00905557.png)
Jeff Davidson](/jetsondavis)

Follow

- Joined
  Jun 9, 2019

• [Jan 7 '20 • Edited on Jan 7](https://dev.to/jetsondavis/comment/joga)

Dropdown menu

- [Copy link](https://dev.to/jetsondavis/comment/joga)
- - [Hide](#)

---

Thanks Mark - great cheat sheet! Btw, what does your dog think of the
article?

Favorite heart outline button

Favorite heart outline button

2 likes

[](#/macmacky/70-javascript-interview-questions-5gfi/comments/new/joga)

Comment button

Reply

Collapse

Expand

[![ankitkanojia profile
image](https://res.cloudinary.com/practicaldev/image/fetch/s--LBaM_X8Z--/c_fill,f_auto,fl_progressive,h_50,q_auto,w_50/https://dev-to-uploads.s3.amazonaws.com/uploads/user/profile_image/306189/dc3a80df-4a57-4d48-8e9e-dccaca2a02ea.jpeg)](https://dev.to/ankitkanojia)

[Ankit Kanojia](https://dev.to/ankitkanojia)

Ankit Kanojia

[![](https://res.cloudinary.com/practicaldev/image/fetch/s--OerYISYE--/c_fill,f_auto,fl_progressive,h_90,q_auto,w_90/https://dev-to-uploads.s3.amazonaws.com/uploads/user/profile_image/306189/dc3a80df-4a57-4d48-8e9e-dccaca2a02ea.jpeg)
Ankit Kanojia](/ankitkanojia)

dedicated IT professionals, its subsidiaries and Joint Ventures provide
customized IT solutions for industries.

Follow

- Work
  Adept Coder | Full Stack Developer
- Location
  INDIA
- Education
  BCA-MCA
- Joined
  Jan 2, 2020

• [Jan 3 '20](https://dev.to/ankitkanojia/comment/jk8e)

Dropdown menu

- [Copy link](https://dev.to/ankitkanojia/comment/jk8e)
- - [Hide](#)

---

Great article. Great article !!!!

Favorite heart outline button

Favorite heart outline button

2 likes

[](#/macmacky/70-javascript-interview-questions-5gfi/comments/new/jk8e)

Comment button

Reply

Collapse

Expand

[![macmacky profile
image](https://res.cloudinary.com/practicaldev/image/fetch/s--ip3rQvUF--/c_fill,f_auto,fl_progressive,h_50,q_auto,w_50/https://dev-to-uploads.s3.amazonaws.com/uploads/user/profile_image/201157/3607fd1f-3a5f-4fdf-8421-01debc8523b7.jpg)](https://dev.to/macmacky)

[Mark A](https://dev.to/macmacky)

Author

Mark A

[![](https://res.cloudinary.com/practicaldev/image/fetch/s--11luy8FC--/c_fill,f_auto,fl_progressive,h_90,q_auto,w_90/https://dev-to-uploads.s3.amazonaws.com/uploads/user/profile_image/201157/3607fd1f-3a5f-4fdf-8421-01debc8523b7.jpg)
Mark A](/macmacky)

a Full-Stack developer who likes reading Tom Clancy's books and loves
talking with dogs.

Follow

- Work
  Software Engineer
- Location
  Cebu City
- Education
  Bachelor's Degree in Computer Engineering
- Joined
  Jul 24, 2019

Author

• [Jan 3 '20](https://dev.to/macmacky/comment/jknl)

Dropdown menu

- [Copy link](https://dev.to/macmacky/comment/jknl)
- - [Hide](#)

---

Thanks 😁😁😁

Favorite heart outline button

Favorite heart outline button

1 like

[](#/macmacky/70-javascript-interview-questions-5gfi/comments/new/jknl)

Comment button

Reply

Collapse

Expand

[![gharibi profile
image](https://res.cloudinary.com/practicaldev/image/fetch/s--7yaZJqTk--/c_fill,f_auto,fl_progressive,h_50,q_auto,w_50/https://dev-to-uploads.s3.amazonaws.com/uploads/user/profile_image/128454/d5ed6e9f-cbe6-4d7e-b1bd-a5f7f03d40ae.jpeg)](https://dev.to/gharibi)

[A. Gharibi](https://dev.to/gharibi)

A. Gharibi

[![](https://res.cloudinary.com/practicaldev/image/fetch/s--NOgvFfUi--/c_fill,f_auto,fl_progressive,h_90,q_auto,w_90/https://dev-to-uploads.s3.amazonaws.com/uploads/user/profile_image/128454/d5ed6e9f-cbe6-4d7e-b1bd-a5f7f03d40ae.jpeg)
A. Gharibi](/gharibi)

Technology Evangelist

Follow

- Location
  Germany
- Joined
  Jan 13, 2019

• [Jan 3 '20](https://dev.to/gharibi/comment/jl02)

Dropdown menu

- [Copy link](https://dev.to/gharibi/comment/jl02)
- - [Hide](#)

---

Awesome, well done mate!

Favorite heart outline button

Favorite heart outline button

2 likes

[](#/macmacky/70-javascript-interview-questions-5gfi/comments/new/jl02)

Comment button

Reply

Collapse

Expand

[![macmacky profile
image](https://res.cloudinary.com/practicaldev/image/fetch/s--ip3rQvUF--/c_fill,f_auto,fl_progressive,h_50,q_auto,w_50/https://dev-to-uploads.s3.amazonaws.com/uploads/user/profile_image/201157/3607fd1f-3a5f-4fdf-8421-01debc8523b7.jpg)](https://dev.to/macmacky)

[Mark A](https://dev.to/macmacky)

Author

Mark A

[![](https://res.cloudinary.com/practicaldev/image/fetch/s--11luy8FC--/c_fill,f_auto,fl_progressive,h_90,q_auto,w_90/https://dev-to-uploads.s3.amazonaws.com/uploads/user/profile_image/201157/3607fd1f-3a5f-4fdf-8421-01debc8523b7.jpg)
Mark A](/macmacky)

a Full-Stack developer who likes reading Tom Clancy's books and loves
talking with dogs.

Follow

- Work
  Software Engineer
- Location
  Cebu City
- Education
  Bachelor's Degree in Computer Engineering
- Joined
  Jul 24, 2019

Author

• [Jan 3 '20](https://dev.to/macmacky/comment/jl08)

Dropdown menu

- [Copy link](https://dev.to/macmacky/comment/jl08)
- - [Hide](#)

---

Thanks mate! 😁

Favorite heart outline button

Favorite heart outline button

1 like

[](#/macmacky/70-javascript-interview-questions-5gfi/comments/new/jl08)

Comment button

Reply

Collapse

Expand

[![lannex profile
image](https://res.cloudinary.com/practicaldev/image/fetch/s--Btn2SLTm--/c_fill,f_auto,fl_progressive,h_50,q_auto,w_50/https://dev-to-uploads.s3.amazonaws.com/uploads/user/profile_image/96737/bb73d577-225b-42a6-84e0-c63c1867a86e.JPG)](https://dev.to/lannex)

[Shin, SJ](https://dev.to/lannex)

Shin, SJ

[![](https://res.cloudinary.com/practicaldev/image/fetch/s--Jmfr4cyr--/c_fill,f_auto,fl_progressive,h_90,q_auto,w_90/https://dev-to-uploads.s3.amazonaws.com/uploads/user/profile_image/96737/bb73d577-225b-42a6-84e0-c63c1867a86e.JPG)
Shin, SJ](/lannex)

a Full-Stack Developer who wants to be a better

Follow

- Email
  [lannex.shin@gmail.com](mailto:lannex.shin@gmail.com)
- Location
  Seoul, South Korea
- Education
  Bachelor's Degree in Communication Design
- Joined
  Aug 29, 2018

• [Jan 6 '20](https://dev.to/lannex/comment/jn7f)

Dropdown menu

- [Copy link](https://dev.to/lannex/comment/jn7f)
- - [Hide](#)

---

Great article!\
 Can I translate it into Korean and post it on my blog?\
 I'll clarify the source.

Favorite heart outline button

Favorite heart outline button

2 likes

[](#/macmacky/70-javascript-interview-questions-5gfi/comments/new/jn7f)

Comment button

Reply

Collapse

Expand

[![macmacky profile
image](https://res.cloudinary.com/practicaldev/image/fetch/s--ip3rQvUF--/c_fill,f_auto,fl_progressive,h_50,q_auto,w_50/https://dev-to-uploads.s3.amazonaws.com/uploads/user/profile_image/201157/3607fd1f-3a5f-4fdf-8421-01debc8523b7.jpg)](https://dev.to/macmacky)

[Mark A](https://dev.to/macmacky)

Author

Mark A

[![](https://res.cloudinary.com/practicaldev/image/fetch/s--11luy8FC--/c_fill,f_auto,fl_progressive,h_90,q_auto,w_90/https://dev-to-uploads.s3.amazonaws.com/uploads/user/profile_image/201157/3607fd1f-3a5f-4fdf-8421-01debc8523b7.jpg)
Mark A](/macmacky)

a Full-Stack developer who likes reading Tom Clancy's books and loves
talking with dogs.

Follow

- Work
  Software Engineer
- Location
  Cebu City
- Education
  Bachelor's Degree in Computer Engineering
- Joined
  Jul 24, 2019

Author

• [Jan 6 '20](https://dev.to/macmacky/comment/jn7m)

Dropdown menu

- [Copy link](https://dev.to/macmacky/comment/jn7m)
- - [Hide](#)

---

No Problem man and Thanks 😃!

Favorite heart outline button

Favorite heart outline button

2 likes

[](#/macmacky/70-javascript-interview-questions-5gfi/comments/new/jn7m)

Comment button

Reply

Collapse

Expand

[![nataliedeweerd profile
image](https://res.cloudinary.com/practicaldev/image/fetch/s--DpuDF1Hp--/c_fill,f_auto,fl_progressive,h_50,q_auto,w_50/https://dev-to-uploads.s3.amazonaws.com/uploads/user/profile_image/158999/4d56b44c-b55e-4fa3-8f85-77331779f44b.png)](https://dev.to/nataliedeweerd)

[𝐍𝐚𝐭𝐚𝐥𝐢𝐞 𝐝𝐞 𝐖𝐞𝐞𝐫𝐝](https://dev.to/nataliedeweerd)

𝐍𝐚𝐭𝐚𝐥𝐢𝐞 𝐝𝐞 𝐖𝐞𝐞𝐫𝐝

[![](https://res.cloudinary.com/practicaldev/image/fetch/s--UMsrv0fN--/c_fill,f_auto,fl_progressive,h_90,q_auto,w_90/https://dev-to-uploads.s3.amazonaws.com/uploads/user/profile_image/158999/4d56b44c-b55e-4fa3-8f85-77331779f44b.png)
𝐍𝐚𝐭𝐚𝐥𝐢𝐞 𝐝𝐞 𝐖𝐞𝐞𝐫𝐝](/nataliedeweerd)

Full-stack web developer and proud geek. Married to a flying Dutchman.
Lover of cats.

Follow

- Location
  UK
- Education
  Computing Science, BSc
- Joined
  Apr 21, 2019

• [Jan 3 '20](https://dev.to/nataliedeweerd/comment/jl0j)

Dropdown menu

- [Copy link](https://dev.to/nataliedeweerd/comment/jl0j)
- - [Hide](#)

---

I need to brush up on my JS so this will be super helpful for me! Thank
you!

Favorite heart outline button

Favorite heart outline button

2 likes

[](#/macmacky/70-javascript-interview-questions-5gfi/comments/new/jl0j)

Comment button

Reply

Collapse

Expand

[![macmacky profile
image](https://res.cloudinary.com/practicaldev/image/fetch/s--ip3rQvUF--/c_fill,f_auto,fl_progressive,h_50,q_auto,w_50/https://dev-to-uploads.s3.amazonaws.com/uploads/user/profile_image/201157/3607fd1f-3a5f-4fdf-8421-01debc8523b7.jpg)](https://dev.to/macmacky)

[Mark A](https://dev.to/macmacky)

Author

Mark A

[![](https://res.cloudinary.com/practicaldev/image/fetch/s--11luy8FC--/c_fill,f_auto,fl_progressive,h_90,q_auto,w_90/https://dev-to-uploads.s3.amazonaws.com/uploads/user/profile_image/201157/3607fd1f-3a5f-4fdf-8421-01debc8523b7.jpg)
Mark A](/macmacky)

a Full-Stack developer who likes reading Tom Clancy's books and loves
talking with dogs.

Follow

- Work
  Software Engineer
- Location
  Cebu City
- Education
  Bachelor's Degree in Computer Engineering
- Joined
  Jul 24, 2019

Author

• [Jan 3 '20](https://dev.to/macmacky/comment/jl0p)

Dropdown menu

- [Copy link](https://dev.to/macmacky/comment/jl0p)
- - [Hide](#)

---

Glad you like it 😁

Favorite heart outline button

Favorite heart outline button

1 like

[](#/macmacky/70-javascript-interview-questions-5gfi/comments/new/jl0p)

Comment button

Reply

Collapse

Expand

[![jpelaa profile
image](https://res.cloudinary.com/practicaldev/image/fetch/s--vq0yUedR--/c_fill,f_auto,fl_progressive,h_50,q_auto,w_50/https://dev-to-uploads.s3.amazonaws.com/uploads/user/profile_image/139916/93706d4a-6e41-42f9-bf46-693f202f56bb.jpg)](https://dev.to/jpelaa)

[JP](https://dev.to/jpelaa)

JP

[![](https://res.cloudinary.com/practicaldev/image/fetch/s--B1D5D4dN--/c_fill,f_auto,fl_progressive,h_90,q_auto,w_90/https://dev-to-uploads.s3.amazonaws.com/uploads/user/profile_image/139916/93706d4a-6e41-42f9-bf46-693f202f56bb.jpg)
JP](/jpelaa)

I'm beginner front-end developer

Follow

- Work
  Frontend Developer at doodleblue
- Location
  chennai
- Joined
  Feb 24, 2019

• [Jan 4 '20](https://dev.to/jpelaa/comment/jl77)

Dropdown menu

- [Copy link](https://dev.to/jpelaa/comment/jl77)
- - [Hide](#)

---

Very detailed answers

Favorite heart outline button

Favorite heart outline button

2 likes

[](#/macmacky/70-javascript-interview-questions-5gfi/comments/new/jl77)

Comment button

Reply

Collapse

Expand

[![macmacky profile
image](https://res.cloudinary.com/practicaldev/image/fetch/s--ip3rQvUF--/c_fill,f_auto,fl_progressive,h_50,q_auto,w_50/https://dev-to-uploads.s3.amazonaws.com/uploads/user/profile_image/201157/3607fd1f-3a5f-4fdf-8421-01debc8523b7.jpg)](https://dev.to/macmacky)

[Mark A](https://dev.to/macmacky)

Author

Mark A

[![](https://res.cloudinary.com/practicaldev/image/fetch/s--11luy8FC--/c_fill,f_auto,fl_progressive,h_90,q_auto,w_90/https://dev-to-uploads.s3.amazonaws.com/uploads/user/profile_image/201157/3607fd1f-3a5f-4fdf-8421-01debc8523b7.jpg)
Mark A](/macmacky)

a Full-Stack developer who likes reading Tom Clancy's books and loves
talking with dogs.

Follow

- Work
  Software Engineer
- Location
  Cebu City
- Education
  Bachelor's Degree in Computer Engineering
- Joined
  Jul 24, 2019

Author

• [Jan 4 '20](https://dev.to/macmacky/comment/jl89)

Dropdown menu

- [Copy link](https://dev.to/macmacky/comment/jl89)
- - [Hide](#)

---

Thanks man!

Favorite heart outline button

Favorite heart outline button

1 like

[](#/macmacky/70-javascript-interview-questions-5gfi/comments/new/jl89)

Comment button

Reply

Collapse

Expand

[![pavelpotapkin profile
image](https://res.cloudinary.com/practicaldev/image/fetch/s--6BUB5gZh--/c_fill,f_auto,fl_progressive,h_50,q_auto,w_50/https://dev-to-uploads.s3.amazonaws.com/uploads/user/profile_image/307865/e12e1c02-7377-4daf-ba56-8907f16bea71.png)](https://dev.to/pavelpotapkin)

[Pavel Potapkin](https://dev.to/pavelpotapkin)

Pavel Potapkin

[![](https://res.cloudinary.com/practicaldev/image/fetch/s--vdSpC76_--/c_fill,f_auto,fl_progressive,h_90,q_auto,w_90/https://dev-to-uploads.s3.amazonaws.com/uploads/user/profile_image/307865/e12e1c02-7377-4daf-ba56-8907f16bea71.png)
Pavel Potapkin](/pavelpotapkin)

Follow

- Joined
  Jan 4, 2020

• [Jan 4 '20](https://dev.to/pavelpotapkin/comment/jl38)

Dropdown menu

- [Copy link](https://dev.to/pavelpotapkin/comment/jl38)
- - [Hide](#)

---

Thank you for the great article. It must be mistake in 1 question when
you provide example of casting null and undefined to Boolean, you cast
only null in both cases.

Favorite heart outline button

Favorite heart outline button

2 likes

[](#/macmacky/70-javascript-interview-questions-5gfi/comments/new/jl38)

Comment button

Reply

Collapse

Expand

[![macmacky profile
image](https://res.cloudinary.com/practicaldev/image/fetch/s--ip3rQvUF--/c_fill,f_auto,fl_progressive,h_50,q_auto,w_50/https://dev-to-uploads.s3.amazonaws.com/uploads/user/profile_image/201157/3607fd1f-3a5f-4fdf-8421-01debc8523b7.jpg)](https://dev.to/macmacky)

[Mark A](https://dev.to/macmacky)

Author

Mark A

[![](https://res.cloudinary.com/practicaldev/image/fetch/s--11luy8FC--/c_fill,f_auto,fl_progressive,h_90,q_auto,w_90/https://dev-to-uploads.s3.amazonaws.com/uploads/user/profile_image/201157/3607fd1f-3a5f-4fdf-8421-01debc8523b7.jpg)
Mark A](/macmacky)

a Full-Stack developer who likes reading Tom Clancy's books and loves
talking with dogs.

Follow

- Work
  Software Engineer
- Location
  Cebu City
- Education
  Bachelor's Degree in Computer Engineering
- Joined
  Jul 24, 2019

Author

• [Jan 4 '20](https://dev.to/macmacky/comment/jl3b)

Dropdown menu

- [Copy link](https://dev.to/macmacky/comment/jl3b)
- - [Hide](#)

---

Thanks man for pointing that one out.

Favorite heart outline button

Favorite heart outline button

2 likes

[](#/macmacky/70-javascript-interview-questions-5gfi/comments/new/jl3b)

Comment button

Reply

Collapse

Expand

[![mohamedelidrissi_98 profile
image](https://res.cloudinary.com/practicaldev/image/fetch/s--Z7ugdQ6Y--/c_fill,f_auto,fl_progressive,h_50,q_auto,w_50/https://dev-to-uploads.s3.amazonaws.com/uploads/user/profile_image/204762/23cac4ba-af52-4ed8-90d4-033b8f59f90d.jpg)](https://dev.to/mohamedelidrissi_98)

[Mohamed ELIDRISSI](https://dev.to/mohamedelidrissi_98)

Mohamed ELIDRISSI

[![](https://res.cloudinary.com/practicaldev/image/fetch/s--LY1RcO_2--/c_fill,f_auto,fl_progressive,h_90,q_auto,w_90/https://dev-to-uploads.s3.amazonaws.com/uploads/user/profile_image/204762/23cac4ba-af52-4ed8-90d4-033b8f59f90d.jpg)
Mohamed ELIDRISSI](/mohamedelidrissi_98)

21, full-stack web dev, future entrepreneur

Follow

- Work
  Student
- Location
  Morocco
- Joined
  Jul 31, 2019

• [Jan 3 '20](https://dev.to/mohamedelidrissi_98/comment/jkcc)

Dropdown menu

- [Copy link](https://dev.to/mohamedelidrissi_98/comment/jkcc)
- - [Hide](#)

---

This is a gem, thanks for writing this!

Favorite heart outline button

Favorite heart outline button

2 likes

[](#/macmacky/70-javascript-interview-questions-5gfi/comments/new/jkcc)

Comment button

Reply

[View full discussion (94
comments)](/macmacky/70-javascript-interview-questions-5gfi/comments)

[Code of Conduct](/code-of-conduct) • [Report abuse](/report-abuse)

## Read next {.crayons-subtitle-1}

[](/harperdb/improving-mobile-app-performance-with-a-powerful-database-7j5)

![margo_hdb profile
image](https://res.cloudinary.com/practicaldev/image/fetch/s--7oqL5T4v--/c_imagga_scale,f_auto,fl_progressive,h_100,q_auto,w_100/https://dev-to-uploads.s3.amazonaws.com/uploads/user/profile_image/399959/f8b3f1c1-a9af-4f19-855b-5c58d1644bde.jpg)

### Improving Mobile App Performance with a Powerful Database {.fs-xl .mb-0 .lh-tight}

Margo McCabe - Jul 22

[](/ionic/10-reasons-to-choose-ionic-for-mobile-development-213a)

![maxlynch profile
image](https://res.cloudinary.com/practicaldev/image/fetch/s--TV-AjASV--/c_imagga_scale,f_auto,fl_progressive,h_100,q_auto,w_100/https://dev-to-uploads.s3.amazonaws.com/uploads/user/profile_image/77831/dd90b1ab-73fc-4b3a-a63b-3e824eaccc27.jpeg)

### 10 Reasons to Choose Ionic for Mobile Development {.fs-xl .mb-0 .lh-tight}

Max Lynch - Jul 22

[](/ashutoshmishra4/amazing-mini-image-editor-with-vanilla-javascript-day-3-of-javascript30-48fh)

![ashutoshmishra4 profile
image](https://res.cloudinary.com/practicaldev/image/fetch/s--qu01Fu-4--/c_imagga_scale,f_auto,fl_progressive,h_100,q_auto,w_100/https://dev-to-uploads.s3.amazonaws.com/uploads/user/profile_image/554732/b399ca78-3bbf-46a1-9ff0-9a9b08d855e9.png)

### Amazing Mini Image Editor with Vanilla JavaScript – Day 3 of JavaScript30 {.fs-xl .mb-0 .lh-tight}

Ashutosh Mishra - Jul 22

[](/woshimbo/beginner-with-questions-21ma)

![woshimbo profile
image](https://res.cloudinary.com/practicaldev/image/fetch/s--1gN27VK_--/c_imagga_scale,f_auto,fl_progressive,h_100,q_auto,w_100/https://dev-to-uploads.s3.amazonaws.com/uploads/user/profile_image/669486/a4eff305-a0a7-4741-b030-0c62fa46926a.png)

### Beginner With Questions {.fs-xl .mb-0 .lh-tight}

Woshimbo - Jul 20

[![](https://res.cloudinary.com/practicaldev/image/fetch/s--11luy8FC--/c_fill,f_auto,fl_progressive,h_90,q_auto,w_90/https://dev-to-uploads.s3.amazonaws.com/uploads/user/profile_image/201157/3607fd1f-3a5f-4fdf-8421-01debc8523b7.jpg)
Mark A](/macmacky)

a Full-Stack developer who likes reading Tom Clancy's books and loves
talking with dogs.

Follow

- Work
  Software Engineer
- Location
  Cebu City
- Education
  Bachelor's Degree in Computer Engineering
- Joined
  Jul 24, 2019

### More from [Mark A](/macmacky) {.crayons-subtitle-2}

[How to configure Webpack with React Testing Library from the ground
up](/macmacky/how-to-configure-webpack-with-react-testing-library-from-the-ground-up-4occ)

\#testing \#react \#tutorial \#webdev

[Free Resources to Learn while in
Lockdown](/macmacky/free-resources-to-learn-while-in-lockdown-54n9)

\#webdev \#javascript \#beginners \#tutorial

[How to Debug Nodejs, TypeScript Code in
VSCode](/macmacky/how-to-debug-nodejs-typescript-code-in-vscode-4o27)

\#typescript \#tutorial \#javascript \#vscode

[DEV Community](/) – A constructive and inclusive social network for
software developers. With you every step of your journey.

Built on [Forem](https://www.forem.com) — the [open
source](https://dev.to/t/opensource) software that powers
[DEV](https://dev.to) and other inclusive communities.

Made with love and [Ruby on Rails](https://dev.to/t/rails). DEV
Community © 2016 - 2021.

[](https://www.forem.com)

Forem logo
