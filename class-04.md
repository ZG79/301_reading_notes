
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
