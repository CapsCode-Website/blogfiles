Hello Devs,

Is it possible to style console.log() in JavaScript ?
Its YES.

Have you ever tried this ?
If No, then lets do it together in these 2 simple steps.

1. Add %c before the text you want to style.
2. Insert one more argument in the console log function with the style you want to apply.

Do Checkout some of these examples:

```javascript
console.log(`I LOVE 💜 %c${name}`, "color: green");
```

> will produce

> ![Alt Text](https://raw.githubusercontent.com/CapsCode-Website/blogfiles/master/javascript/style-console-in-javascript/1.jpg?raw=true)

---

```javascript
console.log(`I LOVE 💜 %c${name}`, "color: red; font-size: 50px");
```

> will produce

> ![Alt Text](https://raw.githubusercontent.com/CapsCode-Website/blogfiles/master/javascript/style-console-in-javascript/2.jpg?raw=true)

---

```javascript
console.log(`%cI LOVE 💜 %c${name}`, "color: red; font-size: 50px");
```

> will produce

> ![Alt Text](https://raw.githubusercontent.com/CapsCode-Website/blogfiles/master/javascript/style-console-in-javascript/3.jpg?raw=true)

If you liked this, please let me know in the comment.

Thanks,\
CapsCode
