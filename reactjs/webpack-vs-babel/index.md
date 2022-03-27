Creating a React application requires you to set up build tools such as Babel and Webpack. These build tools are required because React's JSX syntax is a language that the browser doesn't understand.
To run your React application, you need to turn your JSX into plain JavaScript, which browsers understand.

https://www.freecodecamp.org/news/create-react-app-npm-scripts-explained/

Babel is a JS transpiler that converts new JS code into old ones. It is a very flexible tool in terms of transpiling. One can easily add presets such as es2015, es2016, es2017, or env; so that Babel compiles them to ES5.

A sourcemap is a mapping between the generated/transpiled/minified JavaScript file and one or more original source files. The main purpose of sourcemaps is to aid debugging. Basically, if there’s an error in the generated code file, the map can tell you the original source file location. That’s it. It’s pretty powerful in practice!
