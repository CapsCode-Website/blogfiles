Hello Developers,

Have you worked with APIs and used different HTTP Methods like GET, POST, PUT, PATCH and DELETE etc,
if yes, then have you ever thought of why we have these many different methods, why everyone is using the same nomenclature and what is the requirements for these.

If not then let's have a look at all of these questions right below and **I CAN GUARANTEE THAT AFTER READING THIS ARTICLE YOU WILL NEVER HAVE ANY DOUBTS RELATED TO HTTP METHODS**.

## Table of content
---
1. [Why do we need HTTP methods](#why-we-need-http-methods)
2. [What is the use of the HTTP status code](#what-is-the-use-of-http-status-code)
3. [What is the use of the HTTP request header](#what-is-the-use-of-http-request-header)
4. [GET](#get-method)
5. [POST](#post-method)
6. [PUT](#put-method)
7. [PATCH](#patch-method)
8. [DELETE](#delete-method)
9. [HEAD](#head-method)
10. [OPTIONS](#options-method)
11. [TRACE](#trace-method)
12. [CONNECT](#connect-method)

Before directly jumping onto the HTTP methods, let's first see some of the important points/ topics which might help you during your further read.
If you are already aware of these, then you can directly jump onto the HTTP method topic. [HTTP METHODS](#get-method)

## 1. Why do we need HTTP methods? <a name="why-we-need-http-methods"></a>

We need different HTTPS methods(like GET, POST, PUT, DELETE etc) so that all the developers will use the common naming convention for CRUD operations.
   
**Explanation**
World Wide Web(WWW) is distributed in 2 sections, one is client and the other is server.
Let's say I have created an API and for reading data I will tell CLIENT to use the READ method, and same the way some other developer has created the API used SEARCH to get the data from the server, then there will be a lot of confusion in the World Wide Web, although READ & SEARCH both are doing the same operation (fetching the data from the server).

Every developer will get confused with all these different naming conventions for the same operation in the server.
So, w3c [World Wide Web Consortium](https://www.w3.org/Consortium/) has created standard HTTP methods, so that everyone can use the common naming convention for CRUD operations.

The HTTP protocol is used to send information in a format that both the client and the server can understand.

-----

## 2. What is the use of the HTTP status code? <a name="what-is-the-use-of-http-status-code"></a>

Whenever we request an API, the API also sends the acknowledgment back to the client and we call it an API Response. This API Response gives information regarding the API status whether it is successful or the API has failed or there is some server error etc.

**To identify these errors, we have different status codes.**
Please check out all lists of the APIs [here](https://www.capscode.in/blog/list-of-http-status-code)

Using these status codes we can identify the failure or success and what status code backend server is sending to the frontend so that in the frontend we can use this code to show some proper error messages on different failures and show data in the UI on success.

----

## 3. What is the use of the HTTP request header? <a name="what-is-the-use-of-http-request-header"></a>
 
The HTTP request header is used to pass additional information like content type, cookies value, Auth, etc to the server. This information is represented as a key-value pair in the request header while calling APIs.

**Ex.** 

`Content-Type` header defines the return type of the response data.
The `Access-Control-Allow-Origin` response header indicates whether the response can be shared with requesting code from the given origin etc.
   
If you want to learn more about the HTTP Header then please refer to the official [MDN Doc](https://developer.mozilla.org/en-US/docs/Web/HTTP/Headers)



\
That's all about why we need HTTP methods, HTTP status codes and request headers.
Now let's see what are the various HTTP methods available and what is the difference between them.

---

## 4. GET <a name="get-method"></a>
GET method is used to get the data from a requested resource/ server or in another way, use GET to retrieve resource/ information **only**

**Ex.**

let's say we have an API URL like this, https://api.capscode.in/user
and when we do the GET call to this URL, it will return the list of users from the database.


HTTP Requests using the HTTP GET method should only fetch data, cannot enclose data in the body/payload of a GET message, and should not have any other effect on data on the server.

A payload within a GET request has no definition. Sending a request body/ payload in a GET request might cause rejection of the request. We should avoid sending payload to the server and consuming payload by the server (It's a violation of HTTP Protocol).

**NOTE:** For any given HTTP GET API, if the resource is found on the server, then it must return HTTP response code 200 (OK) – along with the response body,
In case the resource is NOT found on the server then API must return HTTP response code 404 (NOT FOUND)


\
**Let's see some of the Questions that might arise during further reading !!**

<details>
<summary>Q. Can I send HTTP headers using the GET method?</summary>

Yes, you can send any `HTTP headers` with your GET request.
</details>

<details>
<summary>Q. Can I send data(request payload) using the HTTP GET method?</summary>
No, HTTP GET requests cannot have a request body/ payload. But you can still send data to the server using

URL parameters

https://www.api.capscode.in/user/12

or 

using query string
https://www.api.capscode.in/user?userId=12


In this case, you are limited to the `maximum` size of the URL, which is about `2000 characters`(depending on browser and browser version). 

The HTTP GET method is defined as `idempotent`, which means that multiple identical GET requests should have the same effect as a single request on the server. 
(We will discuss *what is Idempotent* below)
</details>


<details>
<summary>Q. Can we use GET to make insertions, updations or deletions in the database </summary>

Yes, we can, it depends on the backend code and as a developer what we are going to do with the GET request coming from the UI.

**But we should avoid violating the HTTP protocol as sometimes it may lead to the rejection of the API call.**
</details>

\
**Important points to note**

1. GET requests can be cached (Chacheable)
2. GET APIs are idempotent OR GET APIs should be idempotent
3. GET requests to remain in the browser history
4. GET requests can be bookmarked
5. GET requests should never be used when dealing with sensitive data
6. GET requests to have length restrictions
7. GET requests are only used to request data (not modify) or GET requests should only be used to request data (not modify).
8. Parameters remain in browser history because they are being passed in the URL
9. GET Request has NO body or we should avoid sending body in GET calls.
10. Successful response of GET call has body.
11. GET is less secure because the data sent is part of the URL and is visible to everyone as a part of the URL.
12. Only ASCII characters are allowed in GET calls no binary chars and that's why we cannot send binary files (/upload file)
13. GET calls are safe (An HTTP method is safe if it doesn't alter the state of the server)



<details>
<summary>Q what are idempotent and non-idempotent ?</summary>
Idempotent means A^n = A 
or (A*A*A....\*n times A) = A
In terms of REST APIs, when making multiple identical requests to the server has the same effect on the server as making a single request – then that REST API is called idempotent.
</details>

<details>
<summary>Q. What is Chacheable ?</summary>

A cacheable response is an HTTP response that can be cached.

HTTP caching applies only to idempotent requests, which makes a lot of sense.

Only idempotent and nullipotent requests yield the same result when run multiple times. In the HTTP world, this fact means that GET requests can be cached but POST requests cannot. But this is not completely correct,

Responses to the POST method are not cacheable, UNLESS the response includes appropriate Cache-Control or Expires header fields.
So, YES, you can cache POST request response but only if it reached the client with appropriate headers. In most cases, you don't want to cache the response. But in some cases - such as if you are not saving any data on the server - it's entirely appropriate.

The POST method itself is semantically meant to post something to a resource group. POST cannot be cached because if you do something once vs twice vs three times, then you are altering the server's resource each time. Each request matters and should be delivered to the server.
</details>

| Method | Safe | Idempotent |
| -------- | ------ | ----------- |
| GET | yes | yes |
| POST | no | no |
| PUT | no | yes |
| DELETE | no | yes |
| OPTIONS | yes | yes |
| CONNECT | no | no |
| HEAD | yes | yes |
| TRACE | yes | yes |



<details>
<summary> Q. What is SAFE & UNSAFE HTTP methods</summary>

An HTTP method is safe if it doesn't alter the state of the server. In other words, a method is safe if it leads to a read-only operation. Several common HTTP methods are safe: GET, HEAD, or OPTIONS. All safe methods are also idempotent, but not all idempotent methods are safe. For example, PUT and DELETE are both idempotent but unsafe.

[Source](#https://developer.mozilla.org/en-US/docs/Glossary/Safe/HTTP)

</details>

----

## 5. POST <a name="post-method"></a>
POST is used to send data to the server to create/update a resource.
or\
You can say that whenever you want to create/update resources in the server, you should use the POST request.

When talking strictly about REST, POST methods are used to create a new resource in the collection of resources. When a new resource is POSTED to the collection of resources by calling an API of the parent source (where all resources are defined), this new resource will be created by getting a new ID (a new resource URI).

**Ex-**

```js
// API URL: https://api.capscode.in/user
request payload:
    {
        username:'tom',
        phone: "0123456789",
        country:'India'
    }
// response : some auto generated id as 5
```
The data that needs to be sent to the server with a POST request is stored in the request body as the payload of the HTTP request & the type of the body of the request is indicated by the Content-Type header.


Responses to this method are not `cacheable` unless the response includes appropriate `Cache-Control or Expires` header fields.

Please note that POST is **neither** safe **nor idempotent**, and invoking two identical POST requests will result in two different resources containing the same information (except resource ids).

\
**Important points to note**

1. POST requests are never cached (can be done explicitly as mentioned above).
2. POST requests do not remain in the browser history.
3. POST requests cannot be bookmarked.
4. POST requests have no restrictions on data length.
5. Parameters are not saved in browser history.
6. POST Request has a request body(/payload).
7. Successful response of POST request has body.
8. POST requests are not safe.
9. POST requests are not idempotent.
10. POST requests are cacheable (Only if freshness information is included)
11. POST requests are allowed in HTML forms so that we can securely send form data.

\
**NOTE:** Ideally, if a resource has been created on the origin server, the response code **SHOULD** be 201 (Created) and contain an entity that describes the status of the request and refers to the new resource, and a Location header.



**Some questions which may come**
<details>
<summary>Q. Is body mandatory in POST request ?</summary>

Yes, it is expected to have body/content in the body, but it is not required(Mandatory).
</details>

<details>
<summary>Q. How to send a lot of data (filter data) from the frontend to the server to retrieve data based on the filter.</summary>

To retrieve data we have to use the GET call, but as per the question we have to send the data to the server, if the data is less than 4000 chars and non-sensitive then we can send these data in the URL and use the GET call but if the data is large or data is sensitive data then we have to send the data in the payload of POST call because if we send the data in the URL then it will be visible from the URL and may lead to exposure of sensitive data.
So POST calls can also be used to get the data.
but isn't it against the HTTP protocol?

Let's answer this in the next question,
</details>


<details>
<summary>Q. Can we INSERT/UPDATE/DELETE data in a GET method ?</summary>

GET https://www.api.capscode.in/users/id \
DELETE https://www.api.capscode.in/users/id

From the above URLs, you can easily tell which one would return a result and which one would remove the record (depending on the application being used).

Now, coming to the question. Although it is you who would write the code & implement the logic. So, it depends on you whether you delete that record or not and whether to return the record or return something else. 
So these methods are just the way HTTP protocol was designed to create an intuition for the users and developers to understand what's happening behind the scene.

Other than this, if you want to use these verbs to do something else, you surely can. The underlying code would execute as you want it to. I can write the action method, which deletes the user from the database

Although the above code was to get the response (not a user or other stuff, just a response), but I added the code to delete something (or to delete the user). No error will occur, and the record would also be deleted, provided no other error occurs.

**The actual thing is that you should follow the protocol.** Because other developers have no idea what your function would do unless the verb is specified. Otherwise, you can surely do anything.

You can also remove that attribute from your application.
</details>

---

## 6. PUT <a name="put-method"></a>
PUT is used to send data to the server to create/update a resource.

Generally (*not necessarily*), PUT APIs are used to update the resource state (if the resource does not exist, then API may decide to create a new resource or not). If you invoke a PUT API N times, the very first request will update the resource and **the other N-1 requests will just overwrite the same resource state again and again – effectively not changing anything**.

PUT is similar to POST in that it can create resources, but it does so when there is a defined URI. PUT overwrites the entire entity if it already exists, and creates a new resource if it doesn’t exist.

PUT implies putting a resource - completely replacing whatever is available at the specified URL with a different (updated) resource. By definition, a PUT request is idempotent.

If you want to update a specific resource (which comes with a specific URI), you can call the PUT method to that resource URI with the request body containing the completely new version of the resource you are trying to update.

**NOTE:** If a new resource has been created by the PUT API, the origin server MUST inform the user agent via the HTTP response code 201 (Created) response.
If an existing resource is modified, either the 200 (OK) or 204 (No Content) response codes SHOULD be sent to indicate the status/action of the request.

**Ex:**

```js
API URL : https://www.api.capscode.in/user/5
Request payload: {
    username:'tom',
    phone: "9876543210",
    country:'India'
}
```


**Some points about PUT Request**
1. PUT Request has body.
2. The successful response may or may not have a body.
3. PUT Requests are not safe.
4. PUT Requests are Idempotent.
5. PUT Requests are not Cacheable.
6. PUT Requests are not Allowed in HTML forms.



**NOTE:** For idempotent things, you're also allowed to do an insert operation with PUT. So both POST/PUT can be used for insert/update (both submit data). It's up to the developer how they want to use it. Some like to map CRUD to the methods - others just POST or PUT for everything depending on idempotence.

There's no strict correspondence between HTTP methods and CRUD. This is a convention adopted by some frameworks, but it has nothing to do with REST constraints.

NOTE: It's ok to use POST for updates when you want to replace or change the entire resource, it was never said that POST is for "create" operations only. But if it's a partial update then we have to use the PATCH method.

<details>
<summary>
Q. Difference between POST and PUT
</summary>

HTTP POST https://www.api.capscode.in/users \
HTTP POST https://www.api.capscode.in/users/123/accounts \
\
HTTP PUT https://www.api.capscode.in/users/123 \
HTTP PUT https://www.api.capscode.in/users/123/accounts/456

The difference between the POST and PUT APIs can be observed in request URIs. POST requests are made on resource collections, whereas PUT requests are made on a single resource.

or

Calling POST requests repeatedly /multiple time creates the same resource multiple times in the database/server. 
But PUT will replace the resource at the specified id in the API URL.
</details>


---


## 7. PATCH <a name="patch-method"></a>
PATCH Request is used to make **partial updates/modifications** to a resource within a collection of resources.

If you see PUT requests modify a resource entity too by updating the resource at a specified URI with a new resource. So to make it more precise – the PATCH method is the correct choice for **partially updating** an existing resource, and you should only use **PUT if you’re replacing a resource with a newly updated value entirety**.

**NOTE:** The PATCH method is not a replacement for the POST or PUT methods. It applies a delta (diff) rather than replacing the entire resource.

**Ex:**

```js
API URL : https://www.api.capscode.in/users/5
Request payload: {
    phone: "+91-9876543210",
}
```

PUT is an update/ replace operation but PATCH is a partial update/ modify operation

**some additional information about PATCH**
1. PATCH request is non-idempotent.
2. PATCH request has body.
3. The successful response has body.
4. PATCH requests are not safe.
5. PATCH requests are not Idempotent.
6. PATCH requests are not Cacheable.
7. PATCH requests are not allowed in HTML forms.

<details>
<summary>Q. How PATCH is different from POST & PUT ?</summary>

let's say we have an API endpoint as `/users/{{userid}}`, and a user has a phone. With a PATCH request, you may only need to send the updated phone number in the request body - as opposed to POST and PUT which require the full user entity.
But in the PUT & POST, we are supposed to send the complete information along with the updated phone number in the payload.
We can send only the updated phone number in the payload along with the id and based on this the backend code can take action to just update the phone for the current id, but again it's a violation of the HTTP Protocol.
</details>

---

## 8. DELETE <a name="delete-method"></a>
The DELETE method deletes the resource at the specified URL.

**NOTE:** A successful response to DELETE requests SHOULD have the response code 200 (OK).
The status code should be 202 (Accepted) if the action has been queued.
The status should be 204 (No Content) if the action has been performed but the response does not include an entity.
Repeatedly calling DELETE API on that resource will not change the outcome – however, calling DELETE on a resource a second time will return a 404 (NOT FOUND) since it was already removed.

**Ex:**

```js
API URL: https://www.api.capscode.in/users/5

//this will DELETE the user having user id 5.
```

**Some important points about DELETE**
1. DELETE Request may or may not have body.
2. The successful response may or may not have body.
3. DELETE requests are not safe.
4. DELETE requests are Idempotent.
5. DELETE requests are not Cacheable.
6. DELETE requests are not Allowed in HTML forms.

---

## 9. HEAD <a name="head-method"></a>
HEAD is almost identical to GET but without the response body.

In other words, if GET /users return a list of users, then HEAD /users will make the same request but will not return the list of users.

This is useful for retrieving meta-information written in **response headers**, without having to transport the entire content.

HEAD requests are useful for checking what a GET request is going to return before actually making a GET request.

**Ex:**

like before downloading a large file or response body and before actually downloading it backend can send the message that the file size is big and based on that you can take action.

This method is often used for testing hypertext links for validity, accessibility, downloading a large file and recent modification.

**some important notes about HEAD**
1. GET response has a header & body but the HEAD response has only headers.
2. HEAD Request has no body.
3. The successful response has no body.
4. HEAD requests are safe.
5. HEAD requests are idempotent.
6. HEAD requests are cacheable.
7. HEAD requests are not allowed in HTML forms.


---


## 10. OPTIONS <a name="options-method"></a>
OPTIONS requests permitted communication options for a given URL or server. A client can specify a URL with the OPTIONS method, or an asterisk (\*) to refer to the entire server.

In CORS, a preflight request is sent with the OPTIONS method so that the server can respond if it is acceptable to send the request.


**Some points to note for the OPTIONS request**
1. OPTIONS request has no body.
2. The successful response has body.
3. OPTIONS requests are safe.
4. OPTIONS requests are idempotent.
5. OPTIONS requests are not cacheable.
6. OPTIONS requests are not allowed in HTML forms.

---

## 11. TRACE <a name="trace-method"></a>
The TRACE method is used to perform a message loop-back test that tests the path for the target resource (useful for debugging purposes).

Doesn't work in most of the browsers.

**Some point to note for the TRACE request**
1. TRACE request has no body.
2. The successful response has no body.
3. TRACE requests are safe.
4. TRACE requests are idempotent.
5. TRACE requests are not cacheable.
6. TRACE requests are not Allowed in HTML forms.


---


## 12. CONNECT <a name="connect-method"></a>
The CONNECT method is used to start two-way communications (a tunnel) with the requested resource/ server. It can be used to open a tunnel between the client and the server.

**Some points to note about CONNECT request**
1. CONNECT request has no body.
2. The successful response has body.
3. CONNECT requests are not safe.
4. CONNECT requests are not idempotent.
5. CONNECT requests are not cacheable.
6. CONNECT requests are not Allowed in HTML forms.


---------

Additional Info:

Learn more about HTTP caching: https://developer.mozilla.org/en-US/docs/Web/HTTP/Caching




Thank you for reading this so far. This is a brief introduction to **HTTP Methods**, the difference between them and when to use which request method.

Hope it's a nice and informative read for you. If you find this article useful, like and share this article. Someone could find it useful too.

If you find anything technically inaccurate, please feel free to reach out to us.

VISIT https://www.capscode.in/blog TO LEARN MORE.

See you in my next Blog article, Take care!!

Thanks,\
CapsCode