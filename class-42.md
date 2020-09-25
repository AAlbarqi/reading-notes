# OAuth

- OAuth is an open standard for access delegation, commonly used as a way for Internet users to grant websites or applications access to their information on other websites but without giving them the passwords.

- OAuth 2 : The first step of OAuth 2 is to get authorization from the user. OAuth 2 provides several "grant types" for different use cases. The grant types defined are:

    - Authorization Code for apps running on a web server, browser-based and mobile apps
    - Password for logging in with a username and password (only for first-party apps)
    - Client credentials for application access without a user present
    - Implicit was previously recommended for clients without a secret, but has been superseded by using the Authorization Code grant with PKCE.

Roles: Applications, APIs and Users:

- The Third-Party Application: "Client"
The client is the application that is attempting to get access to the user's account. It needs to get permission from the user before it can do so.

- The API: "Resource Server"
The resource server is the API server used to access the user's information.

- The Authorization Server
This is the server that presents the interface where the user approves or denies the request. In smaller implementations, this may be the same server as the API server, but larger scale deployments will often build this as a separate component.

## Terms

- authentication : is the process of verifying the identity of a person or device.

- authorization : is a security mechanism used to determine user/client privileges or access levels related to system resources, including computer programs, files, services, data and application features.

- encryption : the method by which information is converted into secret code that hides the information's true meaning. 

- hashing : A hash function is a function which when given a key, generates an address in the table. Converting one value to another.

- session : a storage that consists of information on server-side.

- cookie : data, stored in small text files, on your computer.

- token : a symbol representing something. 

- Basic Auth : a simple authentication scheme built into the HTTP protocol. 

- encoding : the process of converting data from one form to another. 

- secret : digital authentication credentials (secrets).

- cryptography : a method of protecting information and communications through the use of codes, so that only those for whom the information is intended can read and process it.

#### Resources:
[OAuth](https://aaronparecki.com/oauth-2-simplified/)