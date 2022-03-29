Hello Devs,

In this blog post I am going to tell you something about hiding reactjs code in production server.

## Table of content

1. Introduction
2. What makes your source code visible in the browser
3. Hide your reactjs code using .env file
4. Hide your reactjs code using package.json file (in Linux, Windows & other OS)
5. using `cross-env` library
6. Build you custom js file to delete map files

## Introduction

I am sure you have developed a ReactJS application using create-react-app or your own webpack configuration and also deployed it in some hosting platform like Netlify, Vercel, Heroku, Azure, AWS etc.
But have you ever opened your website and in developers tool of your browser, have you ever checked the source tab of it.
If not! Please go and check and see whether your ReactJS codes are visible to public or not like below,
![codeinbrowser](https://raw.githubusercontent.com/CapsCode-Website/blogfiles/master/reactjs/how-to-hide-reactjs-code/1.JPG?raw=true)

If you have your code visible like this, then you are in correct place of this Planet to hide your react codes.
By the end of this blog post I will show you what are the different ways to hide the reactjs codes in production environment and their advantages/ disadvantages.

If you know how to hide the react codes, then also you can have a glance on the other ways of doing so and let me know in the comment whether you are knowing that or not.

## What makes your source code visible in the browser

its map files, but what are they ?

if you don't want to learn about map files and its usage then you can go to the next topic[topic link]
when you are buiding reactjs code babel JSX into the native javascript code (minified JavaScript file) which is little harder to debug withing your components when any error comes, so webpack and babel creates a map file (map files are JSON blob which are non readable by humans).

A sourcemap is a mapping between the generated/transpiled/minified JavaScript file and one or more original source files. The main purpose of sourcemaps is to aid debugging. Basically, if there’s an error in the generated code file, the map can tell you the original source file location. That’s it. It’s pretty powerful in practice!
source[https://trackjs.com/blog/debugging-with-sourcemaps/]

[https://medium.com/@Linda_Ikechukwu/easy-debugging-in-react-with-webpack-source-maps-5dd80a753cab]

Now run `npm run build` command lets create a build folder of your reactjs app.
and then please check you map files inside build\static\js

![image of map files](https://raw.githubusercontent.com/CapsCode-Website/blogfiles/master/reactjs/how-to-hide-reactjs-code/2.JPG?raw=true)

NOTE : if you deploy this build file then your code will be visible in the browser.
so you can delete the map files and then deploy the build folder, but thats not the correct way of doing so and thats not the way a developer will do.

In your localhost (dev environment) webpack auto generates the source map files so that you can see the line numbers of the error in your code

So, without wasting time, lets begin

Here are different ways for hiding your reactjs code from browsers,

**1. Hide your ReactJS code using `.env` file.**
create `.env` file in the root of your reactjs application (the place where src folder is there not inside the src folder or else in the same path where package.json is defined)

Now, add below line of code in it

```javascript
GENERATE_SOURCEMAP = false;
```

and then make a build of your reactjs app using command `npm run build`

What it will do is, it will create a build folder without the map files[link of above topic of map file]. You can go inside the build\static\js
![image of the build folder without map files](https://raw.githubusercontent.com/CapsCode-Website/blogfiles/master/reactjs/how-to-hide-reactjs-code/3.JPG?raw=true)
This way to generating build folder is not Operating System dependent.

Deploy the app now and you cannot see the code in source tab in deelopers tool of your browser

**2. Using `package.json` file.**
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

NOTE: "Remove the .map files" sadly isn't enough. The build also enerates a asset-manifest.json file that contains references to that map files.

**3. using `cross-env` library**
install `cross-env` library in devDependency

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

**4. Build you custom js file to delete map files**

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

**5. Using `command` line.**

```javascript
GENERATE_SOURCEMAP=false react-scripts build
```
