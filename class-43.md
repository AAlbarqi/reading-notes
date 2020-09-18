# Bearer Authorization

- JWT: JSON Web Token (JWT) is an open standard (RFC 7519) that defines a compact and self-contained way for securely transmitting information between parties as a JSON object.

![](https://research.securitum.com/wp-content/uploads/sites/2/2019/10/jwt_ng1_en.png)

- JWTs can be either signed, encrypted or both. If a token is signed, but not encrypted, everyone can read its contents, but when you don't know the private key, you can't change it. Otherwise, the receiver will notice that the signature won't match anymore.

![](https://thepracticaldev.s3.amazonaws.com/i/lzhrko3j6l8uut86tkz1.png)

## Terms

- Client ID : At registration the client application is assigned a client ID and a client secret (password) by the authorization server. The client ID and secret is unique to the client application on that authorization server.

- Authentication Endpoint : is an authentication mechanism used to verify the identity of a network's external or remote connecting device.

- Access Token Endpoint : an HTTP endpoint that micropub clients can use to obtain an access token given an authorization code.

- API Endpoint : a point at which an application program interface (API) -- the code that allows two software programs to communicate with each other -- connects with the software program.

- Authorization Code : used for any transaction or entry that has restrictions on which users are entitled to access.

- Access Token : an object encapsulating the security identity of a process or thread.