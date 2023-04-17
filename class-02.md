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
