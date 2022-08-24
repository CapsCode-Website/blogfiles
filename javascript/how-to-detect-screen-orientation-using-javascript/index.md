Hello Devs,

In this blog we will see "How to detect screen orientation using JavaScript".

Below are the most useful ways to get/ detect the orientation of the screen/ device using JavaScript.

without wasting time, lets get into the blog,

## **1. How to detect screen orientation using `window` object**

```js
if (window.innerHeight > window.innerWidth) {
  alert("You are in portrait mode");
}

if (window.innerHeight < window.innerWidth) {
  alert("You are in landscape mode");
}
```

## **2. How to detect screen orientation using `window.screen` object**

On mobile devices, if you open a keyboard then the above may fail, so we can use `screen.availHeight` and `screen.availWidth`, which gives proper height and width even after the keyboard is opened.

```js
if (screen.availHeight > screen.availWidth) {
  alert("You are in portrait mode");
}

if (screen.availHeight < screen.availWidth) {
  alert("You are in landscape mode");
}
```

#### **or**

```javascript
if (screen.height > screen.width) {
  alert("You are in portrait mode");
}

if (screen.height > screen.width) {
  alert("You are in landscape mode");
}
```

## **3. How to detect screen orientation using `screen.orientation.type`**

```javascript
if (
  orientation === "portrait-secondary" ||
  orientation === "portrait-primary"
) {
  alert("You are in portrait mode");
}

let orientation = screen.orientation.type;
if (orientation === "landscape-primary") {
  alert("You are in landscape mode");
}

if (orientation === "landscape-secondary") {
  alert("You are in landscape mode with screen as upside down");
}

if (orientation === undefined) {
  alert("orientation not supported in current browser");
}
```

## **4. How to detect screen orientation using `matchMedia`**

```javascript
if (window.matchMedia("(orientation: portrait)").matches) {
  alert("You are in portrait mode");
}

if (window.matchMedia("(orientation: landscape)").matches) {
  alert("You are in landscape mode");
}
```

Thank you for reading this so far. This is a brief introduction on **How to Detect Screen Orientation using JavaScript** .
If you find this article useful, like and share this article. Someone could find it useful too.

If you find anything technically inaccurate please feel free to comment below.

Hope its a nice and informative read for you.
VISIT https://www.capscode.in/blog TO LEARN MORE...
See you in my next Blog article, Take care!!

Thanks,\
CapsCode
