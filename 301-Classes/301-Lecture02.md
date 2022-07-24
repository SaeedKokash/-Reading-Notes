# React: Component Lifecycle Events #

Definition: React lets you define components as classes or functions. The methods that you are able to use on these are called lifecycle events. These methods can be called during the lifecycle of a component, and they allow you to update the UI and application states.

![](https://miro.medium.com/max/1400/0*0saPKFiTUk6W3FYp)

- *Mounting, Updating, and Unmounting are the three phases of the component lifecycle.*

## Based off the diagram, what happens first, the ‘render’ or the ‘componentDidMount’? ##

Render happens first.

## What is the very first thing to happen in the lifecycle of React? ##

**Mounting** is first thing that happens and it is when an instance of a component is being created and inserted into the DOM. The mounting happens after **Initialization** in which the component is going to start its journey by setting up the state (see below) and the props. This is usually done inside the constructor method 

![](https://cdn-media-1.freecodecamp.org/images/1*_drMYY_IEgboMS4RhvC-lQ.png)

## Put the following things in the order that they happen (componentDidMount, render, constructor, componentWillUnmount, React Updates) ##

1. constructor
2. render
3. componentDidMount
4. React Updates
5. componentWillUnmount

## What does componentDidMount do ##
It loads anything using a network request or initialize the DOM and it is invoked immediately after a component is mounted.

### *[Source 01](https://medium.com/@joshuablankenshipnola/react-component-lifecycle-events-cb77e670a093)* *[Source 02](https://www.freecodecamp.org/news/how-to-understand-a-components-lifecycle-methods-in-reactjs-e1a609840630/)* ###
<hr>
<hr>

# React State Vs Props #

![](https://assets-global.website-files.com/5dbb30f00775d4350591a4e5/612d0550e1af68ae6ba4df9f_Screen%20Shot%202021-08-30%20at%2012.20.18%20PM.png)

## What types of things can you pass in the props? ##
We can pass any type of data (arguments) into a react component, the data is passed from one component to another.

## What is the big difference between props and state? ##
The big difference is that props are handeled outside the component and states are handeled inside the component.

![](https://i.stack.imgur.com/G8Kj0.png)

## When do we re-render our application? ##

When changes are made to the application then the state changes and re-renders.


## What are some examples of things that we could store in state? ##

We stoe informations that could be changed or updated by the user for re-rendering like a form. 

### *[Source 01](https://www.youtube.com/watch?v=IYvD9oBCuJI)* *[Source 02](https://www.microverse.org/blog/how-to-create-components-with-props-and-validate-prop-types-in-react)* ###

<hr>
<hr>

## Useful Resources ##

- [React Docs - State and Lifecycle](https://reactjs.org/docs/state-and-lifecycle.html)
- [React Docs - handling events](https://reactjs.org/docs/handling-events.html)
- [React Tutorial through ‘Developer Tools’](https://reactjs.org/tutorial/tutorial.html)
- [React Bootstrap Documentation](https://react-bootstrap.github.io/)
- [Boootstrap Cheatsheet](https://getbootstrap.com/docs/5.0/examples/cheatsheet/)
- [Bootstrap Shuffle - a class “sandbox”](https://bootstrapshuffle.com/classes)
- [Netlify](https://www.netlify.com/l)

<hr>
<hr>

## Things I want to know more about
I want to understand more about the lifecycle because It's very confusing.
