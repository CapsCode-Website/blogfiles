Hello Devs,

In this blog I am going to discuss about the https status code in an API calls.
I know, you all must have worked on many API's till date and also checked the Network tab in browser's Developers tool to check whether the HTTP request is success or its failed. But have you ever seen something called status code in the network tab, which contain some random numbers like `200`, `404`, `501` etc.

In this blog I am going to discuss about these numbers, what these numbers are and what these numbers denotes.
So without wasting time, lets get deep dive into the tutorial.

### What is status code ?

`HTTP` response status codes indicates that whether the request made by you or your browser has been successfully completed or not.
Depending on the response status you will get the different status code.
Status codes are categorized in the following 5 groups.

1. Informational responses (status code between 100–199)
2. Successful responses (status code between 200–299)
3. Redirects (status code between 300–399)
4. Client errors (status code between 400–499)
5. Server errors (status code between 500–599)

### Lets see some of the general status code in each category.

### 1. Informational responses (status code between 100–199)

`100` Continue, if status code is 100, it indicates that the response is OK and you can continue to make other request.

`101` Switching Protocols

`102` Processing

### 2. Successful responses (status code between 200–299)

`200` OK

`201` Created

`202` Accepted

`203` Non-authoritative Information

`204` No Content

`205` Reset Content

`206` Partial Content

`207` Multi-Status

`208` Already Reported

`226` IM Used

### 3.Redirects (status code between 300–399)

`300` Multiple Choices

`301` Moved Permanently

`302` Found

`303` See Other

`304` Not Modified

`305` Use Proxy

`307` Temporary Redirect

`308` Permanent Redirect

### 4. Client errors (status code between 400–499)

`400` Bad Request

`401` Unauthorized

`402` Payment Required

`403` Forbidden

`404` Not Found

`405` Method Not Allowed

`406` Not Acceptable

`407` Proxy Authentication Required

`408` Request Timeout

`409` Conflict

`410` Gone

`411` Length Required

`412` Precondition Failed

`413` Payload Too Large

`414` Request-URI Too Long

`415` Unsupported Media Type

`416` Requested Range Not Satisfiable

`417` Expectation Failed

`418` I'm a teapot

`421` Misdirected Request

`422` Unprocessable Entity

`423` Locked

`424` Failed Dependency

`426` Upgrade Required

`428` Precondition Required

`429` Too Many Requests

`431` Request Header Fields Too Large

`444` Connection Closed Without Response

`451` Unavailable For Legal Reasons

`499` Client Closed Request

### 5. Server errors (status code between 500–599)

`500` Internal Server Error

`501` Not Implemented

`502` Bad Gateway

`503` Service Unavailable

`504` Gateway Timeout

`505` HTTP Version Not Supported

`506` Variant Also Negotiates

`507` Insufficient Storage

`508` Loop Detected

`510` Not Extended

`511` Network Authentication Required

`599` Network Connect Timeout Error

Thank you for reading this far. These HTTP status code are the most commonly used status codes while working with the API calls. If you want to learn more about the other staus codes, please visit [MDN Doc](https://developer.mozilla.org/en-US/docs/Web/HTTP/Status)
If you find this article useful, like and share this article. Someone could find it useful too. If you find anything technically inaccurate please feel free to reach out to us.

Hope its a nice and informative read for you.
VISIT https://www.capscode.in/blog TO LEARN MORE...

### IF MY ARTICLE HELPED YOU

<a href="https://www.buymeacoffee.com/capscode" target="_blank"><img src="https://cdn.buymeacoffee.com/buttons/default-orange.png" alt="Buy Me A Coffee" height="41" width="174"></a>

See you in my next Blog article, Take care!!

[source/ credit: https://developer.mozilla.org/en-US/docs/Web/HTTP/Status](https://developer.mozilla.org/en-US/docs/Web/HTTP/Status)

Thanks,\
CapsCode
