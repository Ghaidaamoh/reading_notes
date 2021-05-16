# javascript books:

**chap10**
![image](https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcRg6NV17XZpaojHC8x40vQUcPZOKaxDV0EjxQ&usqp=CAU)

**Error Handling & Debugging**

- When you are writing JavaScript, do not expect to write it perfectly the first time Programming is like problem solving: 
  you are given a puzzle and not only do you have to solve it, but you also need to create the instructions that allow the
  computer to solve it.

- When writing a long script, nobody gets everything right in their first attempt. The error messages that a browser 
  gives look cryptic at first, but they can help you determine what went wrong in your JavaScript and how to fix it. 

1. **THE CONSOLE & DEV TOOLS** Tools built into the browser that help you hunt for errors.
2. **COMMON PROBLEMS** Common sources of errors, and how to solve them. 
3. **HANDLING ERRORS** How code can deal with potential errors gracefully. 

- **ORDER OF EXECUTION**To find the source of an error, it helps to know how scripts are processed. The order in which statements are 
    executed can be complex; some tasks cannot complete until another statement or function has been run.
- **EXECUTION CONTEXTS** The JavaScript interpreter uses the concept of execution contexts.There is one global execution context; plus, 
    each function creates a new new execution context. 
- **UNDERSTANDING ERRORS** If a JavaScript statement generates an error, then it throws an exception. At that point, the interpreter
    stops and looks for exception-handl ing code.
- If you understand execution contexts (which have two stages) and stacks, you are more likely to find the error 
in your code. 
- Debugging is the process of finding errors. It involves a process of deduction. 
- The console helps narrow down the area in which the error is located, so you can try to find the exact error. 
- JavaScript has 7 different types of errors. Each creates its own error object, which can tell you its line number 
and gives a description of the error. 
- If you know that you may get an error, you can handle it gracefully using the try, catch, finally statements. 
Use them to give your users helpful feedback.

  