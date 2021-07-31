# Error Handling & Debugging

Understanding how to deal with errors and debug is crucial when writing code. It's almost guaranteed that your code won't be perfect on the first go round, so it's important to know how to interpret errors to make the debugging process easier.

### The Stack

It's imperative to know how the JavaScript interpreter works. The interpreter is incapable of reading all of your code simultaneosly. It can only process one line at a time. Whenever the interpreter comes across a line of code that references data from another function, it stacks the new function on top of the current task. Say you declared a variable with a function like so: `const users = getCurrentUsers();`. Here, the function `getCurrentUsers()` would be added to the stack on top of the variable `users`. Once JavaScript is able to interpret the result of `getCurrentUsers()`, it'll use that to process what `users` actually stores.

### Error Objects

Error objects can aid in finding where mistakes lay in your code. An error object consists of a name denoting the type of error, a message that gives more context of the issue, and a file number & line number to let you know where the error is occurring. There are seven types of built-in error objects in JavaScript. Here's a list:

- **Error** - Generic error. Other errors are based off of this one

- **SyntaxError** - Improper syntax

- **ReferenceError** - Attempted to reference a variable that wasn't declared or within scope

- **TypeError** - Unexpected data type that can't be coerced

- **RangeError** - Numbers aren't in acceptable range

- **URIError** - methods like `encodeURI()` and `decodeURI()` were used incorrectly

- **EvalError** - `eval()` function was used incorrectly
