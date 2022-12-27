Hello Devs,

CSS variables are the most important topic that most developers ignore learning and due to this, they miss out on doing some of the complicated stuff of CSS in a single line of code.
In this article, we will learn all the important aspects and uses of CSS variables.


## Table of content
1. [What are CSS variables](#what-are-css-variables)
2. [How to declare CSS variable](#how-to-declare-css-variable)
3. [How to consume CSS variable](#how-to-consume-css-variable)
4. [Scope of CSS variable](#scope-of-css-variable)
5. [How to reassign value to CSS variable](#how-to-reassign-value-of-css-variable)
6. [Hoisting in CSS variable](#hoisting-in-css-variable)
7. [CSS variable in media-query](#css-variable-in-media-query)
8. [Change CSS variable value using JavaScript](#change-css-variable-value-using-javascript)
9. [CSS variable inheritance](#css-variable-inheritance)
10. [Additional -- CSS functions & methods](#additional)


## 1. What are CSS variables <a name="what-are-css-variables"></a>
CSS variables are just like the normal variables in any programming language. We can define the variable, assign & reassign the value to it and use it within their scope.

---
## 2. How to declare CSS variable <a name="how-to-declare-css-variable"></a>
To declare CSS Variable we use `--`

syntax:

```css
--varName: value
```
---
## 3. How to consume CSS variable <a name="how-to-consume-css-variable"></a>
To consume variables in CSS, we use  `var(name, value)`
where,
name: is required and it will be the name of the variable (must start with --)
value: optional the default value which will be used if the name variable is not found

syntax:
```css
css-property : var(--varName, defaultValue)
```
---
## 4. Scope of a CSS variable <a name="scope-of-css-variable"></a>
Here comes the most important and interesting part of CSS variables i.e the Scope of CSS variables.
To begin with this we will first see what is scope in CSS and how we can define it.
Generally, a CSS variable is only visible to child elements of the parent element it is declared in.

```css
:root{
    any variable defined here can be accessible across the document (all the element inside <html> tag).
    CSS variables declared in the :root selector are said to be in the Global scope
}

element:{
    any variable defined here can be accessible within all of its children
}

.className{
    any variable defined here can be accessible only for the class="className" and by its children elements, classes, ids (as its locally defined only for class className)
}

#idName{
    any variable defined here can be accessible only for the id="idName" and by its children elements, classes, ids (as its locally defined only for id idName)
}
```

**NOTE:** Local variable will override global

Now let's see some examples,

### 1. defining a global variable

**Syntax**
```css
:root{
    --lightcolor: lightgrey;
}

div{
    background-color: var(--lightcolor)
}

button{
    background-color: var(--lightcolor)
}
```

**Example**

```html
<body>
    <div>
      Div 1
    </div>

    <div>
      Div 2
    </div>

    <button>
        click
    </button>
</body>
```

```css
:root {
  --themecolorlight: #93beec;
  --themecolordark: #8395a7;
  /* the CSS variable --themecolorlight and --themecolordark is accessible throughout the document. */
}

div {
  background-color: var(--themecolorlight);
}

button{
    background-color: var(--themecolordark);
}
```


### 2. Declaring variable inside the element
 
**Syntax**
```css
body{
--lightcolor: lightgrey;
}
/* this CSS variable are accessible to all the elements, ids, classes which are inside body tag or children of body tag */

div{
    background: var(--lightcolor)
}
/* this CSS variable are accessible to all the elements, ids, classes which are inside div tag or children of div tag */
```

**Example**

```html
<body>
    <div>
      <h1>
        Heading 1
      </h1>
      <h1 class="heading2">
        Heading 2 with class heading2
      </h1>
      <h1 id="heading3">
        Heading 3
      </h1>
    </div>
</body>
```

```css
body {
  --lightcolor: #ea7773;
  --lightcolor2: yellow;
  --lightcolor3: green;
}

h1 {
  background-color: var(--lightcolor);
}

.heading2 {
  background-color: var(--lightcolor2);
}
#heading3 {
  background-color: var(--lightcolor3);
}
```


for the above HTML,
```css
div {
    --bgColor: limegreen;
}
body {
    background: var(--bgColor);
}
```

The body will unable to get the bgColor variable value (i.e limegreen), because the body is not the child of the div element. But the elements which are children of div can use the bgColor variable.

### 3. declaring a variable inside the class name

**Syntax**

```css
.container{
    background: var(--lightcolor)
}
/* this CSS variable are accessible to all the elements, ids, classes which are inside container class or children of container class */

/* Any element which are outside of container call and accessing the lightcolor variable will unable to set the lightcolor value */
```

**Example**
```html
<body>
    <div class="container">
      <h2>
        container Heading 1
      </h2>
      <h2 class="containerHeading2">
        container Heading 2 with class heading2
      </h2>
      <h2 id="containerHeading3">
        container Heading 3
      </h2>
    </div>

    <h2>
      Heading outside of container but inside the body
    </h2>
</body>
```


```css
.container {
  --containerlightcolor: #cf9fff;
  --containerlightcolor2: #e74292;
  --containerlightcolor3: #022599;
}
h2 {
  background-color: var(--containerlightcolor);
  /* h2 with text "Heading outside of container but inside the body" will not get this variable color as its outside of container class */
}

.containerHeading2 {
  background-color: var(--containerlightcolor2);
}
#containerHeading3 {
  background-color: var(--containerlightcolor3);
}
```
---
### 4. declaring a variable inside the id

**Syntax**
```css
#header{
       background: var(--lightcolor) 
}
```

**Example**

works the same as classes


---
## 5. How to reassign the value of the CSS variable <a name="how-to-reassign-value-of-css-variable"></a>

**local variable will override global**

```css
    :root{
        --buttoncolor: red
    }

    button{
        --buttoncolor:blue
        background-color: var(--buttoncolor)
    }

```
---
## 6. Hoisting in CSS Variable <a name="hoisting-in-css-variable"></a>

Just like JavaScript functions CSS variables are hoisted and can be used before their declaration

```css
body {
    background-color: var(--bgColor);
}

:root {
    --bgColor:black;
}
```
The above code will run perfectly fine and the body will be able to give a background of black.
This feature is very important to keep in mind while declaring variables in CSS.

Hoisting of CSS variable works similarly to functions of JavaScript

---
## 7. CSS variable in media-query <a name="css-variable-in-media-query"></a>

```html
<body>
<h1>Using Variables in Media Queries</h1>

<div class="container">
<div class="container2">
  <h2>Lorem Ipsum</h2>
  <p>When the browser's width is 450px or wider, set the --fontsize variable value to 50px and the --blue variable value to lightblue. Resize the browser window to see the effect.</p>
  </div>
</div>

</body>
```
```css
.container {
  --fontsize: 5px;
}

div{
  font-size: var(--fontsize);
  /* all the div's inside container will take the font-size as 5px for screen size smaller than 450px */
}

@media screen and (min-width: 450px) {
  .container {
    --fontsize: 50px;
  }
  :root {
    --themecolorlight: lightblue;
  }
  /* all the div's inside container will take the font-size as 50px for screen size bigger than 450px */
}
```

Now the twist that comes here is,
if we define --fontsize: 50px in the :root inside a media query, then it will not work as expected for a screen size bigger than 450px.
```css
@media screen and (min-width: 450px) {
  :root {
    --blue: lightblue;
    --fontsize: 50px;
  }
}
```

because for the container class we have defined the --fontsize as a local variable, it will use the local variable --fontsize and we know that the **local variable will override global**.
if we reassign the --fontsize variable with a different value then it should be within the container class only as we have seen above.

If we redefine the --fontsize variable in container2 then everything will work perfectly fine.
```css
@media screen and (min-width: 450px) {
  :root {
    --blue: lightblue;
  }
  .container2{
  --fontsize: 150px;
  }
}
```
as container2 is the child of container and div is the child of container2 as well.

---
## 8. Change CSS variable value using JavaScript <a name="change-css-variable-value-using-javascript"></a>

```js
var r = document.querySelector(':root');
console.log(getComputedStyle(r))
r.style.setProperty('--buttoncolor', 'lightblue');
```


---
## 9. CSS variable inheritance <a name="css-variable-inheritance"></a>

Just like CSS properties, CSS variables also are cascading in nature (i.e they inherit).
The value of an element is inherited from its parent if no custom property is defined.

```html
<div class="container">
  <div class="container-item-1">
    <h1 class="container-text-1">I am h1 of container item 1</h1>
  </div>
  <div class="container-item-2">
    <h1 class="container-text-2">I am h1 of container item 2</h1>
  </div>
</div>
```

```css
.container{
  --bgColor: red
}
.container-text-1{
  background:var(--bgColor)
  /* this will make container-item-1 red */
}

.container-item-2{
  --bgColor: green
}
.container-text-2{
  background:var(--bgColor) 
  /* this will make container-item-2 green */
}

```


the background color of container-item-1 and container-item-2 will be different because the element, class or id will inherit from its nearest parent and that is the reason for different background colors for container-item-1 and container-item-2.

---
## 10. Additional <a name="additional"></a>

Just for a side note, we should be aware of the CSS Methods and Functions.
The best resource to read is from [MDN](https://developer.mozilla.org/en-US/docs/Web/CSS/CSS_Functions)

---



Thank you for reading this so far. This is a brief introduction to **Variables In CSS** and its different aspects.

You can check out some of the examples in our [codesandbox](https://codesandbox.io/s/example2-nqx5qm?file=/index.css).

Hope it's a nice and informative read for you. If you find this article useful, like and share this article. Someone could find it useful too.

If you find anything technically inaccurate, please feel free to reach out to us.

VISIT https://www.capscode.in/blog TO LEARN MORE.

See you in my next Blog article, Take care!!

Thanks,\
CapsCode