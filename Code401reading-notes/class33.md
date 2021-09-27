# Login and Auth

**Why is the Context API useful?**

- Because it's enables you to exchange unique details and assists in solving prop-drilling from all levels of your application.

**Can a component outside of a provider get its context?**

- Yes we can call useContext in each component to pull out the values we need. It doesn’t matter how far apart the components are as long as they’re wrapped in a provider.

**What are some common use cases for using the Context API?**

- Some sample use cases where the Context API proves helpful are:
   - Theming — Pass down app themei
   - 18n — Pass down translation messages
   - Authentication — Pass down current authenticated user

**Describe “Context Hell”**

- the React Context hell is the nasty code you get taking advantage of the React Context API.

- How to fix it?
    - To clean up the nasty code you get from taking advantage of React Context API we need a way to nest multiple Context.Provider without passing them as children of each other.

    - To achieve that we can use the React.cloneElement API.

    - The cloneElement API

## Terms

- global state: a global state is a set of local states which are all concurrent with each other

- global context: it's designed to share data that can be considered “global” for a tree of React components, such as the current authenticated user, theme, or preferred language.

- provider: Provider React component that allows consuming components to subscribe to context changes.

- consumer: A React component that subscribes to context changes. Using this component lets you subscribe to a context within a function component

### what is role based access control?

- Role-based access control (RBAC) restricts network access based on a person's role within an organization and has become one of the main methods for advanced access control.

- Some of the designations in an RBAC tool can include:
  - Management role scope – it limits what objects the role group is allowed to manage.
  - Management role group – you can add and remove members.
  - Management role – these are the types of tasks that can be performed by a specific role group.
  - Management role assignment – this links a role to a role group.

**react-cookies component**

- Cookies are the data stored in the form of key-value pairs that are used to store information about the user on their computer by the websites that the users browse and use it to verify them.

- To set or remove the cookies, we are going to use a third-party dependency of react-cookie.

