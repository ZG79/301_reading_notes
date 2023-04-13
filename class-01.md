# React and Component-Based Architecture

### What is a “component”?
A component is a modular, self-contained, and reusable piece of code that encapsulates a specific functionality or feature. It can be composed of different parts or sub-components and can interact with other components to create a more complex system. Components can be easily replaced, modified, or added without affecting the rest of the system, which makes it easier to maintain and scale the application.Each component has its own JS and CSS code, they are reusable, easier to read, write and test.
### What are the characteristics of a component?
- Reusability: Components can be reused in different contexts and applications.
- Encapsulation: A component is self-contained and its internal workings are hidden from other components.
- Composability: Components can be combined to form larger and more complex systems.
- Customizability: Components can be configured and customized to fit specific needs.
- Extensibility: Components can be extended with additional functionality.
- Replaceability: Components can be replaced with alternative implementations without affecting the rest of the system.
### What are the advantages of using component-based architecture?
The characteristics of the component are the advantages of using it. On top of that it's easy to develop for its clear separation of concerns, and reduced complexity. It is also easy to use for collaboration. 

### What is React component? 
- is a JavaScript / ES6 function
- must return a React element
- take props as parameter if necessary
 - React has 2 types of components: Functional (Stateless) and Class (Stateful).
 
 <strong>Functional (Stateless) component</strong>: a JavaScript (or ES6) function which returns a React element.
 ```js 
 function Welcome(props) {
  return <h1>Hello, {props.name}</h1>;
}
```
<strong>Class (Stateful) component </strong>: ES6 classes. They are more complex than functional components including constructors, life-cycle methods, render( ) function and state (data) management.
- is an ES6 class, will be a component once it ‘extends’ React component.
- can accept props (in the constructor) if needed
- can maintain its own data with state
- must have a render( ) method which returns a React element (JSX), or null
  
  ```js
  import React, { Component } from 'react';
  class Counter extends Component {
  constructor(props) {
    super(props);
    this.state = {
      count: 0
    };
  }
  incrementCount = () => {
    this.setState({ count: this.state.count + 1 });
  }
  render() {
    return (
      <div>
        <h1>Count: {this.state.count}</h1>
        <button onClick={this.incrementCount}>Increment</button>
      </div>
    );
    }
   }
   export default Counter;
  ```
  
  ## React Prop
  React is a component-based library that divides the UI into little reusable pieces. In some cases, those components need to communicate (send data to each other) and the way to pass data between components is by using props.
  
  “Props” is a special keyword in React, which stands for properties and is being used for passing data from one component to another.

But the important part here is that data with props are being passed in a uni-directional flow. (one way from parent to child)

Furthermore, props data is read-only, which means that data coming from the parent should not be changed by child components.
  
  
