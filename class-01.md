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
  
## 19 keypoints about React

React is a popular JavaScript library for building user interfaces. It allows you to create reusable UI components and efficiently update and render them based on changes in application state.

React follows a component-based architecture, where the user interface is divided into independent and reusable components. Each component encapsulates its own logic and state.

React uses a virtual DOM (Document Object Model) to optimize the rendering process. It creates a lightweight representation of the actual DOM, allowing React to efficiently update only the necessary parts of the UI when the application state changes.

JSX (JavaScript XML) is an extension of JavaScript used in React. It allows you to write HTML-like code within JavaScript, making it easier to define the structure and appearance of components.

React utilizes a unidirectional data flow. The application state is stored in a central place and passed down to child components as props. Child components can trigger updates by invoking callback functions passed to them.

React provides lifecycle methods that allow you to hook into different stages of a component's lifecycle, such as mounting, updating, and unmounting. This enables you to perform actions like fetching data or cleaning up resources at the appropriate times.

React emphasizes the concept of reusable and composable components. By breaking down the UI into smaller components, you can create a library of reusable elements that can be combined to build complex user interfaces.

React offers a virtual DOM diffing algorithm that efficiently calculates and applies the minimal set of changes required to update the UI. This minimizes the performance impact of rendering updates and ensures a smooth user experience.

React provides a way to manage component-specific state using the useState hook. With this hook, you can define and update local state within a component without the need for class-based components.

React supports conditional rendering, allowing you to show or hide components based on certain conditions. You can use JavaScript expressions or conditional statements to control the visibility of components.

React supports the concept of "props" (short for properties) that allow data to be passed from parent components to child components. Props are immutable and provide a way to communicate and share data between components.

React encourages a declarative approach to building user interfaces. Instead of directly manipulating the DOM, you define how the UI should look based on the current state and let React handle the updates.

React provides a way to handle user interactions and events through event handlers. You can attach event handlers to elements and components to respond to user actions, such as clicks or form submissions.

React supports the concept of "hooks," which are functions that allow you to add additional capabilities to functional components. Hooks, such as useEffect and useContext, enable you to work with side effects and access context within functional components.

React supports the concept of "controlled components" where the component's state is controlled by the application rather than the component itself. This allows for centralized state management and easier form handling.

**React can be used in conjunction with other libraries and frameworks to build complete applications. Popular choices include React Router for handling routing, Redux for state management, and Axios for making HTTP requests.**

React has a strong and active community, with numerous open-source libraries and resources available. You can leverage these resources to enhance your development experience and find solutions to common challenges.

React Native is a framework built on top of React that allows you to develop native mobile applications using JavaScript. It shares many concepts and principles with React, making it easier to transition between web and mobile development.

React provides tools like React Developer Tools and error boundaries that aid in debugging and troubleshooting React applications.
