# Node JS Tutorial for Beginners #6 - Modules and require()

 - What is a module?
   - Just to orgnize our application code into different files. It's a way to split the code into a logical modules,and each module for each code that have a certain functionality and we cal call them whenever we need them.

- What does the word requiredo?
   - It's a function that we use it when we need to use one function into another file.Which mean it's global in the nodeJs and we can use it anywhere

- How do we bring another module into the file the we are working in?
   - We choose which part we want to pass it and we export it by using the module.exports

- What do we have to do to make a module available?
   - We pass the name of the module we want inside the module.exports method.
     Example: module.exports=module_name
    - Then we declare it as avariable in the file we want it to be used in, in the reqiure section
     Example:
     `let function_name = require ('./the name of the function')
