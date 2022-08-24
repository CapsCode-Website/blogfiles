Hello Devs,

If you are a web developer then you must know this concept of JavaScript i.e VOID / VOID(0)
In this article i am going to tell you everything about VOID operator in JavaScript.
So without wasting any time, lets get into the article

## Table of contents

| No. | Topic                                                                 |
| --- | --------------------------------------------------------------------- |
| 1   | [What is Void ?](#what-is-void)                                       |
| 2   | [What is the use of VOID operator](#what-is-the-use-of-void-operator) |
| 3   | [When to use Javascript void(0)](#when-to-use-javascript-void)        |
| 4   | [why to use void ](#why-to-use-void)                                  |

### What is VOID ?

**void**: void means completely empty/ or nothing
NOTE: null and void are different

**[⬆ Back to Top](#table-of-contents)**

### What VOID operator do ?

void operator in JS evaluates the given expression and then returns undefined

syntax:
void(2+3) //this evaluated 2+3 and return undefined:
lets prove this
void(console.log(2+3))//this will print 5 but return undefined

**[⬆ Back to Top](#table-of-contents)**

### What is the use of VOID operator ?

use of void(0) in `<a>` tag
Void(0) is used to prevent the page from refreshing and parameter "zero" is passed while calling.
Void(0) is used to call another method without refreshing the page.

**[⬆ Back to Top](#table-of-contents)**

### When to use Javascript void ?

We can use Javascript void(0) when we do not want the browser to load a new page or refresh the same page​ when a link is clicked. Instead, we want the browser to perform the Javascript attached to that link.

**[⬆ Back to Top](#table-of-contents)**

### why to use void ?

```html
<a href="" onclick="alert('The page will reload!!!')"
  >Click Here to display alert!</a
>
```

<a href="" onclick="alert('The page will reload!!!')">Click Here to display alert!</a>
**_this will show alert and then reload the page._**

```html
<a href="javascript:void(0);" onclick="alert('The page will not reload.')"
  >Click Here to display alert!</a
>
```

<a href="javascript:void(0);" onclick="alert('The page will not reload.')">Click Here to display alert!</a>
**_this will alert but will not reload the page._**

We can also run any JS code without reloading or refreshing the page.

```html
<a
  id="link"
  href="javascript:void(document.querySelector('#link').style.color = 'green')"
  >Link</a
>
```

Another use case of links with the **javascript:void(0)** reference is that sometimes, a link may run some JavaScript code in the background, and navigating may be unnecessary. In this case, the expressions would be used as the arguments passed to void.

> A common usage of JavaScript:Void(0) is with hyperlinks.

Sometimes, you may need to call some JavaScript from within a link. Normally, when you click a link, the browser loads a new page or refreshes the same page (depending on the URL specified). But you probably don't want this to happen if you've attached some JavaScript to that link.

To prevent the page from unnecessary refreshing, you could use **JavaScript:void(0)**.

some additional examples:

```html
<a href="#" ondblclick="alert('Well done!')">Double Click Me!</a>
```

<a href="#" ondblclick="alert('Well done!')">Double Click Me!</a>
--page refreshed as soon you clicked the link

```html
<a href="JavaScript:void(0);" ondblclick="alert('Well done!')"
  >Double Click Me!</a
>
```

<a href="JavaScript:void(0);" ondblclick="alert('Well done!')">Double Click Me!</a>
--this don't

**[⬆ Back to Top](#table-of-contents)**

Thank you for reading this far. This is a brief introduction of **VOID in JS** .
If you find this article useful, like and share this article. Someone could find it useful too. If you find anything technically inaccurate please feel free to comment below.
Now you can also play around the objects in JS.

Hope its a nice and informative read for you.
VISIT https://www.capscode.in/blog TO LEARN MORE...

### IF MY ARTICLES HELPED YOU

<a href="https://www.buymeacoffee.com/capscode" target="_blank"><img src="https://cdn.buymeacoffee.com/buttons/default-orange.png" alt="Buy Me A Coffee" height="41" width="174"></a>

Thanks,\
CapsCode
