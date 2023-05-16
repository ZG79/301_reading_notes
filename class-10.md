# Call Stack
The call stack is primarily used for function invocation (call). Since the call stack is single, function(s) execution, is done, one at a time, from top to bottom. It means the call stack is synchronous.

### What is call?
A "call" refers to the act of invoking or executing a function.

### How many ‘calls’ can happen at once?
In a single-threaded program, typically only one call can execute at a time. In a multi-threaded or concurrent program, multiple calls can execute simultaneously. Each thread can execute its own set of calls independently, allowing for parallelism and concurrent execution. 

### What does LIFO mean?
A call stack is a data structure that uses the Last In, First Out (LIFO) principle to temporarily store and manage function invocation (call). It means that the last function that gets pushed into the stack is the first to be pop out, when the function returns.

### 
