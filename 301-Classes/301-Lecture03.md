# React Docs - lists and keys #

## What does .map() return? ##

.map() returns an entirely new array with transformed elements and the same amount of data.

## If I want to loop through an array and display each value in JSX, how do I do that in React? ##
we use .map() function to loop through the array and we return the result that we want using curly braces {}

## Each list item needs a unique *key*. ##

## What is the purpose of a key? ##
Keys help React identify which items have changed, are added, or are removed. Keys should be given to the elements inside the array to give the elements a stable identity

**Note**:It is not recommended using indexes for keys if the order of items may change. This can negatively impact performance and may cause issues with component state.

### *[Source](https://reactjs.org/docs/lists-and-keys.html)* ###

<hr>
<hr>

# The Spread Operator #

## What is the spread operator? ##
In JavaScript, spread syntax refers to the use of an ellipsis of three dots (…) to expand an iterable object into the list of arguments.

## Give an example of using the spread operator to combine two arrays. ##

``` 
  let fruits = ["apples", "bananas"];
  let vegetables = ["corn", "carrots"];
  let produce = [...fruits, ...vegetables];
  
  Output:
  ["apples","bananas","corn","carrots"]
  ```

## Give an example of using the spread operator to add a new item to an array. ##

```
let numberStore = [0, 1, 2];
let newNumber = 12;
let numberStore = [...numberStore, newNumber];

Output:
[0, 1, 2, 12]
```

## Give an example of using the spread operator to combine two objects into one. ##

```
let person = {
    firstName: 'John',
    lastName: 'Doe',
};


let job = {
    jobTitle: 'JavaScript Developer',
    location: 'USA'
};

let employee = {
    ...person,
    ...job
};


Output:
{
    firstName: 'John',
    lastName: 'Doe',
    jobTitle: 'JavaScript Developer',
    location: 'USA'
}
```

### *[Source 01](https://medium.com/coding-at-dawn/how-to-use-the-spread-operator-in-javascript-b9e4a8b06fab)* *[Source 02](https://www.javascripttutorial.net/es6/javascript-spread/ )* ###

<hr>
<hr>

# How to Pass Functions Between Components #

## what is the first step that the developer does to pass functions between components? ##
He created a function and passed state into it to so he can create a setState and make it updatable.

## In your own words, what does the increment function do? ##
It checks if the name that is inserted equals the name thats already in the constructor; then the count will increase by one and it will be updated.

## How can you pass a method from a parent component into a child component? ##
You can call the method back on any element that you want in the child component.

## How does the child component invoke a method that was passed to it from a parent component? ##
You decide that by the method that you want, in the video it was by clicking a button.

### *[Source ](https://www.youtube.com/watch?v=c05OL7XbwXU)* ###

<hr>
<hr>

## Useful Resources ##

- [React Tutorial through ‘Declaring a Winner’](https://reactjs.org/tutorial/tutorial.html)
- [React Docs - Lifting State Up](https://reactjs.org/tutorial/tutorial.html)

<hr>
<hr>

## Things I want to know more about
I want to learn more about spread operator and I want to understand how to pass functions between components more because its still not clear.
