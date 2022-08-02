# Functional Programming Concepts #

## What is functional programming? ##
Functional programming is a programming paradigm — a style of building the structure and elements of computer programs — that treats computation as the evaluation of mathematical functions and avoids changing-state and mutable data

## What is a pure function and how do we know if something is a pure function? ##
It returns the same result if given the same arguments (it is also referred as deterministic) and it does not cause any observable side effects.
pure functions do not have an internal state. Therefore, all operations performed in pure functions are not affected by their state. As a result, the same input parameters will give the same deterministic output regardless of how many times you run the function.

## What are the benefits of a pure function? ##
- It is easier to use and test
- A pure function works as an independent function that gives the same output for the same inputs.
- Pure functions are readable because of independent behavior. Moreover, they are straightforward to debug.
 
## What is immutability? ##
Unchanging over time or unable to be changed, its state cannot change after it’s created.

## What is Referential transparency? ##
A pure function that will always have the same output, given the same input.

`pure functions + immutable data = referential transparency`


### *[Source](https://medium.com/the-renaissance-developer/concepts-of-functional-programming-in-javascript-6bc84220d2aa)*  ###

<hr>
<hr>

# Node JS Tutorial for Beginners #6 - Modules and require() #

## What is a module? ##
its a bit of code that has a certain functionaliy which is written in a different place and is called back when needed


## What does the word ‘require’ do? ##
its a method we use to call a module in another module

## How do we bring another module into the file the we are working in? ##
we go to our module that we want to bring and we write `module.exports = (function name or whatever needed); , the we use the require method in the file we are working on and we put the path to the other module

## What do we have to do to make a module available? ##
we use module.exports method to let the model be able to be exported to other modules

### *[Source](https://www.youtube.com/watch?v=xHLd36QoS4k)*  ###

## Useful Resources ##


<hr>
<hr>

## Things I want to know more about
