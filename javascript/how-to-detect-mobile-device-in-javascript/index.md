Hello Devs,

In this blog, we are going to learn that how you can detect mobile device or browser or OS using JavaScript and you can redirect the user to the mobile application or to the web application automatically.

## Table of content

1. [What is navigator object in JavaScript ](#one)
2. [Properties of navigator object](#two)
3. [How to detect mobile device or browser or OS](#three)
4. [How to detect mobile device or browser or OS in Production](#four)

So without wasting any time, lets get into the tutorial.

### 1.What is `navigator` object in JavaScript <a name="one"></a>

To get the bowser details or device details, JavaScript stores these information in the `navigator` property of `window` object.
`navigator` object contains lots of information about the browser, some of the most used/ important information we will see later in this tutorial.

Lets first see what `navigator` object is.
if you directly want to see how to get the detect mobile and desktop then you can skip this part can click [here](#three)

**`navigator` object contains information about the browser.**
(NOTE: Not all but all major browser support this object)

### 2.Some of the most important properties are,

<a name="two"></a>

1. `Clipboard` - used to copy something to clipboard and paste it any where (Ex. while making Click to copy)
2. `connection`
3. `language` - shows the language of browser.
4. `geolocation` - Returns a Geolocation object that can be used to locate the user's position
5. `onLine` - check whether the browser is online
6. `platform` - machine type where browser is installed.
7. `cookieEnabled` - it returns a Boolean value that indicates whether cookies are enabled or not.
8. `serviceWorker` - mainly used to checks if the browser supports service workers
9. `vibrate(time)` - make device vibrate if it support that
10. `userAgent` - _will see below_
11. `userAgentData` - _will see below_

I think this much information about the navigator object is enough to understand what is `navigator` object and what all information it contains

Now, let see

### 3.How to detect mobile device or browser or OS. <a name="three"></a>

To get these information we will use the property `userAgent`, `userAgentData` of navigator object.

**`navigator.userAgent`**
`userAgent` will give you the information of lot of things like device name, browser name, OS version but the information returned by browser is not much understandable.
So, we can understand these returned information from the hack.

to get OS version and name you can follow the below hack,

```js
if (window.navigator.userAgent.indexOf("Windows NT 10.0") != -1) {
  console.log("OS is Windows 10");
}

if (window.navigator.userAgent.indexOf("Windows NT 6.3") != -1) {
  console.log("OS is Windows 8.1");
}

if (window.navigator.userAgent.indexOf("Windows NT 6.2") != -1) {
  console.log("OS is Windows 8");
}

if (window.navigator.userAgent.indexOf("Windows NT 6.1") != -1) {
  console.log("OS is Windows 7");
}

if (window.navigator.userAgent.indexOf("Windows NT 6.0") != -1) {
  console.log("OS is Windows Vista");
}

if (window.navigator.userAgent.indexOf("Windows NT 5.1") != -1) {
  console.log("OS is Windows XP");
}

if (window.navigator.userAgent.indexOf("Windows NT 5.0") != -1) {
  console.log("OS is Windows 2000");
}

if (window.navigator.userAgent.indexOf("Mac") != -1) {
  console.log("OS is Mac/iOS");
}

if (window.navigator.userAgent.indexOf("X11") != -1) {
  console.log("OS is UNIX");
}

if (window.navigator.userAgent.indexOf("Linux") != -1) {
  console.log("OS is Linux");
}
```

to check mobile device info you can follow below hack,

```js
function detectMobile() {
  const toMatch = [
    /Android/i,
    /webOS/i,
    /iPhone/i,
    /iPad/i,
    /iPod/i,
    /BlackBerry/i,
    /Windows Phone/i,
  ];

  return toMatch.some((toMatchItem) => {
    return navigator.userAgent.match(toMatchItem);
  });
}
```

`userAgent` is much more complex to get these details.
So we have one more property i.e.
**`navigator.userAgentData`**
This gives the information about browser and mobile detection in 1 line.

```js
navigator.userAgentData.mobile; //returns true or false, depending on the condition
```

**NOTE**: Both of these 2 ways are not recommended to be use in the production.

So lets now see the best way to do so,

### 4.Better way is,<a name="four"></a>

using **`matchMedia`**
it gives you more flexibility to decide that after what screen size you want to deal it as mobile or desktop and lot of other info,
please check official doc from MDN, [MDN - Media Query](#https://developer.mozilla.org/en-US/docs/Web/API/Window/matchMedia)
[MDN- Media Query Features](#https://developer.mozilla.org/en-US/docs/Web/CSS/Media_Queries/Using_media_queries#media_features)
[About Pointer](#https://developer.mozilla.org/en-US/docs/Web/CSS/@media/pointer)

```js
function DetectDevice() {
  let isMobile = window.matchMedia || window.msMatchMedia;
  if (isMobile) {
    let match_mobile = isMobile("(pointer:coarse)");
    return match_mobile.matches;
  }
  return false;
}

DetectDevice(); //return true if mobile, and return false if desktop
```

matchMedia also gives you the right to let you choose that after what screen-size you want to treat the device as Mobile(same as CSS Media Query) and its much more flexible than `navigator` object.

```js
if (window.matchMedia("only screen and (max-width: 760px)")) {
  //do something you want to for the screen size less than 760
}
```

_we can also use `window` and `screen` object achieve this, but these are the older way and much complicated in bigger applications._

```js
if(window.innerWidth > 768){//do something}
if(screen.width > 768){//do something}
```

Thank you for reading this far. This is a brief introduction on **How to Detect Mobile Screen & OS using JavaScript** .
If you find this article useful, like and share this article. Someone could find it useful too.

If you find anything technically inaccurate please feel free to comment below.

Hope its a nice and informative read for you.
VISIT https://www.capscode.in/blog TO LEARN MORE...
See you in my next Blog article, Take care!!

Thanks,\
CapsCode
