# Understanding The Problem Domain Is The Hardest Part Of Programming

- The big issue is that many problem domains are like a puzzle with a blurry picture or no picture at all.
  The real world is a messy place.  Many of the problem domains we face as programmers are difficult to
  understand and look completely different depending on your viewpoint.As programmers, we also are often
  not given complete information about the problem domain, so we don’t even have the information we need to understand it.
**Programming is easy if you understand the problem domain**

**javascript book:**
## chap3:

- WHAT IS AN OBJECT?
  Objects group together a set of variables and functions to create a model of a something you would recognize
  from the real world. In an object, variables and functions take on new names.

- IN AN OBJECT: VARIABLES BECOME KNOWN AS PROPERTIES If a variable is part of an object, it is called a
  property.

- IN AN OBJECT: FUNCTIONS BECOME KNOWN AS METHODS If a function is part of an object, it is called a method.
  Methods represent tasks that are associated with the object.

- Using an Object Literal:
- This is the easiest way to create a JavaScript Object.
- define and create an object in one statement.
- An object literal is a list of name.

  **Example:**

  ![object](https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcTBd3OT2JANly_EQTRnkaXgc8n4dcGHVEBd1w&usqp=CAU)

- **Property access:**
  object.property
  object['property']

### chap5:

**The Document Object Model**:  (DOM) specifies how browsers should create a model of an HTML
  page and how JavaScript can access and update the contents of a web page while it is in the browser window.
**THE DOM TREE IS A MODEL OF A WEB PAGE**  As a browser loads a web page, it creates a model of that page.
  The model is called a DOM tree, and it is stored in the browsers' memory. It consists of four main types of nodes.
**WORKING WITH THE DOM TREE**

- Accessing and updating the DOM tree involves two steps:
1. Locate the node that represents the element you want to work with.
2. Use its text content, child elements, and attributes.

- The browser represents the page using a DOM tree.
- DOM trees have four types of nodes: document nodes, element nodes, attribute nodes, and text nodes.
- You can select element nodes by their id or cl ass attributes, by tag name, or using CSS selector syntax.
- Whenever a DOM query can return more than one node, it will always return a Nadel i st.
- From an element node, you can access and update its content using properties such as textContent and
  innerHTML or using DOM manipulation techniques.
- An element node can contain multiple text nodes and child elements that are siblings of each other.
- In older browsers, implementation of the DOM is inconsistent (and is a popular reason for using jQuery).
- Browsers offer tools for viewing the DOM tree .