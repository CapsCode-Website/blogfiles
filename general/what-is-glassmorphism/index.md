Hey Devs,

This is CapsCode.
Without wasting much time lets start with the TOP UI DESIGN TREND OF 2021 (i.e Glassmorphism)
As we all are aware that Neumorphism was the most used/ loved design in 2020, with the starting is new year we are also entering into the new design trend in place of Neumorphism i.e Glassmorphism.
This UI design is really an amazing and more interesting than Neumorphism.

### _DEMO_:

![demo-image](https://raw.githubusercontent.com/CapsCode-Website/blogfiles/master/General/what-is-glassmorphism/output.jpg?raw=true)

Lets start creating Glassmorphism designs.

**prerequisite:** basic html, css tags only

Lets create **index.html** file as below:

```html
<!DOCTYPE html>
<html>
  <head>
    <link rel="stylesheet" href="index.css" />
  </head>
  <body>
    <div class="wrap">
      <h1>< CapsCode /></h1>
      <p>Visit: www.capscode.in</p>
      <div class="drop drop1">
        <div class="drop drop2"></div>
        <div class="drop drop3"></div>
        <div class="drop drop4"></div>
      </div>
    </div>
  </body>
</html>
```

then we will add css to these elements:
so lets create **index.css** file,

```css
html,
body {
  width: 100%;
  min-height: 100%;
  overflow: hidden;
  min-height: 99vh;
}

body {
  background: #ea7773;
  display: flex;
  align-items: center;
  justify-content: center;
}

.wrap {
  position: relative;
}

h1 {
  font-family: Arial;
  color: black;
  font-size: 9em;
  padding: 20px 30px;
}

p {
  font-family: Arial;
  color: black;
  font-size: 2em;
}

.drop {
  background: rgba(255, 255, 255, 0.4);
  border-radius: 10px;
  border: 1px solid rgba(255, 255, 255, 0.2);
  position: absolute;
  backdrop-filter: blur(5px);
  -webkit-backdrop-filter: blur(5px);
  display: block;
  margin: 0 auto;
}

.drop1 {
  width: 57%;
  height: 250px;
  top: 56px;
  left: 0;
  right: 0;
  z-index: 2;
  backdrop-filter: blur(5px);
  -webkit-backdrop-filter: blur(5px);
}

.drop2 {
  width: 90px;
  height: 90px;
  top: -30px;
  left: -80%;
  right: 0;
  z-index: 4;
}

.drop3 {
  width: 100px;
  height: 60px;
  top: 220px;
  right: 30px;
  z-index: 3;
}

.drop4 {
  width: 100px;
  height: 100px;
  border-radius: 50%;
  top: -90px;
  right: -80px;
}
```

that's it my dear devs :)

we are done with how to create Glassmorphism designs, now you can customize it as much as you want.

If you like it please give a 👍

Thank you,

CapsCode

www.capscode.in

www.myemoji.ml
