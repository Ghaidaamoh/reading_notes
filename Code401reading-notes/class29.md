# Advanced State with Reducers

**How can we ensure that an effect hook runs only once?**

- If we pass an empty array [] , it just renders the component only once like componentDidMount.

**Can useState() update more than one state variable at the same time ❓**

- Unlike the setState in class components, the setState returned from useState doesn't merge objects with existing state, it replaces the object entirely.

**Is useState() synchronous?**

- no , useState() doesn’t update value of the variable if called just after setting value.

## Terms

- State Hook: Hook state is the new way of declaring a state in React app. Hook uses useState() functional component for setting and retrieving state.

- Component Lifecycle: Each component in React has a lifecycle which you can monitor and manipulate during its three main phases. The three phases are: Mounting, Updating, and Unmounting.