# React Lifecycle
The React lifecycle has three phases to monitor and manipulate the component. The phases are: 
- Mounting: Putting elements into the DOM. There are 4 built-in method that gets called, when mounting.
  - constructor()
  - getDerivedStateFromProps()
  - render()
  - componentDidMount()
- Updating: When a component is updated, whenever there us a change in the component's state or peops. There are 5 built-in methods.
  - getDerivedStateFromProps()
  - shouldComponentUpdate()
  - render()
  - getSnapshotBeforeUpdate()
  - componentDidUpdate()
- Unmounting: when a component is removed from the DOM. There is only one built-in method for this stage. 
  - componentWillUnmount()
### Based off the diagram, what happens first, the ‘render’ or the ‘componentDidMount’?
Since the render method is responsible for rendering component (outputs the HTML to the DOM)TO THE DOM, while 'componentDidMount' gets called immediately after the component is mounted in the DOM, the render happens first. It provides an opportunity to interact with the DOM or perform any necessary setup after the component has been rendered.
### What is the very first thing to happen in the lifecycle of React?
The very first thing to happen in the lifecycle of a React component is the creation of the component instance. This is done by calling the component constructor, which is responsible for initializing the component's state and binding the component's methods to the component instance.
### Put the following things in the order that they happen: componentDidMount, render, constructor, componentWillUnmount, React Updates
Constructor, Render, React Updates, componentDidMount, componentWillUnmount.
- Constructor: This is the first method to be called when a component is created, and it is responsible for setting up the component's initial state and binding any necessary event handlers.

- Render: After the constructor has finished executing, the render method is called, which generates the initial markup for the component based on its props and state.

- React Updates: If the component's props or state change, React will re-render the component and update the DOM accordingly.

- componentDidMount: After the initial render, the componentDidMount method is called, which gives the component a chance to perform any necessary setup work, such as fetching data from a server or adding event listeners.

- componentWillUnmount: Finally, when the component is about to be removed from the DOM, the componentWillUnmount method is called, which gives the component a chance to perform any necessary cleanup work, such as removing event listeners or cancelling any outstanding network requests.
### What does componentDidMount do?
This method is called after the component is rendered(inserted into the DOM) for the first time. This method is a good place to perform any initialization tasks that require access to the DOM or to external data sources, such as fetching data from a server or setting up event listeners.
### What types of things can you pass in the props?
rops can be used to pass any type of data that can be represented in JavaScript. The key is to make sure that the data being passed is immutable and that the child component is designed to handle the props in a way that is consistent with its intended behavior.
### What is the big difference between props and state?
Props you pass into the component, and the state is handled inside of the component and you can update the component, while props are handled outside of the component and must updated outside of the component. 
### When do we re-render our application?
When you change the state inside of your application, it's going to re-render the section of that application. 
### What are some examples of things that we could store in state?
When the user changes/updated something it's stored in the state. 

tips: which one is handled by the component. 

If only in the component: state

if handling outside: props (inherit from the parent)

## 17 keypoints of React lifecycle

The React component lifecycle consists of three main phases: Mounting, Updating, and Unmounting.

Mounting phase: This phase occurs when a component is being created and inserted into the DOM. It includes the following lifecycle methods:

constructor: The constructor is called before a component is mounted. It is used for initializing state and binding event handlers.
render: The render method is responsible for returning the JSX that represents the component's UI.
componentDidMount: This method is invoked immediately after a component is mounted and inserted into the DOM. It is commonly used for performing initial setup, fetching data from APIs, or setting up event listeners.
Updating phase: This phase occurs when a component's state or props are updated. It includes the following lifecycle methods:

render: The render method is called again to update the UI based on the new state or props.
componentDidUpdate: This method is invoked after the component has been updated and re-rendered. It is often used for side effects, such as making additional API requests based on the updated data or interacting with the DOM.
Unmounting phase: This phase occurs when a component is being removed from the DOM. It includes the following lifecycle method:

componentWillUnmount: This method is called just before a component is unmounted and destroyed. It is commonly used for cleaning up resources, such as removing event listeners or canceling API requests.
React introduced a new set of lifecycle methods known as "lifecycle hooks" with the introduction of React Hooks. These hooks provide a way to add lifecycle-like behavior to functional components. The most commonly used hooks include useEffect, useCallback, and useMemo.

useEffect hook: This hook replaces componentDidMount, componentDidUpdate, and componentWillUnmount lifecycle methods. It allows you to perform side effects, such as data fetching or subscribing to events, within a functional component.

The useEffect hook takes a callback function as its first argument, which is executed after every render. You can specify dependencies as a second argument to control when the effect should run.

useCallback hook: This hook is used to memoize functions and prevent unnecessary re-renders of child components that depend on these functions.

useMemo hook: This hook is used to memoize the result of a computation and cache it so that it is not recalculated on every render.

With the introduction of React 16.3, some lifecycle methods have been deprecated and replaced with safer alternatives. For example, componentWillMount, componentWillReceiveProps, and componentWillUpdate have been replaced with constructor and getDerivedStateFromProps.

getDerivedStateFromProps: This static lifecycle method is invoked after a component is instantiated as well as before it receives new props. It allows you to update the state based on changes in props. However, it is recommended to use this method sparingly, as it can make the component's behavior complex.

The shouldComponentUpdate method allows you to control whether a component should re-render or not. By default, it returns true, but you can optimize performance by implementing custom logic to determine when a component should update.

React provides a way to catch errors in components using the componentDidCatch lifecycle method. This method is called when an error occurs during rendering, in a lifecycle method, or in the constructor of any child component.

React 17 introduced some changes to the lifecycle behavior


```js
import React, { Component } from 'react';

class ExampleComponent extends Component {
  constructor(props) {
    super(props);
    this.state = {
      count: 0
    };
  }

  componentDidMount() {
    console.log('Component mounted');
  }

  componentDidUpdate(prevProps, prevState) {
    console.log('Component updated');
    if (prevState.count !== this.state.count) {
      console.log('Count updated');
    }
  }

  componentWillUnmount() {
    console.log('Component will unmount');
  }

  incrementCount() {
    this.setState(prevState => ({
      count: prevState.count + 1
    }));
  }

  render() {
    return (
      <div>
        <h2>Example Component</h2>
        <p>Count: {this.state.count}</p>
        <button onClick={() => this.incrementCount()}>Increment</button>
      </div>
    );
  }
}

export default ExampleComponent;
```

Note that in modern React development, functional components and React Hooks are preferred over class components and lifecycle methods. However, understanding the concept of lifecycle methods is still useful when working with existing codebases or certain advanced scenarios.


Sources: 

w3schools.com

openai.com

medium.com

webdevsimplified - youtube channel



