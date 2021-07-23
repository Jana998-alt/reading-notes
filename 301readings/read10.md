# Read10: In memory storage


## Understanding the JavaScript Call Stack

- What is a ‘call’?

a call stack is a data structure that uses the Last In, First Out (LIFO) principle to temporarily store and manage function invocation (call).

- How many ‘calls’ can happen at once?

only one

- What does LIFO mean?

at the last function that gets pushed into the stack is the first to be pop out, when the function returns.


What causes a Stack Overflow?

when there is a recursive function (a function that calls itself) without an exit point. 


## JavaScript error messages

- What is a ‘refrence error’?

it is when a code attempts to reference a non-existing variable.for example, when  you try to use a variable that is not yet declare. it is an

- What is a ‘syntax error’? 

An exception caused by the incorrect use of a pre-defined syntax. for example, when you have something that cannot be parsed in terms of syntax.

- What is a ‘range error’?

it is thrown when trying to pass a value as an argument to a function that does not allow a range that includes the value.

- t is a ‘tyep error’?

thrown when an operation could not be performed

- What is a breakpoint?

At each breakpoint, JavaScript will stop executing, and let you examine JavaScript values.

- What does the word ‘debugger’ do in your code?

stops the execution of JavaScript, and calls (if available) the debugging function.
