# What is a component?

- Component-based architecture focuses on the decomposition of the design into individual functional or logical components that represent 
well-defined communication interfaces containing methods, events, and properties. It provides a higher level of abstraction and divides
the problem into sub-problems, each associated with component partitions.The primary objective of component-based architecture is to 
ensure component reusability.

- A component is a modular, portable, replaceable, and reusable set of well-defined functionality that encapsulates its implementation 
  and exporting it as a higher-level interface.It has an obviously defined interface and conforms to a recommended behavior common to 
  all components within an architecture.That is, a software component can be deployed independently and is subject to composition by 
  third parties.Component-oriented software design has many advantages over the traditional object-oriented approaches such as− Reduced
  time in market and the development cost by reusing existing components.

**Object-oriented view:** A component is viewed as a set of one or more cooperating classes.

**Conventional view:** It is viewed as a functional element or a module of a program that integrates the processing logic, the internal 
data structures that are required to implement the processing logic and an interface that enables the component to be invoked and data
to be passed to it.

**Process-related view:** In this view, instead of creating each component from scratch, the system is building from existing components 
maintained in a library. As the software architecture is formulated, components are selected from the library and used to populate the architecture.
A user interface component includes grids, buttons referred as controls, and utility components expose a specific subset of functions used in other components.

## What are the charactistics of a component?

- Reusability − Components are usually designed to be reused in different situations in different applications. However, some components may be 
  designed for a specific task.

- Replaceable − Components may be freely substituted with other similar components.

- Not context specific − Components are designed to operate in different environments and contexts.

- Extensible − A component can be extended from existing components to provide new behavior.

- Encapsulated − A A component depicts the interfaces, which allow the caller to use its functionality, and do not expose details of the internal 
  processes or any internal variables or state.

- Independent − Components are designed to have minimal dependencies on other components.


### What are the advantages of using component based architecture?

- Ease of deployment − As new compatible versions become available, it is easier to replace existing versions with no impact on the other components or the system as a whole.

- Reduced cost − The use of third-party components allows you to spread the cost of development and maintenance.

- Ease of development − Components implement well-known interfaces to provide defined functionality, allowing development without impacting other parts of the system.

- Reusable − The use of reusable components means that they can be used to spread the development and maintenance cost across several applications or systems.

- Modification of technical complexity − A component modifies the complexity through the use of a component container and its services.

- Reliability − The overall system reliability increases since the reliability of each individual component enhances the reliability of the whole system via reuse.

- System maintenance and evolution − Easy to change and update the implementation without affecting the rest of the system.

- Independent − Independency and flexible connectivity of components. Independent development of components by different group in parallel. Productivity for the software development and future software development.

# What is props short for?
React is a component-based library which divides the UI into little reusable pieces. «Props» is a special keyword in React, which stands for properties and is being used for passing data from one component to another.Furthermore, props data is read-only, which means that data coming from the parent should not be changed by child components.

## How are props used in React?

1. Firstly, define an attribute and its value(data)
2. Then pass it to child component(s) by using Props
3. Finally, render the Props Data

### What is the flow of props?
data with props are being passed in a uni-directional flow. (one way from parent to child).

# Intro to React:

**What Is React?**
React is a declarative, efficient, and flexible JavaScript library for building user interfaces. It lets you compose complex UIs from small and isolated pieces of code called “components”.

**we have three React components:**

- Square: The Square component renders a single **button** and the Board renders 9 squares.
- Game: The Game component renders a board with placeholder values which 
- Board 

**Introducing JSX**

- const element = **h1** Hello, world! **/h1**; This funny tag syntax is neither a string nor HTML.It is called JSX, and it is a syntax extension to JavaScript. 

- Why JSX? Instead of artificially separating technologies by putting markup and logic in separate files, React separates concerns with loosely coupled units called «components» that contain both.

## Rendering Elements:

- Rendering an Element into the DOM: We call this a “root” DOM node because everything inside it will be managed by React DOM.Applications built with just React usually have a single root DOM node. If you are integrating React into an existing app, you may have as many isolated root DOM nodes as you like.

- Updating the Rendered Element: React elements are immutable. Once you create an element, you can’t change its children or attributes. An element is like a single frame in a movie: it represents the UI at a certain point in time.With our knowledge so far, the only way to update the UI is to create a new element, and pass it to ReactDOM.render().

- React Only Updates What’s Necessary: React DOM compares the element and its children to the previous one, and only applies the DOM updates necessary to bring the DOM to the desired state.

### Components and Props:

- Components let you split the UI into independent, reusable pieces, and think about each piece in isolation. This page provides an introduction to the idea of components. 
- Composing Components: Components can refer to other components in their output. This lets us use the same component abstraction for any level of detail. A button, a form, a dialog, a screen: in React apps, all those are commonly expressed as components.