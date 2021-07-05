# Redux - Asynchronous Actions

## Review, Research, and Discussion


* How granular should your reducers be?
     *  It is difficult to manage states that are deeply nested, so more reducers is better than only a few. Redux gives us combineReducers to let us define more precisely what our initial state will look like.

* Pro or Con – multiple reducers can “fire” when a commonly named action is dispatched
   *  Not sure, I would guess con as it gets messy and actions need to get filtered through.

* Name a strategy for preventing the above?
  * Using Redux middleware thunk, allows for evaluating the actions.



## Vocabulary Terms

### store :
  * Holds the whole state tree of the application, only way to change the state inside is to dispatch an action on it.
### combined reducers : 
  * Helper function turns an object whose values are different reducing functions into a single reducing function you can pass to createStore.

## Redux - Asynchronous Actions

<img src ="https://i.morioh.com/74428a9fdb.png">

* Redux Thunk Middleware:
  * Redux Thunk is a middleware that lets you call action creators that return a function instead of an action object.
  * That function receives the store's dispatch method, which is then used to dispatch regular synchronous actions inside the function's body once the asynchronous operations have been completed.
  * allows for delayed actions, including working with promises. One of the main use cases for this middleware is for handling actions that might not be synchronous.

### Async Data Fetching
Redux store is oblivious to async logic, it only synchronously dispatches actions and updates the state by calling the reducer functions, then notified the UI about changes.

Redux Thunk is middleware that allows you to return functions, rather than just actions, within Redux. This allows for delayed actions, including working with promises.

Redux Thunk allows us to dispatch those actions asynchronously and resolve each promise that gets returned.
