# SENDING FORM DATA

### Client/server architecture

![](https://media.prod.mdn.mozit.cloud/attachments/2012/11/20/4291/c1a4a06f1fd9ed42ec5b06e814dd3111/client-server.png)

An HTML form on a web page is nothing more than a convenient user-friendly way to configure an HTTP request to send data to a server. This enables the user to provide information to be delivered in the HTTP request.

### On the client side: defining how to send the data

The <form> element defines how the data will be sent. All of its attributes are designed to let you configure the request to be sent when a user hits a submit button. The two most important attributes are `action` and `method`.

#### The action attribute 
The action attribute defines where the data gets sent. Its value must be a valid relative or absolute URL. If this attribute isn't provided, the data will be sent to the URL of the page containing the form — the current page. 
`<form action="/somewhere_else">`

#### The method attribute
The method attribute defines how data is sent. The most common being the GET method and the POST method.
1. The GET method: is the method used by the browser to ask the server to send back a given resource.
Example: `<form action="http://www.foo.com" method="GET">`

The data is appended to the URL as a series of name/value pairs. After the URL web address has ended, we include a question mark (?) followed by the name/value pairs, each one separated by an ampersand (&). In this case we are passing two pieces of data to the server:
    - say, which has a value of Hi
    - to, which has a value of Mom
2. The POST method: It's the method the browser uses to talk to the server when asking for a response that takes into account the data provided in the body of the HTTP request
Example: `<form action="http://www.foo.com" method="POST">`
When the form is submitted using the POST method, you get no data appended to the URL.

**Notes** :
1. If you need to send a password (or any other sensitive piece of data), never use the GET method or you risk displaying it in the URL bar, which would be very insecure.
2. If you need to send a large amount of data, the POST method is preferred because some browsers limit the sizes of URLs. In addition, many servers limit the length of URLs they accept.

### On the server side: retrieving the data
Whichever HTTP method you choose, the server receives a string that will be parsed in order to get the data as a list of key/value pairs.
There are many server-side technologies you can use for form handling, including Perl, Java, .Net, Ruby, etc.

![styling HTML5 Form](https://www.youtube.com/playlist?list=PL4cUxeGkcC9g5_p_BVUGWykHfqx6bb7qK)
[HTML FORMS](https://htmlreference.io/forms/)