# Authentication

- Hashing is a way for protecting passwords and considered to be pretty safe for ensuring the integrity of data or password.
- General-purpose hash function designed for speed,because they are often used to calculate checksum values for large data sets and files

- PROBLEMS WITH CRYPTOGRAPHIC HASH ALGORITHM:
    - Brute Force attack
    - Hash Collision attack

- Bcrypt is an adaptive hash function based on the Blowfish symmetric block cipher cryptographic algorithm and introduces a work factor (also known as security factor), which allows you to determine how expensive the hash function will be.

- basic access authentication is a method for an HTTP user agent (e.g. a web browser) to provide a user name and password when making a request. In basic HTTP authentication, a request contains a header field in the form of Authorization: Basic <credentials>, where credentials is the Base64 encoding of ID and password joined by a single colon :.

- JWT : JSON Web Token (JWT) is an open standard (RFC 7519) that defines a compact and self-contained way for securely transmitting information between parties as a JSON object. 

![](https://www.vaadata.com/blog/wp-content/uploads/2016/12/JWT_tokens_EN.png)

- JSON Web Tokens consist of three parts separated by dots (.), which are: 
    - Header: The header typically consists of two parts: the type of the token, which is JWT, and the signing algorithm being used, such as HMAC SHA256 or RSA.
    - Payload: contains the claims. Claims are statements about an entity (typically, the user) and additional data. 
    - Signature: used to verify the message wasn't changed along the way, and, in the case of tokens signed with a private key, it can also verify that the sender of the JWT is who it says it is.

## Terms

- Router Middleware : what it does actualy is to take the original request, and forward it to a sub handler according to the path example : "/home" for a GET request is mapped to function getHome that handle it and eventually send a response to the client on the behalf of the original handler.

- Dynamic Module Loading : provide an API for importing one module into another, and customizing the properties and behavior of that module when it is imported.

- Singleton Pattern : is a software design pattern that restricts the instantiation of a class to one "single" instance. 

- CRUD -> REST Method Matches : 
    - Create = PUT with a new URI
    - POST to a base URI returning a newly created URI
    - Read   = GET
    - Update = PUT with an existing URI
    - Delete = DELETE
- Mock Testing : is an approach to unit testing that lets you make assertions about how the code under test is interacting with other system modules.

### Resources: 

[OWASP](https://cheatsheetseries.owasp.org/cheatsheets/Authentication_Cheat_Sheet.html)
[bcrypt](https://www.npmjs.com/package/bcrypt)