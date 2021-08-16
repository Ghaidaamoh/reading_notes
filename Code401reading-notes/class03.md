# Express REST API

- Name 3 real world use cases where you’d want to change the request with custom middleware

1. Handling errors
2. Adding query params
3. Make changes to the request and the response objects.

- True or false: The route handler is middleware?
  - False

**In what ways can a middleware function end the process and send data to the browser?**

- middleware functions that return a Promise will call next(value) when they reject or throw an error, next will be called with either the rejected value or the thrown Error.

**At what point in the request lifecycle can you “inject” middleware?**

- For injecting we will need to create the request, and create a middleware component that actually injects when making the request

**What can cause express to error with Request headers sent twice, cannot start a second response?**

- It's means that you're already in the Body or Finished state, but some function tried to set a header or statusCode. When you see this error, try to look for anything that tries to send a header after some of the body has already been written.

**Document the following Vocabulary Terms**

- **Middleware:** are functions that have access to the request object req, the response object res, and the next middleware function in the application’s request-response cycle. The next middleware function is commonly denoted by a variable named next.
- **Request Object:** is the main entry point for an application to issue a request to the Library - all operations on a URL must use a Request object.
- **Response Object:** It is the object which communicates between the server and the output which is sent to the client.
- **Application Middleware:** is software that lies between an operating system and the applications running on it. Essentially functioning as hidden translation layer, middleware enables communication and data management for distributed applications.
- **Routing Middleware:** It's means that the middleware functions can perform the following tasks:Execute any code,Make changes to the request and the response objects.
- **Test Driven Development:** is a software development process relying on software requirements being converted to test cases before software is fully developed,
- **Behavioral Testing:** is a structured study and analysis of a person’s behavior using various methods like interviews, direct supervision, and self-observation.