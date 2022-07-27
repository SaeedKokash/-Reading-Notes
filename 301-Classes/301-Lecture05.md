# React Docs - Thinking in React #

## What is the single responsibility principle and how does it apply to components? ##
It means that a component or a function or anything should do only one thing, if it starts to get complicated and mixed up with other stuff and growing, it should be distorted or decomposed into smaller parts that are connected to it (subcomponents,functions...)
![](https://media-exp2.licdn.com/dms/image/C4D12AQHa5pFybjJk2w/article-inline_image-shrink_1500_2232/0/1607887277091?e=1663804800&v=beta&t=do_GnonpCmcU53CJgmbjqgAKj0I-x84lFzHZz2iaEKs)

## What does it mean to build a ‘static’ version of your application? ##
It means to build an application without the ability to interact with it, we dont use state, we only use props. It will all be built on the same component and it could be written top-down or visa versa depending on the project, the components will only have render() methods

## Once you have a static application, what do you need to add? ##
We need to add state in order to make it interactivable, we need to identify where which components mutates or owns states, the purpose is that we need to be *DRY -> Don't Repeat Yourself* 

## What are the three questions you can ask to determine if something is state? ##
1. Is it passed in from a parent via props? If so, it probably isn’t state.
2. Does it remain unchanged over time? If so, it probably isn’t state.
3. Can you compute it based on any other state or props in your component? If so, it isn’t state.

## How can you identify where state needs to live? ##
1. Identify every component that renders something based on that state.
2. Find a common owner component (a single component above all the components that need the state in the hierarchy).
3. Either the common owner or another component higher up in the hierarchy should own the state.
4. If you can’t find a component where it makes sense to own the state, create a new component solely for holding the state and add it somewhere in the hierarchy above the common owner component.

### *[Source 01](https://reactjs.org/docs/thinking-in-react.html)* ###

<hr>
<hr>

# Higher-Order Functions #

## What is a “higher-order function”?##
Functions that operate on other functions, either by taking them as arguments or by returning them

## Explore the greaterThan function as defined in the reading. In your own words, what is line 2 of this function doing? ##
```
1.      function greaterThan(n) {
2.      return m => m > n;
3.      }
4.      let greaterThan10 = greaterThan(10);
5.      console.log(greaterThan10(11));
6.      // → true
```

line 2 -> is returning a mathematical logic of comparing m and n which returns true or false.

## Explain how either map or reduce operates, with regards to higher-order functions. ##
Map operates on a list of values in order to produce a new list of values, by applying the same computation to each value. Reduce operates on a list of values to collapse or combine those values into a single value


### *[Source 01](https://eloquentjavascript.net/05_higher_order.html#h_xxCc98lOBK)* 

<hr>
<hr>

## Useful Resources ##


<hr>
<hr>

## Things I want to know more about
I want to learn more about reduce.
