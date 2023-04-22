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
###What is the spread operator?
The JavaScript spread operator (...) allows us to quickly copy all or part of an existing array or object into another array or object.
### List 4 things that the spread operator can do.
- Concatenate arrays: The spread operator can be used to combine multiple arrays into a single array. For example: [...array1, ...array2, ...array3].

- Copy arrays: The spread operator can be used to create a new array that contains all the elements of an existing array. For example: [...originalArray].

- Pass arguments to a function: The spread operator can be used to pass the elements of an array as individual arguments to a function. For example: myFunction(...myArray).

- Create a new object: The spread operator can be used to create a new object that includes all the properties of an existing object, and optionally add or overwrite properties. For example: { ...oldObject, newProperty: 'value' }.
### Give an example of using the spread operator to combine two arrays.
```js 
const myVehicle = {
  brand: 'Ford',
  model: 'Mustang',
  color: 'red'
}

const updateMyVehicle = {
  type: 'car',
  year: 2021, 
  color: 'yellow'
}

const myUpdatedVehicle = {...myVehicle, ...updateMyVehicle}
```
### Give an example of using the spread operator to add a new item to an array.
```js
const myArray = [1, 2, 3];

// Using the spread operator to add a new item to the end of the array
const newArray = [...myArray, 4];

console.log(newArray); // [1, 2, 3, 4]
```

### Give an example of using the spread operator to combine two objects into one
```js
const obj1 = { foo: "bar", x: 42 };
const obj2 = { foo: "baz", y: 13 };

const clonedObj = { ...obj1 };
// { foo: "bar", x: 42 }

const mergedObj = { ...obj1, ...obj2 };
// { foo: "baz", x: 42, y: 13 }
```

###  what is the first step that the developer does to pass functions between components?
define the function in the parent component and then pass it down as a prop to the child component.

### In your own words, what does the increment function do?
increment function next to the state changes the object value if it's selected. Increment function in the constructor, calls the function that was written to change the state.
### How can you pass a method from a parent component into a child component?
In React, you can pass a method from a parent component into a child component as a prop. 

### How does the child component invoke a method that was passed to it from a parent component?

In React, when a method is passed from a parent component to a child component as a prop, the child component can invoke the method by calling the function passed to it as a prop.
