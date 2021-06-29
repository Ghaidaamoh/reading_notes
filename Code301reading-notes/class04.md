
# React Docs - Forms

 - What is a Controlled Component?
   - The form elements in HTML they maintain their own state and update it based on user input, but in React,the state for them is typically kept in the state property of components, and only updated with setState().So Controlled Component allow us to combine the two by making the React state be the single source of truth ,which means that the React component that renders a form also controls what happens in that form on subsequent user input.

- Should we wait to store the users responses from the form into state when they submit the form OR should we update the state with their responses as soon as they enter them? Why.
   - We update it as soon as they enter , because we are using an event handler that is runs on every keystroke to update the React state, the displayed value will update as the user types.

- How do we target what the user is entering if we have an event handler on an input field?
   -By using the {this.handleChange} with the same input field .

## The Conditional (Ternary) Operator Explained

- Why would we use a ternary operator?
   - It's allow us to write the condition code in just one line of code.

- Rewrite the following statement using a ternary statement:

if(x===y){

console.log(true);

} else {

console.log(false);

}

x===y ? 'true' : 'false';

