# API
## About Rest: designed around 2000s by Roy Fielding. 
It standsfor : "Representational State Transfer." It is an architectural style for designing web services that communicate over the HTTP protocol. 
### What is an identifier of a resource? Give an example.
REST APIs are designed around resources, which are any kind of object, data, or service that can be accessed by the client.It can be number or strings or anything that follows the URL rule. 

Example: www.apple.com/iphone/14pro - In this URL iphone is the path to the iphone resource and 14pro is identifier.  This URI uniquely identifies the book resource and can be used by clients to access, manipulate, or retrieve information about the book.
### What are the most common HTTP verbs?
The most common operations are GET, POST, PUT, PATCH, and DELETE.
### What should the URIs be based on?
Should be based on the resources they identify.
### example of a good URI.
Not complex. well worded and complete.
https://api.conmputer.com/users/12345
### Chatty web API

Chatty web API is not a good thing. Since all web requests impose a load on the web server, the more requests, the bigger the load. Therefore, try to avoid "chatty" web APIs that expose a large number of small resources. Such an API may require a client application to send multiple requests to find all of the data that it requires. Symptoms of chatty I/O include high latency and low throughput. End users are likely to report extended response times or failures caused by services timing out, due to increased contention for I/O resources.

### What status code does a successful GET , POST, DELETE request return?
GET: returns a status code of 200 OK

POST: If a POST method creates a new resource, it returns HTTP status code 201 (Created). If the method does some processing but does not create a new resource, the method can return HTTP status code 200 and include the result of the operation in the response body. Alternatively, if there is no result to return, the method can return HTTP status code 204 (No Content) with no response body.

DELETE: returns a status code of 204 (No Content)

### What status code does an unsuccessful GET request return?
- 404 Not Found:
- 403 Forbidden: 
- 401 Unauthorized
- 400 Bad Request
- 500 Internal Server Error
