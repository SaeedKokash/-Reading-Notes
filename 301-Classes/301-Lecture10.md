# Understanding the JavaScript Call Stack #

## What is a ‘call’? ##
when you invoke a function

## How many ‘calls’ can happen at once? ##
only 1 call can happen in an asynchronous programming

## What does LIFO mean? ##
LIFO = Last In First Out.
 
## Draw an example of a call stack and the functions that would need to be invoked to generate that call stack. ##
```
function firstFunction(){
  throw new Error('Stack Trace Error');
}

function secondFunction(){
  firstFunction();
}

function thirdFunction(){
  secondFunction();
}

thirdFunction();
```

## What causes a Stack Overflow? ##
The most-common cause of stack overflow is excessively deep or infinite recursion, in which a function calls itself so many times that the space needed to store the variables and information associated with each call is more than can fit on the stack.
`pure functions + immutable data = referential transparency`


### *[Source](https://codeburst.io/javascript-error-messages-debugging-d23f84f0ae7c)*  ###

<hr>
<hr>

# JavaScript error messages #

## What is a ‘reference error’? ##
The ReferenceError object represents an error when a variable that doesn't exist (or hasn't yet been initialized) in the current scope is referenced.

## What is a ‘syntax error’? ##
is an error in the syntax of a coding or programming language

## What is a ‘range error’? ##
A RangeError is thrown when trying to pass a value as an argument to a function that does not allow a range that includes the value. This can be encountered when: passing a value that is not one of the allowed string values to String

## What is a ‘tyep error’? ##
The TypeError object represents an error when an operation could not be performed, typically (but not exclusively) when a value is not of the expected type. A TypeError may be thrown when: an operand or argument passed to a function is incompatible with the type expected by that operator or function; or.

## What is a breakpoint? ##
In the debugger window, you can set breakpoints in the JavaScript code. At each breakpoint, JavaScript will stop executing, and let you examine JavaScript values. After examining values, you can resume the execution of code (typically with a play button).

## What does the word ‘debugger’ do in your code? ##
A debugger is a software tool that can help the software development process by identifying coding errors at various stages of the operating system or application development. Some debuggers will analyze a test run to see what lines of code were not executed.

### *[Source](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Errors)  ###



## Useful Resources ##
- [JavaScript errors reference on MDN](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Errors)

<hr>
<hr>

## Things I want to know more about
