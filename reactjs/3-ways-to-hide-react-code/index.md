## Here are three ways to hide code.

**1. Using `.env` File.**

```javascript
GENERATE_SOURCEMAP = false;
```

[![enter image description here](https://i.stack.imgur.com/CyrWM.png)](https://i.stack.imgur.com/CyrWM.png)

**2. Using `command` line.**

```javascript
GENERATE_SOURCEMAP=false react-scripts build

```

**3. Using `package.json`**

```javascript
scripts: {
  "build": "GENERATE_SOURCEMAP=false react-scripts build"
}
```
