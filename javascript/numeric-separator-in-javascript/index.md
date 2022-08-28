Hello Devs,

In this article let's discuss about one of the most amazing features introduced in `ECMAScript21` (12th edition) i.e., Numeric Separator. 


## Table of content

1. [Introduction](#introduction)
2. [Some Examples](#examples)
3. [Conclusion](#conclusion)


## 1. Introduction <a name="introduction"></a>
This feature enables developers to make the **numeric literals** more readable.
What I mean to say is, large **numeric literals** (both integers and floating-point) which are difficult for the human eye to parse quickly, especially when there are long digit repetitions, this feature of ES12 makes it simple to read.

How?

`Please read this number`
```js
let num = 1000000000000
```
if someone is reading the value of num verbally, then in the first sight one cannot be able to read it. So **numeric separator** help developers make it readable in the first sight.

Let's see how it helps.

`Now, read this number`
```js
let num = 100_000_000_000 
```

### **Did you found it little easier to read than the first one? If YES let me know**

---


## 2. Examples <a name="examples"></a>
Let see some examples,
1. equality & strict equality

```js
let num1 = 1000000000000 
let num2 = 100_000_000_000

console.log(num1==num2) //true
console.log(num1===num2) //true
```


2. What is the output in console for number with underscore in it?

```js
let num = 100_000_000_000
console.log(num) //100000000
```

3. We can use underscore with Binary, Octal, Hex numbers are well

```js
let num1 = 0b1010_0101_1001 // binary
let num2 = 0o2_3_5_7 // octal
let num3 = 0xA_B_C_D_E // hex
```

4. underscore with String Literals.

```js
let str1="hellocapscode"
let str2="hello_capscode"

console.log(str1==str2)//false as numeric separator works well only with numbers

console.log(str1) //hellocapscode
console.log(str2) //hello_capscode
```

---

## 3. Conclusion <a name="conclusion"></a>

Awesome! Now you have learnt 1 new feature of JavaScript, I hope you have now a very clear idea regarding underscore between digits in numeric literals.

Thank you for reading this far. This is a brief introduction of **Numeric Separator In JavaScript**.

If you find this article useful, share this article. Someone could find it useful too. If you find anything technically inaccurate, please feel free to create a [issue](https://github.com/CapsCode-Website/blogfiles/issues).

Hope it's a nice and informative read for you.
VISIT https://www.capscode.in/blog TO LEARN MORE...
See you in my next Blog article, Take care!!

Thanks, \
CapsCode