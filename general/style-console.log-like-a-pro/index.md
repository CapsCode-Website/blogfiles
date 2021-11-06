Hello Devs,

In this blog I will guide you all through "HOW WE CAN STYLE CONSOLE.LOG() USING CSS"
I have made 12 different styles for you to make sure that you will not ended up with any confusions.

So without wasting any time lets get into this tutorial.

1. Add `%c` before the text you want to style.
2. Insert one more argument in the console log function with the style you want to apply.

## Examples:

**1.Simple Console Log Shortcut for JS Objects with the defined color i.e #007acc**

```js
console.log("%cThis is my 1st style", "color: #007acc;", "CAPSCODE");
```

![style 1 of console](https://raw.githubusercontent.com/CapsCode-Website/blogfiles/master/general/style-console.log-like-a-pro/1.png?raw=true)

**2.JSON String Output**

```js
console.log(
  "%cThis is my 2nd style",
  "color: #007acc;",
  JSON.stringify({ fname: "JOHN", lname: "DOE" }, null, "\t")
);
```

![style 2 of console](https://raw.githubusercontent.com/CapsCode-Website/blogfiles/master/general/style-console.log-like-a-pro/2.png?raw=true)

**3.Simple Console Log Shortcut for JS Objects - Green Text**

```js
console.log("%cThis is my 4th style", "color: #26bfa5;", foo);
```

![style 3 of console](https://raw.githubusercontent.com/CapsCode-Website/blogfiles/master/general/style-console.log-like-a-pro/3.png?raw=true)

**4.Simple Console Log Shortcut for JS Objects - Blue Background**

```js
console.log(
  "%cThis is my 5th style",
  "color: white; background-color: #007acc;",
  foo
);
```

![style 4 of console](https://raw.githubusercontent.com/CapsCode-Website/blogfiles/master/general/style-console.log-like-a-pro/4.png?raw=true)

**5.Simple Console Log Shortcut for JS Objects - Green Background**

```js
console.log(
  "%cThis is my 6th style",
  "color: white; background-color: #26bfa5;",
  foo
);
```

![style 5 of console](https://raw.githubusercontent.com/CapsCode-Website/blogfiles/master/general/style-console.log-like-a-pro/5.png?raw=true)

**6.Console logs -> Hello ${TM_FILENAME} line:${TM_LINE_NUMBER} on Green Background**

```js
console.log(
  "%cThis is my 7th style",
  "background: green; color: white; display: block;"
);
```

![style 6 of console](https://raw.githubusercontent.com/CapsCode-Website/blogfiles/master/general/style-console.log-like-a-pro/6.png?raw=true)

**7.Find errors with style**

```js
console.log(
  "%cThis is my 8th style",
  "color: red; display: block; width: 100%;",
  error
);
```

![style 7 of console](https://raw.githubusercontent.com/CapsCode-Website/blogfiles/master/general/style-console.log-like-a-pro/7.png?raw=true)

**8.You need a Rainbow in your code**

```js
console.log(
  "%c CapsCode!",
  "font-weight: bold; font-size: 50px;color: red; text-shadow: 3px 3px 0 rgb(217,31,38) , 6px 6px 0 rgb(226,91,14) , 9px 9px 0 rgb(245,221,8) , 12px 12px 0 rgb(5,148,68) , 15px 15px 0 rgb(2,135,206) , 18px 18px 0 rgb(4,77,145) , 21px 21px 0 rgb(42,21,113); margin-bottom: 12px; padding: 5%"
);
```

![style 8 of console](https://raw.githubusercontent.com/CapsCode-Website/blogfiles/master/general/style-console.log-like-a-pro/8.png?raw=true)

**9.Confused?! so put a this guy in your code.**

```js
console.log(
  "%c ",
  "font-size: 1px; padding: 166.5px 250px; background-size: 500px 333px; background: no-repeat url(https://www.capscode.in/static/media/cap.0d0af8f0.png);"
);
```

![style 9 of console](https://raw.githubusercontent.com/CapsCode-Website/blogfiles/master/general/style-console.log-like-a-pro/9.png?raw=true)

**10.Simple Console Log Shorcut for JS Objects - Green Text**

```js
console.log(
  "%c ",
  "font-size: 1px; padding: 240px 123.5px; background-size: 247px 480px; background: no-repeat url(https://www.capscode.in/static/media/cap.0d0af8f0.png);"
);
```

![style 10 of console](https://raw.githubusercontent.com/CapsCode-Website/blogfiles/master/general/style-console.log-like-a-pro/10.png?raw=true)

**11.Celebrate your code works!**

```js
console.log(
  "%c ",
  "font-size: 1px; padding: 125px 125px; background-size: 250px 250px; background: no-repeat url(https://i2.wp.com/i.giphy.com/media/12BYUePgtn7sis/giphy-downsized.gif?w=770&amp;ssl=1);"
);
```

![style 11 of console](https://raw.githubusercontent.com/CapsCode-Website/blogfiles/master/general/style-console.log-like-a-pro/11.png?raw=true)

**12.Coding GIF**

```js
console.log(
  "%c ",
  "font-size: 1px; padding: 215px 385px; background-size: 770px 430px; background: no-repeat url(https://i0.wp.com/i.giphy.com/media/ZVik7pBtu9dNS/giphy-downsized.gif?w=770&amp;ssl=1);"
);
```

![style 12 of console](https://raw.githubusercontent.com/CapsCode-Website/blogfiles/master/general/style-console.log-like-a-pro/12.png?raw=true)

That all in this article, hope you all have enjoyed it.

### IF MY ARTICLE HELPED YOU

<a href="https://www.buymeacoffee.com/capscode" target="_blank"><img src="https://cdn.buymeacoffee.com/buttons/default-orange.png" alt="Buy Me A Coffee" height="41" width="174"></a>

Thanks,

CapsCode
