# REST

#### SuperAgent
SuperAgent is light-weight progressive ajax API crafted for flexibility, readability, and a low learning curve after being frustrated with many of the existing request APIs. It also works with Node.js!

##### Request basics

A request can be initiated by invoking the appropriate method on the request object, then calling .then() (or .end() or await) to send the request.

`request
   .get('/search')
   .then(res => {
      // res.body, res.headers, res.status
   })
   .catch(err => {
      // err.message, err.response
   });`

`request('GET', '/search').then(success, failure);` : //HTTP method may also be passed as a string

**DELETE, HEAD, PATCH, POST**, and **PUT** requests can also be used, simply change the method name:
request
`.head('/favicon.ico').then(res => { });`

The HTTP method defaults to GET, so if you wish, the following is valid:

`request('/search', (err, res) => { });`

###### Serializing request body

SuperAgent will automatically serialize JSON and forms. You can setup automatic serialization for other types as well:
`request.serialize['application/xml'] = function (obj) {`
    `return 'string generated from obj'; };`

###### Retrying requests

When given the .retry() method, SuperAgent will automatically retry requests, if they fail in a way that is transient or could be due to a flaky Internet connection.

 `.get('https://example.com/search')
   .retry(2) // or:
   .retry(2, callback)
   .then(finished);
   .catch(failed);`

###### Setting Accept

In a similar fashion to the .type() method it is also possible to set the Accept header via the short hand method .accept(). 
- `request.get('/user').accept('application/json')`
- `request.get('/user').accept('json')`
- `request.post('/user').accept('png')`

##### Query strings
req.query(obj) is a method which may be used to build up a query-string. For example populating ?format=json&dest=/login on a POST:
`request
  .post('/')
  .query({ format: 'json' })
  .query({ dest: '/login' })
  .send({ post: 'data', here: 'wahoo' })
  .then(callback);`

###### Cross-Origin Resource Sharing (CORS)

Cross-Origin Resource Sharing (CORS) is a mechanism that uses additional HTTP headers to tell browsers to give a web application running at one origin, access to selected resources from a different origin.
