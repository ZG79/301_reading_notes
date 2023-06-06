## What is OAuth?
OAuth (Open Authorization) is an open standard framework that provides a secure way for users to grant access to their resources stored on one website or application to another website or application, without sharing their credentials, such as username and password, directly.

OAuth allows users to authorize third-party applications to access their data on various platforms (such as social media sites, online services, or APIs) on their behalf. It is commonly used by developers to enable authentication and authorization for their applications and APIs.

### Give an example of what using OAuth would look like.
When I use my google account to log into GitHub. 

### How does OAuth work? What are the steps that it takes to authenticate the user?

- User initiates authentication by accessing a client application or service.
- Client application requests authorization from the authorization server, specifying desired access scope.
- User is redirected to the authorization server to authenticate.
- User provides credentials and grants consent for requested access.
- Authorization server generates an authorization code.
- Authorization code is returned to the client application.
- Client exchanges the authorization code for an access token, authenticating itself.
- Access token is issued by the authorization server.
- Client application uses the access token to access protected resources on the resource server.
- Resource server validates the access token and provides access to requested resources.

### What is OpenID?

OpenID is an open standard and decentralized authentication protocol that allows users to use their existing accounts from an identity provider (IdP) to authenticate themselves on various websites or applications, without needing to create separate credentials for each service.

The primary goal of OpenID is to simplify the authentication process and reduce the burden of managing multiple usernames and passwords for different online platforms. It provides a single sign-on (SSO) solution, where users can use their existing identities to access multiple websites or applications that support OpenID.

### What is the difference between authorization and authentication?

Authentication establishes the identity of a user, while authorization determines what actions or resources that user is allowed to access based on their authenticated identity. Authentication verifies "who you are," while authorization determines "what you can do" after being authenticated. These two processes often work together in a secure system to ensure that only authenticated and authorized users can access the appropriate resources.

### What is Authorization Code Flow?

This flow can only be used for confidential applications (such as Regular Web Applications) because the application's authentication methods are included in the exchange and must be kept secure.

https://images.ctfassets.net/cdy7uua7fh8z/2nbNztohyR7uMcZmnUt0VU/2c017d2a2a2cdd80f097554d33ff72dd/auth-sequence-auth-code.png

### What is Authorization Code Flow with Proof Key for Code Exchange (PKCE)?

The Authorization Code Flow with Proof Key for Code Exchange (PKCE) is an extension of the OAuth 2.0 Authorization Code Flow that provides enhanced security for mobile and public client applications.

PKCE was designed to protect against authorization code interception attacks that can occur in certain environments, such as mobile apps or browser-based applications using JavaScript. These environments may be more susceptible to attacks where an intercepted authorization code could be exchanged for an access token without proper authorization.

### What is Implicit Flow with Form Post? 

Implicit Flow with Form Post is an OAuth 2.0 flow that allows client applications, typically web-based applications running in a browser, to obtain access tokens for authenticating and authorizing users.

### What is Client Credentials Flow?

The Client Credentials Flow is an OAuth 2.0 flow used for obtaining access tokens on behalf of a client application, without involving a specific user. This flow is typically used when the client application needs to authenticate and access protected resources independently.

### What is Device Authorization Flow?

Device Authorization Flow, also known as Device Flow or Device Code Flow, is an OAuth 2.0 authentication flow designed for devices that have limited input capabilities, such as smart TVs, gaming consoles, and Internet of Things (IoT) devices. It enables users to authenticate themselves on these devices by using a separate device with better input capabilities, such as a smartphone or a computer.

### What is Resource Owner Password Flow?


The Resource Owner Password Flow, also known as the Password Grant Type, is an OAuth 2.0 authentication flow that allows a client application to directly exchange the username and password of the resource owner (user) for an access token. This flow is typically used in scenarios where the client application is highly trusted and can securely handle the user's credentials.
