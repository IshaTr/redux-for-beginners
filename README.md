# redux-for-beginnners
This article is a brief overlook of redux principles and its application in a React application.Redux takes the concept of state mutation as a pure function that takes `previous state`, `action` and returns `new state`.

## state
The state tree or state is minimal representation of the data in your application. It's an object type.

## action
The action is minimal representation of the change to that data(state) in your app. It's an object type. It should always be provided with a `type` value that defines the action type that should be a string.

## princliples
1. Every data is stored in a single object that is called state or state tree.
2. The state tree is redundant i.e. you can't write anything to it or modify it. To change the state tree you must dispatch an action
