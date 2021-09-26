# Context API

**Describe use cases useState() vs useReducer()**

- useState is a Basic Hook for managing simple state transformation and useReducer is an Additional Hook for managing more complex state logic, it is worth noting that useState uses the useReducer internally. This implies that you could use useReducer for everything you can do with useState.

- useReducer is usually preferable to useState when you have complex state logic that involves multiple sub-values or when the next state depends on the previous one. useReducer also lets you optimize performance for components that trigger deep updates because you can pass dispatch down instead of callbacks.

**Why do custom hooks need the use prefix?**

- Custom hooks are normal JS functions, named with the prefix ‘use’, that can use hooks inside of it and contain a common stateful logic to be reused in other components.

**What do custom hooks usually do?**

- Custom React hooks can help us with some very important principles of good software architecture, such as code readability, separation of concerns, and avoiding code duplication. In this article we’ll see how we can encapsulate fetch calls, logic, caching, and component state, all inside a custom React Hook.

- React Hooks allow us to use the component’s state, to hook into the component’s lifecycle, and to use other React features in functional components, like we usually do in class components.

**Using any list of custom hooks, research and name one that you think will be useful in your applications**

1. useClippy A hook for copying data to the clipboard and retrieving/pasting it using Ctrl-C/Command-C and Ctrl-V/Command-V.

2. useBrowserContextCommunication useBrowserContextCommunication uses the Broadcast Channel API to deliver an easy solution for communication between different browser contexts (tabs, iframes, windows).

3. useScript useScript is a hook for loading (and notifying when they’re loaded) external scripts, dynamically.

**Describe how a hook that fetches API data might work**

- Wish I knew but I couldn’t get this to work in my lab :). Jokes aside I imagine they all would have a similar structure but have slight variations based on the route and the method you’re using.

## Term	

- reducer: are functions that take the current state and an action as arguments, and return a new state result.

