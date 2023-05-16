# Call Stack
The call stack is primarily used for function invocation (call). Since the call stack is single, function(s) execution, is done, one at a time, from top to bottom. It means the call stack is synchronous.

### What is call?
A "call" refers to the act of invoking or executing a function.

### How many ‘calls’ can happen at once?
In a single-threaded program, typically only one call can execute at a time. In a multi-threaded or concurrent program, multiple calls can execute simultaneously. Each thread can execute its own set of calls independently, allowing for parallelism and concurrent execution. 

### What does LIFO mean?
A call stack is a data structure that uses the Last In, First Out (LIFO) principle to temporarily store and manage function invocation (call). It means that the last function that gets pushed into the stack is the first to be pop out, when the function returns.

### Draw an example of a call stack and the functions that would need to be invoked to generate that call stack.
<img width="498" alt="Screenshot 2023-05-16 at 3 02 10 PM" src="https://github.com/ZG79/301_reading_notes/assets/101478282/b2e1c156-50b5-4ce4-b7f2-8ada96831722">

### What causes a Stack Overflow?

A stack overflow occurs when there is a recursive function (a function that calls itself) without an exit point. The browser (hosting environment) has a maximum stack call that it can accomodate before throwing a stack error.

# JS Error message
An error message often consists of an error type or name, along with a description of the error. 

- Reference error: when you try to use a variable that is not yet declared you get this type os errors.
- What is a ‘syntax error’? this occurs when you have something that cannot be parsed in terms of syntax, like when you try to parse an invalid object using JSON.parse.
- What is a ‘range error’? Try to manipulate an object with some kind of length and give it an invalid length and this kind of errors will show up.
- What is a ‘type error’? when the types (number, string and so on) you are trying to use or access are incompatible, like accessing a property in an undefined type of variable.
- What is a breakpoint? The breakpoint can also be achieved by putting a debugger statement in your code in the line you want to break.
- What does the word ‘debugger’ do in your code?  the debugger statement is used to pause the execution of code at a specific point so the developer can investigate the code. 
