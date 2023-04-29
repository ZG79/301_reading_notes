### What is the single responsibility principle and how does it apply to components?
a component should ideally only do one thing. This principle helps to make code more maintainable, testable, and reusable.
### What does it mean to build a ‘static’ version of your application?
We can build a static versiojn of the website first to put all the content, structure, and layout are predefined and fixed. and add interactivity later.
### Once you have a static application, what do you need to add?
Add functionality to make it dynamic and interactive. Such as adding back-end functionality, data management, and event handling to the application.
### What are the three questions you can ask to determine if something is state?
- Does it change over time?
State will change.
- Is it passed in from a parent via props?
If something is passed down from a parent component via props, it is not state. Props represent data that is passed between components, but is not managed within a component.
- Is it triggering to rerender?
-It should be yes.
### How can you identify where state needs to live?
- Often, we can put the state directly into their common parent.
- we can also put the state into some component above their common parent.
- If we can’t find a component where it makes sense to own the state, create a new component solely for holding the state and add it somewhere in the hierarchy above the common parent component. 
- 
- And to remember: React uses one-way data flow, passing data down the component hierarchy from parent to child component. 

## Higher order functions

### What is a “higher-order function”?
Functions that operate on other functions, either by taking them as arguments or by returning them, are called higher-order functions. 

### Explore the greaterThan function as defined in the reading. In your own words, what is line 2 of this function doing?
```js
function greaterThan(n) {
  return m => m > n;
}
let greaterThan10 = greaterThan(10);
console.log(greaterThan10(11));
// → true
```
In this function line two is erturning boolean value if m is greater than the parameter n. 

### Explain how either map or reduce operates, with regards to higher-order functions.
map: The map method transforms an array by applying a function to all of its elements and building a new array from the returned values. The new array will have the same length as the input array, but its content will have been mapped to a new form by the function.

reduce:  It builds a value by repeatedly taking a single element from the array and combining it with the current value. When summing numbers, you’d start with the number zero and, for each element, add that to the sum.

The function passed to reduce is called a "reducer function", and the parameters to reduce are, apart from the array, a combining function and a start value. 
