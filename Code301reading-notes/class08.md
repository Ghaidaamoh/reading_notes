# API Design Best Practices

 - What does REST stand for?
   - It's referse to Roy Fielding proposed Representational State Transfer,and it's an architectural approach to designing web services,which considered a style for building distributed systems based on hypermedia.

- REST APIs are designed around a ____.
   - Resources, which are any kind of object, data, or service that can be accessed by the client.Resource has an identifier.

- What is an identifer of a resource? Give an example.
   - It's URI that uniquely identifies that resource.
     Example:
     HTTP
     https://adventure-works.com/orders/1

- What are the most common HTTP verbs?
   -  The most common operations are GET, POST, PUT, PATCH, and DELETE.

- What should the URIs be based on?
   - The URIs should be based on nouns the resource and not verbs the operations on the resource.

- Give an example of a good URI.
   - https://adventure-works.com/orders

- What does it mean to have a ‘chatty’ web API? Is this a good or a bad thing?
   - That's means the web APIs that expose a large number of small resources.And it's a bad thing we should try to avoid chatty web APIs.

- What status code does a successful GET request return?
   - It's returns HTTP status code 200 (OK).

- What status code does an unsuccessful GET request return?
   - It's return 404 (Not Found).

- What status code does a successful POST request return?
   - It's return HTTP status code 200.

- What status code does a successful DELETE request return?
   - It's respond with HTTP status code 204.
  
