# Authentication

**Explain what a Singleton is in Computer Science terms**

- A singleton is a class that allows only a single instance of itself to be created and gives access to that created instance. It contains static variables that can accommodate unique and private instances of itself.

**Explain how the Singleton pattern can be used with Node modules, specifically with classes**

- The singleton pattern is used in programming languages such as Java and .NET to define a global variable.
- Creating singleton in Node.JS is very easy. When we take advantage of Node.JS caching then this is trivial. In this article we showed two ways of achieving the same results and I strongly recommend to use the latter one.

## If you were tasked with building a middleware system like Express uses, what approach might you take to construct/operate it?

- Bind application-level middleware to an instance of the app object by using the app.use() and app.METHOD() functions, where METHOD is the HTTP method of the request that the middleware function handles such as GET, PUT, or POST in lowercase.

### Document the following Vocabulary Terms

- Router Middleware: Router is used to manage these incoming requests. It kind of routes your requests to correct handler/code

- Dynamic Module Loading: is a mechanism by which a computer program can, at run time, load a library or other binary into memory, retrieve the addresses of functions and variables contained in the library, execute those functions or access those variables, and unload the library from memory.

- Singleton Pattern: is a software design pattern that restricts the instantiation of a class to one single instance.

- CRUD -> REST Method Matches: CRUD stands for Create, Read, Update, and Delete, which are four primitive database operations. At first glance, these operations map well to the HTTP verbs most frequently used in REST POST , GET , PUT ,DELETE

- Mock Testing: is an approach to unit testing that lets you make assertions about how the code under test is interacting with other system modules. In mock testing, the dependencies are replaced with objects that simulate the behaviour of the real ones.