# Passing Functions as Props
In React, we can pass functions as props to child components to enable communication between components. This allows us to create reusable components that can work with different data and behaviors, making our code more modular and flexible.
```js
import React from "react";
import ChildComponent from "./ChildComponent";

class ParentComponent extends React.Component {
  handleClick = () => {
    console.log("Button clicked");
  };

  render() {
    return (
      <div>
        <ChildComponent onClick={this.handleClick} />
      </div>
    );
  }
}

export default ParentComponent;
```
### What does .map() return?
Map return new array of modified indexes. The new array will have the same length as the original array.
### If I want to loop through an array and display each value in JSX, how do I do that in React?
Using map method.
### Each list item needs a unique KEY.
### What is the purpose of a key?
The key prop is a special attribute that is used by React to keep track of each element in the array and optimize updates. Keys help React identify which items have changed, are added, or are removed. Keys should be given to the elements inside the array to give the elements a stable identity:
```js
const numbers = [1, 2, 3, 4, 5];
const listItems = numbers.map((number) =>
  <li key={number.toString()}>
    {number}
  </li>
);
```
