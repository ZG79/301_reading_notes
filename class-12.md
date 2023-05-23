## Status Codes
A status code is a number higher than 100 and smaller than 600 that is part of a HTTP response. The first digit defines the class of the status. A status code comes with a reason phrase. The code is for programmatic recognition the phrase is for humans to understand what happened.

- 100’s = Server's way of telling the header part has been received, and will try to comply with the request. The request might fail.
- 200’s = All good. 
- 300’s = The location the user is trying to access isn't available, redirecting the request.
- 400’s = Invalid request, error is caused bu client side (incorrect input)
- 500’s = error might caused by the server. User should try the same request again. 
- 202 = A status code 202 means that the request has been accepted for processing, but the processing has not been completed. This status code is useful when the actual operation is asynchronous in nature.
- 308 = aka "Permanent Redirect," is a code that indicates that the target resource has been permanently moved to a different URL. 
- If the client hasn't received the data I'd use 204 No content status code. ( server successfully processed the request and fulfilled it, but there is no content to send back in the response payload.)
- If the resource got deleted or moved I'd use 410 Gone. (The 410 Gone status code indicates that the requested resource is no longer available, and there are no forwarding addresses where it might be found.)
- Forbidden status code: 403 Forbidden status code indicates that the server understood the request but refuses to authorize it. 

## Build a rest API With Node.js, Express & MongoDB
1. Why do we need to pull our MongoDB database string out of our server and put it into our .env?

Because we don't want sensitive information stored in the database to get out in the GitHub or accessible to the public.

2. What is middleware?

When the server gets request and before it sends the data. `app.use()` and parse the request with JSON.  

3. What does app.use(express.json()) do? 

It will enable the middleware provided by the `express.json()`

4. What does the /:id mean in a route?


5. What is the difference between PUT and PATCH?


6. How do you make a default value in a schema?


7. What does a 500 error status code mean?


8. What is the difference between a status 200 and a status 201?

