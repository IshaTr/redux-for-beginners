# redux-for-beginnners
This article is a brief overlook of redux principles and its application in a React application.Redux takes the concept of state mutation as a pure function that takes `previous state`, `action` as arguments and returns `next state`. It should be kept in mind that the mutation, being a pure function, doesn't affect the `previous state` of the app but returns an altogether new state. Redux is fast since it works with `previous state` and calculates the `next state` values wrt `actions` taken. So, it can take the reference of the values from previous state that aren't affected that makes it fast.

## state
The state tree or state is minimal representation of the data in your application. It's an object type.

## action
The action is minimal representation of the change to that data(state) in your app. It's an object type. It should always be provided with a `type` value that defines the action type that should be a string.

## store
The store binds all the elements of the redux. It maintains state, let's you dispatch actions and eventually, perform mutations.

## reducer
These are the pure functions used to update the state tree by taking `previous state` and `action` as arguments and returning the `next state`.

## princliples
1. Every data is stored in a single object that is called state or state tree.
2. The state tree is redundant i.e. you can't write anything to it or modify it. To change the state tree you must dispatch an action
3. To do the state mutation, redux uses a pure function that takes `previous state` and `action` as arguments and returns the `next state`. This function is called `reducer`.
