Hello Dev,

In this article, I will explain you 1 very important limitation of setTimeout in JavaScript.

Browsers including Internet Explorer, Chrome, Safari, and Firefox store the delay as a 32-bit signed integer internally. This causes an integer overflow when using delays larger than **2,147,483,647 ms (about 24.8 days)**, resulting in the timeout being executed immediately.


```js
function func(){
    setTimeout(()=>{
        console.log('Print hello after 2,147,483,648 milliseconds')
    }, 2147483648)
}

func() 

```

Expected output/ behavior for the above code should be the callback function of `setTimeout` should execute after **2,147,483,648 milliseconds**.

But the callback function will get executed immediately because the maximum delay value in `setTimeout` is **2,147,483,647 milliseconds** and we have provided **2,147,483,648 milliseconds** as delay.


Thank you for reading this so far. This is a brief introduction on **How Large Delay Value In `setTimeout` Acts in JavaScript**.

Hope it's a nice and informative read for you.
If you find this article useful, like and share this article. Someone could find it useful too.

If you find anything technically inaccurate, please feel free to reach out to us.

VISIT https://www.capscode.in/blog TO LEARN MORE.

See you in my next Blog article, Take care!!

Thanks,\
CapsCode