https://www.youtube.com/watch?v=BcxzejYgKAI -- amazing video
https://www.youtube.com/watch?v=1xVK2m817Bw
https://www.youtube.com/watch?v=YlS-I-hCGzA

# Introduction:

Have you worked with API's and used different HTTP Methods like GET, POST, PUT, PATCH, DELETE
if yes, then have you ever thought of why  do we have these many different methods and what is the requirements for these.

If not then lets have a look on all of these questions.

1. why we need HTTP methods
   We need different https method so that everyone will use the common naming convention for CRUD operation
   Explanation
   World Wide Web is distributed in the 2 sections, one is client and the other is server.
   let say I have created an API and for reading data i will tell CLIENT to use the READ method, and same way some other developer has created the API and tells users to use SEARCH to get the data from the server, then there will be a lot of confusion in the world wide web.
   Every developer will get confused with all these different naming convention for the same operation in the server.
   So, w3c (World Wide Web Consortium)[https://www.w3.org/Consortium/] has created standard HTTP methods

HTTP protocol is used to send information in a format that both the client and the server can understand.

2. What is the use of http status code
   whenever we request an API, the API also sends the acknowledgement and we call it as a API Response.These API Response gives the information whether the API is successful or the API has failed or there is some server error etc.
   To identify these errors, we have different status codes.
   Using these status code we can identify the failure or success and what status code backend is sending to the frontend so that in the frontend we can use this code and show some proper error messages or take some action.
   Please do checkout the all list of the API's(here)[https://www.capscode.in/blog/list-of-http-status-code]

3. Wht is the use of HTTP Request Header?
   HTTP request header is used to pass additional information like content type, cookie values, etc to the server. This information is represented as a key value pair.
   ex. Content-Type header defines the return type of the response data.
   The Access-Control-Allow-Origin response header indicates whether the response can be shared with requesting code from the given origin etc.
   
   If you want to learn more abut the HTTP Header then please refer to the official [MDN Doc] (https://developer.mozilla.org/en-US/docs/Web/HTTP/Headers)


Thats all about why do we need HTTP methods, HTTP status code and Request headers
Now lets see what are the various HTTP methods available and what is the difference between them.

4. GET
   GET method is used to get the data from a requested resource or Use GET to retrieve resource/ information **only**
   Ex. - https://api.capscode.in/userDetails

some important points about GET

1.  Requests using the HTTP GET method should only fetch data, cannot enclose data in the body of a GET message, and should not have any other effect in data on the server.

2.  A payload within a GET request has no definetaion. sending a payload body on a GET request might cause rejection of the request. We should avoid sending payload to the server and consuming payload by the server.

note: For any given HTTP GET API, if the resource is found on the server, then it must return HTTP response code 200 (OK) – along with the response body,
In case the resource is NOT found on the server then API must return HTTP response code 404 (NOT FOUND)

Lets see some of the Question that might arises in future !!

Q. Can I send HTTP Headers using the GET method?
Yes, you can send any HTTP headers with your GET request.

NOTE: if you want to learn about HTTP Header click here (link)

Q. Can I send data(request payload) using the HTTP GET method?
No, HTTP GET requests cannot have a message body. But you still can send data to the server using the URL parameters.
Ex. - /test/demo_form.php?name1=value1&name2=value2
In this case, you are limited to the maximum size of the URL, which is about 2000 characters(browser and browser version dependent). The HTTP GET method is defined as idempotent, which means that multiple identical GET requests should have the same effect as a single request.

Q. Can we use GET to make insertion.
Yes, we can, it depends on the backend code that what we are going to do.
But we should avoid violating the HTTP protocol as sometimes it may leds to rejection of the API call.

Some other notes on GET requests:

GET requests can be cached
GET APIs are idempotent OR GET APIs should be idempotent
GET requests remain in the browser history
GET requests can be bookmarked
GET requests should never be used when dealing with sensitive data
GET requests have length restrictions
GET requests are only used to request data (not modify)
Parameters remain in browser history because they are being passed in the URL

Request has body No
Successful response has body Yes
Safe Yes
Idempotent Yes
Cacheable Yes
Allowed in HTML forms Yes

~what is idempotemt and non-idempotent ?
idempotent means A^n = A (A*A*A....\*n times A) = A
In terms of REST APIs, when making multiple identical requests has the same effect on the server as making a single request – then that REST API is called idempotent.

~ Caching
HTTP caching is applicable only to idempotent requests, which makes a lot of sense; only idempotent and nullipotent requests yield the same result when run multiple times. In the HTTP world, this fact means that GET requests can be cached but POST requests cannot.
"Responses to POST method are not cacheable, UNLESS the response includes appropriate Cache-Control or Expires header fields."
So, YES, you can cache POST request response but only if it arrives with appropriate headers. In most cases you don't want to cache the response. But in some cases - such as if you are not saving any data on the server - it's entirely appropriate.

The POST method itself is semantically meant to post something to a resource. POST cannot be cached because if you do something once vs twice vs three times, then you are altering the server's resource each time. Each request matters and should be delivered to the server.

The PUT method itself is semantically meant to put or create a resource. It is an idempotent operation, but it won't be used for caching because a DELETE could have occurred in the meantime.

The DELETE method itself is semantically meant to delete a resource. It is an idempotent operation, but it won't be used for caching because a PUT could have occurred in the meantime.

More about HTTP caching: https://developer.mozilla.org/en-US/docs/Web/HTTP/Caching

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

5. POST -
   POST is used to send data to a server to create/update a resource.
   When talking strictly about REST, POST methods are used to create a new resource into the collection of resources.

   The data sent to the server with POST is stored in the request body of the HTTP request & The type of the body of the request is indicated by the Content-Type header.
   When talking strictly about REST, POST methods are used to create a new resource into the collection of resources.

Responses to this method are not cacheable unless the response includes appropriate Cache-Control or Expires header fields.

Please note that POST is neither safe nor idempotent, and invoking two identical POST requests will result in two different resources containing the same information (except resource ids).

Some notes on POST requests:

POST requests are never cached (can be done explictly as mentioned above)
POST requests do not remain in the browser history
POST requests cannot be bookmarked
POST requests have no restrictions on data length
Parameters are not saved in browser history

Request has body Yes
Successful response has body Yes
Safe No
Idempotent No
Cacheable Only if freshness information is included
Allowed in HTML forms Yes

note: Ideally, if a resource has been created on the origin server, the response SHOULD be HTTP response code 201 (Created) and contain an entity that describes the status of the request and refers to the new resource, and a Location header.

Is body mandatory in POST request?
Yes it is expected to have Body/Content in body, but it is not required(Mandatory).

Some questions or doubts.
Q. how to send lot of data (filter data) from frontend to server to retrive data.
A. to retrive data we have to use the GET call, but as per the question we have to send the data to server, if the data is less than 4000 char and non sensitive then we can send these data in the URL and use the GET call but of the data is big or data is sensitive data then we have to send the data in the payload of POST call.
So POST call can also be used to get the data.
but isnt it against the http protocol.

lets answer this in the next question,

Q. Can we INSERT/UPDATE/DELETE data in a GET method in MVC?
A. GET http://www.example.com/users/id
DELETE http://www.example.com/users/id

From the above URLs, you can easily tell which one would return a result and which one would remove the record (depending on the application being used).

Now, coming to your question. Although it is you who would implement the actual underlying code. So, it depends on you whether you delete that record or not and whether to return the record or return something else. It is just the way HTTP protocol was designed to create an intuition for the users and developers.

Other than this, if you want to use these verbs to do something else, you surely can. The underlying code would execute as you want it to. I can write the action method, which actually deletes the user from the database

Although the above code was to get the response (not a user or other stuff, just response) but I added the code to delete something (or the user). No error, and the record would also be deleted, provided no other error occurs.

The actual thing is that you should follow the protocol. Because, other developers have no idea what your function would do, unless the verb is specified. It is just to remove the ambiguity of the API of your application. Otherwise, you can surely do anything.

You can also remove that attribute from your application.

NOTE: For idempotent things, you're also allowed to do insert with PUT. So both POST/PUT can be used for insert/update (both submit data). It's up to the dev how they want to use - some like to map CRUD to the methods - others just POST or PUT for everything depending on idempotence.

There's no strict correspondence between HTTP methods and CRUD. This is a convention adopted by some frameworks, but it has nothing to do with REST constraints.

NOTE: It's ok to use POST for updates, it was never said that POST is for "create" operations only.

6. PUT
   PUT is used to send data to a server to create/update a resource.

   Generally – not necessarily – PUT APIs are used to update the resource state (if the resource does not exist, then API may decide to create a new resource or not). If you invoke a PUT API N times, the very first request will update the resource; the other N-1 requests will just overwrite the same resource state again and again – effectively not changing anything.

PUT is similar to POST in that it can create resources, but it does so when there is a defined URI. PUT overwrites the entire entity if it already exists, and creates a new resource if it doesn’t exist.

PUT implies putting a resource - completely replacing whatever is available at the given URL with a different thing. By definition, a PUT is idempotent.

Hence, PUT is idempotent.
Responses to PUT method are not cacheable.

note: If a new resource has been created by the PUT API, the origin server MUST inform the user agent via the HTTP response code 201 (Created) response.
If an existing resource is modified, either the 200 (OK) or 204 (No Content) response codes SHOULD be sent to indicate successful completion of the request.

Request has body Yes
Successful response has body May
Safe No
Idempotent Yes
Cacheable No
Allowed in HTML forms No

Q. Difference between POST and PUT
A.
HTTP POST http://www.appdomain.com/users
HTTP POST http://www.appdomain.com/users/123/accounts

HTTP PUT http://www.appdomain.com/users/123
HTTP PUT http://www.appdomain.com/users/123/accounts/456

The difference between the POST and PUT APIs can be observed in request URIs. POST requests are made on resource collections, whereas PUT requests are made on a single resource.

Generally, when a PUT request creates a resource the server will respond with a 201 (Created), and if the request modifies existing resource the server will return a 200 (OK) or 204 (No Content).

7. PATCH
   is used to make partial update / modification to a resource within a collection of resources.

If you see PUT requests modify a resource entity too. So to make it more precise – the PATCH method is the correct choice for partially updating an existing resource, and you should only use PUT if you’re replacing a resource in its entirety.

NOTE: The PATCH method is not a replacement for the POST or PUT methods. It applies a delta (diff) rather than replacing the entire resource.

PUT is a update / replace operation but PATCH is partial update / Modify operation

PATCH request is non-idempotent

Request has body Yes
Successful response has body Yes
Safe No
Idempotent No
Cacheable No
Allowed in HTML forms No

8. DELETE
   The DELETE method deletes the specified resource at the specified URL.

note: A successful response of DELETE requests SHOULD be an HTTP response code 200 (OK) if the response includes an entity describing the status.
The status should be 202 (Accepted) if the action has been queued.
The status should be 204 (No Content) if the action has been performed but the response does not include an entity.
Repeatedly calling DELETE API on that resource will not change the outcome – however, calling DELETE on a resource a second time will return a 404 (NOT FOUND) since it was already removed.

Request has body May
Successful response has body May
Safe No
Idempotent Yes
Cacheable No
Allowed in HTML forms No

9. HEAD
   HEAD is almost identical to GET, but without the response body.

In other words, if GET /users returns a list of users, then HEAD /users will make the same request but will not return the list of users.

This is useful for retrieving meta-information written in response headers, without having to transport the entire content.
HEAD requests are useful for checking what a GET request will return before actually making a GET request - like before downloading a large file or response body. and before actuall downloading it backend can send the msg that file sie if big.

This method is often used for testing hypertext links for validity, accessibility, and recent modification.

GET fetches head + body, HEAD fetches head only
Request has body No
Successful response has body No
Safe Yes
Idempotent Yes
Cacheable Yes
Allowed in HTML forms No

10. OPTIONS
    OPTIONS method requests permitted communication options for a given URL or server. A client can specify a URL with this method, or an asterisk (\*) to refer to the entire server.

In CORS, a preflight request is sent with the OPTIONS method so that the server can respond if it is acceptable to send the request.

Request has body No
Successful response has body Yes
Safe Yes
Idempotent Yes
Cacheable No
Allowed in HTML forms No

11. TRACE
    The TRACE method method is used to perform a message loop-back test that tests the path for the target resource (useful for debugging purposes).

Request has body No
Successful response has body No
Safe Yes
Idempotent Yes
Cacheable No
Allowed in HTML forms No

12. CONNECT
    The CONNECT method is used to start a two-way communications (a tunnel) with the requested resource.It can be used to open a tunnel.

Request has body No
Successful response has body Yes
Safe No
Idempotent No
Cacheable No
Allowed in HTML forms No
