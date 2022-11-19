# Readings: Redux Basic #

### What is Redux? ###
Redux is a predictable state container designed to help you write JavaScript apps that behave consistently across client, server, and native environments, and are easy to test. While it's mostly used as a state management tool with React, you can use it with any other JavaScript framework or library.

### Benefit of Redux ###
Redux allows you to manage your app’s state in a single place and keep changes in your app more predictable and traceable. It makes it easier to reason about changes occurring in your app. 

### What is Redux used for? ###
Redux is used to maintain and update data across your applications for multiple components to share, all while remaining independent of the components. Without Redux, you would have to make data dependent on the components and pass it through different components to where it’s needed.

for example: 

![1](https://blog.logrocket.com/wp-content/uploads/2020/10/passing-data-components-1.png)

In the example above, we only need some data in the parent and inner child components, but we’re forced to pass it to all the components (including the child component that doesn’t need it) to get it to where it’s needed.

With Redux, we can make state data independent of the components, and when needed, a component can access or update through the Redux store.

![2](https://blog.logrocket.com/wp-content/uploads/2020/10/passing-updating-independently-Redux-store.png)


### How Redux works ###
There is a central store that holds the entire state of the application. Each component can access the stored state without having to send down props from one component to another.

There are three core components in Redux — actions, store, and reducers.

### What are Redux actions? ###
Redux actions are events.

Actions are plain JavaScript objects that must have

- a `type` property to indicate the type of action to be carried out, and
- a `payload` object that contains the information that should be used to change the state.

Actions are created via an action creator, which in simple terms is a function that returns an action. And actions are executed using the store.dispatch() method which sends the action to the store.

Here’s an example of an action:

```
{ 
  type: "LOGIN",
  payload: {
    username: "foo",
    password: "bar"
  }
}
```

Here is an example of an action creator:

```
const setLoginStatus = (username, password) => {
  return {
    type: "LOGIN",
    payload: {
      username, // "foo"
      password // "bar" 
    }
  }
}
```

### What is Redux Store? ###
The store is a “container” (really a JavaScript object) that holds the application state, and the only way the state can change is through actions dispatched to the store. Redux allows individual components connect to the store and apply changes to it by dispatching actions.

*It is highly recommended to keep only one store in any Redux application. You can access the state stored, update the state, and register or unregister listeners via helper methods.*

### Why use Redux? ###
When using Redux with React, states will no longer need to be lifted up. This makes it easier for you to trace which action causes any change.

## SUMMARY ##
- Redux is a library for managing global application state

Redux is typically used with the React-Redux library for integrating Redux and React together

Redux Toolkit is the recommended way to write Redux logic

- Redux uses a "one-way data flow" app structure

State describes the condition of the app at a point in time, and UI renders based on that state

When something happens in the app:

    - The UI dispatches an action
    - The store runs the reducers, and the state is updated based on what occurred
    - The store notifies the UI that the state has changed
    
The UI re-renders based on the new state

- Redux uses several types of code

Actions are plain objects with a `type` field, and describe "what happened" in the app

Reducers are functions that calculate a new state value based on previous state + an action

A Redux store runs the root reducer whenever an action is dispatched


*[Source01](https://blog.logrocket.com/understanding-redux-tutorial-examples/#when-use-redux)*

*[Source02](https://egghead.io/courses/fundamentals-of-redux-course-from-dan-abramov-bd5cc867)*

*[Source03](https://redux.js.org/introduction/getting-started#basic-example)*

*[Source04](https://redux.js.org/tutorials/essentials/part-1-overview-concepts#redux-terms-and-concepts)*

