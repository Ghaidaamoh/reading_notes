# Component Lifecycle Events

## What are component lifecycle events?

React lets you define components as classes or functions. The methods that you are able to use on these are called lifecycle events.
**React Lifecycle Events**
![img](https://miro.medium.com/max/2800/0*0saPKFiTUk6W3FYp)
*The three phases of the component lifecycle*
- Mounting
When an instance of a component is being created and inserted into the DOM it occurs during the mounting phase. Constructor, static getDerivedStateFromProps, render, componentDidMount, and UNSAFE_componentWillMount all occur in this order during mounting.
- Updating
Anytime a component is updated or state changes then it is rerendered.
- Unmounting
The final phase of the lifecycle if called when a component is being removed from the DOM.
**componentWillUnmount is the only lifecycle event during this phase**
**constructor( )**
The constructor for a React component is called before it is mounted.If the component is a subclass you should call super(props), or the props will be undefined.
**static getDerivedStateFromProps( )**
This method exists for rare cases where the state relies on changes in props over time.
**render( )**
Render is the only required method in a class component.
**componentDidMount( )**
This method is invoked immediately after a component is mounted.
**shouldComponentUpdate( )**
The default behavior in react is to rerender after every state change.
**getSnapshotBeforeUpdate( )**
This is another rarely used method that allows you to capture a picture of the DOM to check it before actually changing anything on the DOM.
**componentDidUpdate( )**
This method is useful for performing network requests after a change has occurred.
**componentWillUnmount( )**
This method allows you to clean up the DOM and netwrok requests/ subscriptions.

**static getDerivedStateFromProps()**
This method exists for rare cases where the state relies on changes in props over time.
**render()**
Render is the only required method in a class component. It will examine this.props and this.state when called. The render function should not modify the component state because it would cause a lot of bugs by changing the state every time it rerenders. I also should not directly interact with the browser. render will not be invoked if shouldComponentUpdate() returns false. Here is an example of using render.
**componentDidMount()**
This method is invoked immediately after a component is mounted. If you need to load anything using a network request or initialize the DOM, it should go here. This method is a good place to set up any subscriptions. If you do that, don’t forget to unsubscribe in componentWillUnmount().
setState() can be called here, but it should be used sparingly, because it will cause a rerender, which can lead to perfomance issues.
**shouldComponentUpdate()**
The default behavior in react is to rerender after every state change. Setting shouldComponentUpdate() to false allows you to prevent this from happening. This is in order to optimize performance. If you want to use this method, it may be better to use PureComponent instead, which performs a shallow comparison of props and state. If you do decide to use this method, be sure to check the previous props and state with the current props and state. If shouldComponentUpdate() returns false, then UNSAFE_componentWillUpdate(), render(), and componentDidUpdate() will not be invoked.
**getSnapshotBeforeUpdate()**
This is another rarely used method that allows you to capture a picture of the DOM to check it before actually changing anything on the DOM.
**componentDidUpdate()**
This method is useful for performing network requests after a change has occurred.
**componentWillUnmount()**
This method allows you to clean up the DOM and netwrok requests/ subscriptions.