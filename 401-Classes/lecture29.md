# Readings: Redux Advance #

### What are Redux and Redux-Toolkit? ###
Redux is an open-source JavaScript library for managing application state. It is most commonly used with libraries such as React or Angular for building user interfaces.

Redux Toolkit was introduced with a purpose to be the standard way to write redux logic. It is said to be an opinionated, batteries-included toolset for efficient Redux development. By using this, you can write all the code you need for your Redux store in a single file, including actions and reducers. Using this you can make your code more readable. Redux toolkit includes all the tools, you want for a Redux application. At the end of the day all you have is less code and faster setups of Redux in every scenario.

### Why You Should Use Redux Toolkit ###
Redux Toolkit makes it easier to write good Redux applications and speeds up development, by baking in our recommended best practices, providing good default behaviors, catching mistakes, and allowing you to write simpler code. Redux Toolkit is beneficial to all Redux users regardless of skill level or experience. It can be added at the start of a new project, or used as part of an incremental migration in an existing project.

### Redux Toolkit includes ###

- `configureStore()`: wraps createStore to provide simplified configuration options and good defaults. It can automatically combine your slice reducers, adds whatever Redux middleware you supply, includes redux-thunk by default, and enables use of the Redux DevTools Extension.
- `createReducer()`: that lets you supply a lookup table of action types to case reducer functions, rather than writing switch statements. In addition, it automatically uses the immer library to let you write simpler immutable updates with normal mutative code, like `state.todos[3].completed = true`.
- `createAction()`: generates an action creator function for the given action type string. The function itself has `toString()` defined, so that it can be used in place of the type constant.
- `createSlice()`: accepts an object of reducer functions, a slice name, and an initial state value, and automatically generates a slice reducer with corresponding action creators and action types.
- `createAsyncThunk`: accepts an action type string and a function that returns a promise, and generates a thunk that dispatches `pending/fulfilled/rejected` action types based on that promise
- `createEntityAdapter`: generates a set of reusable reducers and selectors to manage normalized data in the store
- The `createSelector` utility from the Reselect library, re-exported for ease of use.

### What is createSlice in Redux Toolkit? ###
createSlice is a higher order function that accepts an initial state, an object full of reducer functions and a slice name. It automatically generates action creators and action types that correspond to the reducers and state.

In Redux-Toolkit, the createSlice method helps us create a slice of the redux-store. This function aims to reduce the boilerplate required to add data to redux in the canonical way. Internally, it uses createAction and createReducer.

**Step 1: Implement createSilce method and export actions and reducer.**

```
import { createSlice } from '@reduxjs/toolkit';
const locationSlice = createSlice({
    name: "location",
    initialState: {
        location: ['Bangalore', 'Hyderabad', 'Delhi'],
    },
    reducers: {
        save: (state, param) => {
            const { payload } = param;
            state.location = [...state.location, payload];
        },
    }
});
const { actions, reducer } = locationSlice
export const { save } = actions;
export default reducer;
```

**Step 2: Dispatch action by making use of react hooks in functional component.**

```
import React, { useState } from "react";
import { save } from "./locationSlice";
import { useDispatch, useSelector } from "react-redux";
import { Box, TextField, Button } from "@material-ui/core";

export default function App() {
    const [locationName, setLocationName] = useState('');
    const dispatch = useDispatch();
    const { location } = useSelector(state=>state)
    const handleData = (e) => {
        setLocationName(e.target.value);
    }
    const handleSave = () => {
        const ifPrestent = location.includes(locationName);
        if(locationName !== undefined && !ifPrestent) {
            dispatch(save(locationName));
            setLocationName('')
        } else {
            setLocationName('')
        }
    }
    return (
        <Box>
            <Box>
                <TextField 
                    onChange={handleData} 
                    value={locationName} 
                    label="Enter location name"
                />
                <Button
                    style={{margin: '10px'}}
                    variant="contained"
                    color="primary"
                    onClick={handleSave}
                >
                    add
                </Button>
            </Box>
            <Box>
                <h3> List of locations </h3>
            </Box>
            <Box>
                 {location.map((item) => <li>{item}</li>) }
            </Box>
        </Box>
    );
}
```

**Step 3: Configure the store**

```
import React from "react";
import ReactDOM from "react-dom";
import App from "./App";
import { configureStore } from "@reduxjs/toolkit";
import { Provider } from "react-redux";
import rootReducer from "./locationSlice";
const store = configureStore({
    reducer: rootReducer
});
ReactDOM.render(
    <Provider store={store}>
        <App />
    </Provider>,
    document.getElementById('root')
);
```

*[Source01](https://medium.com/geekculture/understanding-createslice-in-redux-toolkit-reactjs-eca8d20f45d7)*

*[Source02](https://redux.js.org/redux-toolkit/overview)*

*[Source03](https://redux-toolkit.js.org/api/createslice)*
