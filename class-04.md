
https://transform.tools/html-to-jsx - JSX converter

## Forms
### Form components 
These built-in browser components accept user input:
```js
<input>
<select>
<textarea>
```
They are special in React because passing the value prop to them makes them controlled.

### Controlling an input with a state variable 
An input like `<input />` is uncontrolled. Even if you pass an initial value like `<input defaultValue="Initial text" />`, your JSX only specifies the initial value. It does not control what the value should be right now.

To render a controlled input, pass the value prop to it (or checked for checkboxes and radios). React will force the input to always have the value you passed. Usually, you would do this by declaring a state variable:

### What is a ‘Controlled Component’?
In React, a controlled component is a form element (like input, textarea, select, etc.) whose value is controlled by React through its state. This means that the value of the form element is not stored in the DOM, but rather in the component's state, and the component updates its state based on the user input.

When a form element is a controlled component, its value is passed as a prop from the parent component, and it also receives an onChange prop, which is a callback function that is called whenever the value of the form element changes. When the user types something into the form element, the onChange function is called, and it updates the component's state with the new value. Then, React re-renders the component with the new value of the form element.

### Should we wait to store the users responses from the form into state when they submit the form OR should we update the state with their responses as soon as they enter them? Why.

There are reasons we need to wait to store the user's response from the form into the state until they submit the form. Because whenever the state changes React rerenders the application so it'll be inefficient to rerender unnecessary times. Unnecessary rerendering will slow down the application and there is a risk to store incomplete data. 

### How do we target what the user is entering if we have an event handler on an input field?
We will use the `event.target.value` property.

## The Conditional (Ternary) Operator

Shorthand for if else statement:
```js
condition ? expressionIfTrue : expressionIfFalse;
```
### Why would we use a ternary operator?
Concise and easy to read.

### Rewrite the following statement using a ternary statement:

```js
if(x===y){
  console.log(true);
} else {
  console.log(false);
}
```
```js
x===y ? console.log(true) : console.log(false)
```
