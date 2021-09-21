# Reading: Component Lifecycle / useEffect() Hook

- Using this Hook, we tell React that the component needs to do something after render.

**Why do we not need more .html pages in a multi-page React app?**

- A single-page application is an application that loads a single HTML page and all the necessary assets (such as JavaScript and CSS) required for the application to run. Any interactions with the page or subsequent pages do not require a round trip to the server which means the page is not reloaded.

**If we wanted a component to show up on every page, where would we put it and why? Outside the Inside the , outside a Inside a**

- will be inside the Route that will be as an instance of BrowserRouter, to allow the React App render needed component that is exisiting inside the Route, and each time the active route “by path” will be rendered.

**What does routing do with the components that were rendered when a new route is requested**

- in switch component from React-router, first route will match the clicked path will be rendered, and will go out the switch and will not see or render the other components.

**What does props.children contain?**

- children is a special property of React components which contains any child elements defined within the component, e.g. the divs inside Example above. {this.props.children} includes those children in the rendered result.

**How do useState() and this.setState() differ?**

- The setState function is used to handle the state object in a React class component.
- setState is merging the previous state with the new one, it means that you dont have to pass the full state object every time you want to change some part of the state. React will update given properties and won’t touch the rest. The useState’s updater rewrites a previous state with a new one and it does not perform any merging. Its just replacement instead of merging.

## Terms:

- State Hook: Hook state is the new way of declaring a state in React app. Hook uses useState() functional component for setting and retrieving state.

- Mounting and Un-Mounting:

  - Mounting is the process of outputting the virtual representation of a component into the final UI representation (e.g. DOM or Native Components).

  - Un-Mounting is the last function to be called immediately before the component is removed from the DOM.