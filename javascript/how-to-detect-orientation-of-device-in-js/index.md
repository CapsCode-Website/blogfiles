how to get the detect orientation using javascript.

1. using window object

```js
if (window.innerHeight > window.innerWidth) {
  alert("Please use Landscape!");
}
```

2. using window.screen object
   On mobile devices, if you open a keyboard then the above may fail, so can use `screen.availHeight` and `screen.availWidth`, which gives proper height and width even after the keyboard is opened.

```JS
if(screen.availHeight > screen.availWidth){
    alert("Please use Landscape!");
}
```

#### **or**

```javascript
if (screen.height > screen.width) {
  alert("Please use Landscape!");
}
```

3. using screen.orientation.type

```js
let orientation = screen.orientation.type;
if (orientation === "landscape-primary") {
  console.log("you are in landscape mode");
}
if (orientation === "landscape-secondary") {
  console.log("you are in landscape mode with screen as upside down!");
}
if (
  orientation === "portrait-secondary" ||
  orientation === "portrait-primary"
) {
  console.log("you are in portrait mode");
}
if (orientation === undefined) {
  console.log("orientation not supported in current browser");
}
```

4. using matchMedia

```javascript
if (window.matchMedia("(orientation: portrait)").matches) {
  // you're in PORTRAIT mode
}

if (window.matchMedia("(orientation: landscape)").matches) {
  // you're in LANDSCAPE mode
}
```
