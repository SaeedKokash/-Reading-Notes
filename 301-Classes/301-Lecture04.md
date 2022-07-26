# React Docs - Forms #

## What is a ‘Controlled Component’? ##
An input form element whose value is controlled by React, we can explain this by saying that the React component that renders an element also conrols what happens within the state that the user input declares.

## Should we wait to store the users responses from the form into state when they submit the form OR should we update the state with their responses as soon as they enter them? Why. ##
we should wait to store the users responses from the form into state,because In React, every state update causes the component being updated to re-render. Because re-rendering is an expensive operation, making state updates synchronously can cause serious performance issues, for example, increasing load times or causing your application to crash. By batching state updates, React avoids unnecessary re-renders, boosting performance overall. 

## How do we target what the user is entering if we have an event handler on an input field? ##
we should create an event handler function which setState the value thats in the initial constructor (required input property) by writing ` event.target.value ` as in this example:
``` 
 handleChange(event) {
    this.setState({value: event.target.value});
  }
  ```

### *[Source 01](https://reactjs.org/docs/forms.html)* *[Source 02](https://blog.logrocket.com/why-react-doesnt-update-state-immediately/)* ###

<hr>
<hr>

# The Conditional (Ternary) Operator Explained #

## Why would we use a ternary operator? ##
to make an if statement shorter into a one line of code

## Rewrite the following statement using a ternary statement:
``` 
if(x===y){
  console.log(true);
} else {
  console.log(false);
}
  ```
##

Answer:

```
(x===y)? console.log(true) : console.log(false) ;
```

### *[Source 01](https://codeburst.io/javascript-the-conditional-ternary-operator-explained-cac7218beeff)* *[Source 02]()* ###

<hr>
<hr>

## Useful Resources ##

- [React Bootstrap - Forms](https://react-bootstrap.github.io/forms/overview/)
- [React Docs - conditional rendering](https://reactjs.org/docs/conditional-rendering.htmll)

<hr>
<hr>

## Things I want to know more about
forms in React and how to apply them and get data from users by them.
