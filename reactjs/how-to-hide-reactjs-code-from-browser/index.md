Hello Devs,

In this blog post I am going to tell you something about hiding `ReactJS` code in production server.

## Table of content

1. [Introduction](#introduction)
2. [What makes your source code visible in the browser](#map-file-in-reactjs)
3. [Hide your ReactJS code using `.env` file](#env-file-in-reactjs)
4. [Hide ReactJS code using package.json file](#hide-reactjs-code-in-windows-and-linux)
5. [Hide ReactJS code using cross-env library](#cross-env-library-to-hide-reactjs-code)
6. [Custom JavaScript file to hide ReactJS code](#delete-map-file-in-reactjs)
7. [Conclusion](#conclusion)

## 1.Introduction <a name="introduction"></a>

I am assuming that you have developed a `ReactJS` application using `create-react-app` (CLI tool for setting up a boilerplate setup to make React apps.)or your own `webpack` configuration and also deployed it in some hosting platform like Netlify, Vercel, Heroku, Azure, AWS etc.
But have you ever opened your website and in developers tool of your browser, have you ever checked the source tab of it.
If not! Please go to your website and check whether your `ReactJS` codes are visible to public or not like below.

![codeinbrowser](https://raw.githubusercontent.com/CapsCode-Website/blogfiles/master/reactjs/how-to-hide-reactjs-code-from-browser/1.JPG?raw=true)

If you have your code visible like this, then you are in the correct place in this Planet to hide your `ReactJS` codes.
By the end of this blog post I will show you what are the different possible ways to hide the `ReactJS` codes in production environment and their advantages/ disadvantages.

If you already know how to hide the `ReactJS` codes what I would recommend you to have a glance at this blog and the other possible ways and let me know in the comment whether you are knowing that or not.

## 2.What makes your `ReactJS` source code visible in the browser <a name="map-file-in-reactjs"></a>

---

Its map files, but what are they ?

**_If you are in hurry to remove only hide your reactjs code from production then go to next topic [Hide your ReactJS Code](#env-file-in-reactjs)_**

When you are building reactjs code, babel converts `JSX` into the native `JavaScript` code (minified `JavaScript` file) which is difficult to debug **withing your components** when any error comes, so webpack and babel creates a map file (map files are JSON blob which are non readable by Humans).

A `sourcemap` is a mapping between the generated/transpiled/minified `JavaScript` file and one or more original source files. The main purpose of `sourcemaps` is to aid debugging. Basically, if there’s an error in the generated code file, the map can tell you the original source file location.

Now back to the code,

We run `npm run build` command to create a build folder of your `ReactJS` app which we deploy to run our application in Production.

Have you ever checked what this build folder consists of ?
Build folder consists of the minified version of you `ReactJS` application which includes HTML, CSS, and JavaScript files. It also includes `map` files.

**Please check you map files inside build\static\js.**

![image of map files](https://raw.githubusercontent.com/CapsCode-Website/blogfiles/master/reactjs/how-to-hide-reactjs-code-from-browser/2.JPG?raw=true)

NOTE : if you deploy this build file then your code will be visible in the browser.
so you can delete the map files manually and then deploy the build folder, but that's not the correct way of doing so and thats not the way any developer likes to do.

In your localhost (dev environment) webpack auto generates the `sourcemap` files so that you can see the line numbers of the error(if any) in your code

So, without wasting time, lets begin

Here are different ways for hiding your `ReactJS` code from browsers,

## 3. Hide your ReactJS code using `.env` file. <a name="env-file-in-reactjs"></a>

---

create `.env` file in the root of your `ReactJS` application (the place where src folder is there not inside the src folder or else in the same path where package.json is defined)

Now, add below line of code in it

```javascript
GENERATE_SOURCEMAP = false;
```

and then make a build of your `ReactJS` app using command `npm run build`

What it will do is, it will create a build folder without the map files[link of above topic of map file]. You can go inside the build\static\js

![image of the build folder without map files](https://raw.githubusercontent.com/CapsCode-Website/blogfiles/master/reactjs/how-to-hide-reactjs-code-from-browser/3.JPG?raw=true)

This way to generating build folder is not Operating System dependent.

Deploy the app now and you cannot see the code in source tab in developers tool of your browser

## 4.Using `package.json` file. <a name="hide-reactjs-code-in-windows-and-linux"></a>

---

The way of remove map files using this way is OS dependent
lets open the `package.json` file and go to script object and change your build command like below,

2.1 In Windows OS:

```javascript
"build": "set \"GENERATE_SOURCEMAP=false\" && react-scripts build"
//The && DOES NOT work in the PowerShell but WORKS in cmd, so make sure in which CLI you are writing npm run build
```

2.2 In Linux OS:

```javascript
"build": "GENERATE_SOURCEMAP=false react-scripts build",
```

2.3 configure build command to auto delete the map files.

2.3.1

```js
"build": "react-scripts build && rm build/static/js/\*.map",
//creating and deleting .map files
```

2.3.2

```js
"build": "rimraf ./build && react-scripts build && rimraf ./build/\*_/_.map"
```

2.3.3

```js
"build":"react-script build && del build/static/js/\*.map"
```

2.4 use `postBuild` command to auto delete map files.

```js
"build":"react-script build"
"postBuild":"rimraf build /\*_/_ .map"
//this will delete all the .map file post build generation
//not the recommened way becaue why to generate the map file if you are deleting it again

```

NOTE: What is prebuild and postbuild ?

```js
"prebuild": "echo I run before the build script",
"build": "react-scripts build",
"postbuild": "echo I run after the build script",
 //prebuild and postbuild runs automatically before and after build command respectively
```

2.5 using regex to delete the map files from build folder

```js
"build": "node scripts/build.js && yarn run delete-maps",
"delete-maps": "yarn run delete-map-files && yarn run delete-references-to-map-files",
"delete-map-files": "find ./build -name '_.map' -delete",
"delete-references-to-map-files": "find ./build -regex '._\\.\\(js\\|css\\)' -exec sed -i -E '\\/[\\*\\/]#\\ssourceMappingURL=main(\\.[0-9a-f]+)?\\.(css|js)\\.map(\\\*\\/)?/g' {} +"
```

NOTE: "Removing only the .map files" sadly isn't enough. The build also enerates a asset-manifest.json file that contains references to that map files.

## 5.using `cross-env` library <a name="cross-env-library-to-hide-reactjs-code"></a>

---

install `cross-env` library in devDependency

```js
npm install --save-dev cross-env
```

Just use NPM package cross-env. Super easy. Works on Windows, Linux, and all environments.
then ,

```js
"build": "cross-env GENERATE_SOURCEMAP=false react-scripts build",
```

Notice that you don't use && to move to the next task.

```js
"scripts": {
"build": "cross-env NODE_ENV=production OTHERFLAG=myValue webpack --config build/webpack.config.js"
}
```

Notice that if you want to set multiple global vars, you just state them in succession, followed by your command to be executed.

## 6.Build you custom js file to delete map files <a name="delete-map-file-in-reactjs"></a>

---

```js
"build": "react-scripts build",
"postbuild": "node ./delete-sourcemap.js",
```

Create a new script called delete-sourcemap.js in your project's root folder:
const fs = require('fs')

```javascript
function deleteMaps(dir) {
  fs.readdir(dir, function (err, files) {
    files.forEach((file) => {
      if (/\.map$/.test(file)) {
        fs.unlinkSync(dir + file);
      } else {
        fs.readFile(dir + file, "utf8", (err, data) => {
          let result = data.split("\n");
          console.log(result.length);
          if (result[result.length - 1] !== undefined && result.length > 1) {
            fs.writeFileSync(
              dir + file,
              result.slice(0, result.length - 1).join("\n")
            );
          }
        });
      }
    });
  });
}

["./build/static/css/", "./build/static/js/"].map(deleteMaps);
```

## Conclusion <a name="conclusion"></a>

---

Awesome! Now you become an expert in hiding the `ReactJS` code from the Production environment. I hope you have now a very clear idea that why the `ReactJS` codes are visible in browser and the basic reason behind them.

Thank you for reading this far. This is a brief introduction of **Hiding ReactJS code in Production Environment**.

If you find this article useful, share this article. Someone could find it useful too. If you find anything technically inaccurate please feel free to create a [issue](https://github.com/CapsCode-Website/blogfiles/issues).

Hope its a nice and informative read for you.
VISIT https://www.capscode.in/blog TO LEARN MORE...
See you in my next Blog article, Take care!!

Thanks,
CapsCode
