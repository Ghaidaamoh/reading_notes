# In memory storage

**What is a refrence error?**
- The call stack is primarily used for function invocation (call).
- The call stack is synchronous.
- A call stack is a data structure that uses the Last In, First Out (LIFO) principle to temporarily store and     manage function invocation (call).
- the last function that gets pushed into the stack is the first to be pop out .
- The call stack maintains a record of the position of each stack frame.
- A stack overflow occurs when there is a recursive function (a function that calls itself) without an exit point.
  
## What is a refrence error?

- Types of error messages :

1. Reference errors :

- This happens when trying to reach variables that are not yet declared .
- or hoisting let and const that takes time to hoist .
- to fix this error declare before initialization .

2. Syntax errors:

- this occurs when you have something that cannot be parsed in terms of syntax .
- Ex : parse an invalid object using JSON.parse.
- This can be solved by just fixing the syntax .

3. Range errors:

- manipulate an object with some kind of length and give it an invalid length IS THE CAUSE .
- The best approach and best practice is ti immute your variables and don't mess with the lengths .

4. Type errors:

- his types of errors show up when the types (number, string and so on) you are trying to use or access are    incompatible .
- To fix this make atesting variable or test if the variable or object exists .

5. Debugging:

- To debug your JS code, the easiest and maybe the most common way its to simply console.log() .
- by using chrome developer tools .
- The breakpoint can also be achieved by putting a debugger statement in your code in the line you want to break.

5. Handling errors:

- We use try and catch to handle errors .
- That will make errors not to break the whole code .
- The errors will show in a different way.

6. Tools for preventing runtime Errors :

- quokka to evaluate your code as you type
- eslint to make sure your style guide is consistency and it will grab you an error or two along the way and For those of you looking to make JS a more strong typed experience you can check out stuff like TypeScript (like I said in a previous article, when learning I rather avoid libraries that abstract the core language so I wouldn’t recommend this last one when starting).