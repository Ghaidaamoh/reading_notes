**Domain Modeling**

**Domain modeling** is the process of creating a conceptual model in code for a specific problem. 
A model describes the various entities, their attributes and behaviors, as well as the constraints 
that govern the problem domain.

**Model epic fails videos**

Imagine you've been tasked to build a program that models the popularity of epic fail videos. 
After months of painstaking research, you've determined that the two essential metrics for gauging 
popularity are an epic rating and whether or not the video has animals. That way, when you need to 
change the algorithm for determining popularity, the changes will be small and targeted.

**Here's some tips to follow when building your own domain models**

- When modeling a single entity that'll have many instances, build self-contained objects with the same attributes and behaviors.
- Model its attributes with a constructor function that defines and initializes properties.
- Model its behaviors with small methods that focus on doing one job well.
- Create instances using the new keyword followed by a call to a constructor function.
- Store the newly created object in a variable so you can access its properties and methods from outside.
- Use the this variable within methods so you can access the object's properties and methods from inside.

# HTML& CSS books:

**chap6**
**Tables**

- What's a Table? A table represents information in a grid format. 
- Basic Table Structure:

1. **table:** The **table** element is used to create a table. The contents of the table are written out row by row.
2. **tr:** You indicate the start of each row using the opening <tr> tag. 

(The tr stands for table row.) It is followed by one or more **td** elements (one for each cell in that row). 
At the end of the row you use a closing **/tr** tag.
**td** Each cell of a table is represented using a <td>element. (The td stands for table data.)

**Table Headings** 
**th:** The **th** element is used just like the <td> element but its purpose is to represent the 
heading for either a column or a row. (The th stands for table heading.) 

**Long Tables:**

- **thead** The headings of the table should sit inside the <thead> element. 
- **tbody** The body should sit inside the <tbody> element. 
- **tfoot** The footer belongs inside the <tfoot> element.


## javascript book:

**chap3:**

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

- **Property access:**
  object.property
  object['property']

**Function:**

- Functions allow you to group a set of related statements together that represent a single task. 
- Functions can take parameters (informatiorJ required to do their job) and may return a value. 
- Web browsers implement objects that represent both the browser window and the document loaded into the 
browser window. 
- JavaScript also has several built-in objects such as String, Number, Math, and Date. Their properties and 
methods offer functionality that help you write scripts. 
- Arrays and objects can be used to create complex data sets (and both can contain the other). 



