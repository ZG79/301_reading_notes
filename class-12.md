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
