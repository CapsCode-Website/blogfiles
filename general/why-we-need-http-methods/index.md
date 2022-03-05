https://www.youtube.com/watch?v=BcxzejYgKAI -- amazing video
https://www.youtube.com/watch?v=1xVK2m817Bw
https://www.youtube.com/watch?v=YlS-I-hCGzA

# Introduction:

Have you worked with API's and used different HTTP Methods like GET, POST, PUT, PATCH, DELETE
if yes, then have you ever thought of why we have

1. why we need HTTP methods
   so that everyone will use the common naming convention for CRUD operation
   Explanation
   World Wide Web is distibuted in the 2 sections, one is client and the other is server.
   let say I have created API and for reading data i will tell CLIENT to use the READ method, and same way some other developer has created the API and tells users to use SEARCH to get the data from the server, then there will be a lot of confusion in the world wide web.
   Every developer will get confused with all these different naming convention for the same operation in the server.
   So, w3c (World Wide Web Consortium)[https://www.w3.org/Consortium/] has created standard HTTP methods

HTTP protocol is used to send information in a format that both the client and the server can understand.

2. use of http status code
   whenever we request an API, the API will also sends the acknowledgement and we call as a API Response. These API Response gives the information whether the API is successful or the API failed or there is some server error etc.
   To idetify these messages, we have different status codes.
   Using these status code we can identify the failure or success and what status code bbackend is sending to the frontend so that in frontend we can use this and show some messages or take some action.
   Please do checkout the all list of the API's(here)[https://www.capscode.in/blog/list-of-http-status-code]

3. HTTP Request Header -- this is used to pass additional information to the server. This information is representated as a key value pairs
   ex. Content-Type header defines the return type of the response data.
   The Access-Control-Allow-Origin response header indicates whether the response can be shared with requesting code from the given origin
   etc.
   please refer to the official MDN doc :https://developer.mozilla.org/en-US/docs/Web/HTTP/Headers

4. GET
   GET method is used to get the data from a requested resource.
   Ex. - https://api.capscode.in/userDetails

   some important points about GET

   1. Requests using the HTTP GET method should only fetch data, cannot enclose data in the body of a GET message, and should not have any other effect on data on the server.

   2. A payload within a GET request has no definetaion. sending a payload body on a GET request might cause rejection of the request. We should avoid sending payload to the server and consuming payload by the server.

Lets see some of the Question that might arises in future !!

Q. Can I send HTTP Headers using the GET method?
Yes, you can send any HTTP headers with your GET request.

Q. Can I send data(request payload) using the HTTP GET method?
No, HTTP GET requests cannot have a message body. But you still can send data to the server using the URL parameters.
Ex. - /test/demo_form.php?name1=value1&name2=value2

In this case, you are limited to the maximum size of the URL, which is about 2000 characters (depends on the browser). The HTTP GET method is defined as idempotent, which means that multiple identical GET requests should have the same effect as a single request.

~what is idempotemt and non-idempotent
idempotent means A^n = A
In the context of REST APIs, when making multiple identical requests has the same effect as making a single request – then that REST API is called idempotent.

Some other notes on GET requests:

GET requests can be cached
GET requests remain in the browser history
GET requests can be bookmarked
GET requests should never be used when dealing with sensitive data
GET requests have length restrictions
GET requests are only used to request data (not modify)

+---------+------+------------+
| Method | Safe | Idempotent |
+---------+------+------------+
| CONNECT | no | no |
| DELETE | no | yes |
| GET | yes | yes |
| HEAD | yes | yes |
| OPTIONS | yes | yes |
| POST | no | no |
| PUT | no | yes |
| TRACE | yes | yes |
+---------+------+------------+
