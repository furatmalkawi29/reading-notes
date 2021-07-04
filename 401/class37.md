# Redux - Combined Reducers

## Review, Research, and Discussion


* Why choose Redux instead of the Context API for global state?

     * In a large scale application, Redux is a better way to control state.

* What is the purpose of a reducer?

   *  Process of giving someone the ability to access a resource.

* What does an action contain?

  * Object literals that tell the reducer what is being done to the app, and any data required for the update..
* Why do we need to copy the state in a reducer?
 * Reducers are not allowed to modify the existing state, instead they must make immutable updates by copying the existing state and making changes to the copied values.


## Vocabulary Terms

### immutable state :
  * State cannot be modified, reducers must make copies of existing state to make updates.
### time travel in redux :
  * Redux DevTools records dispatched actions and the state of the Redux store at every point in time, which makes it possible to inspect the state and travel back in time to a previous application state without reloading the page or re-starting the app.

### action creator :
  * Instead of creating action objects inline in the places where you dispatch actions, can create functions generating them. You might write an action creator into a separate file, and import it into your component. 

### reducer :
  * Functions that take current state and an action as arguments, and return a new state result, (state, action) => newState.

### dispatch :
 * A store holds the whole state tree of the application, the only way to change the state inside it is to dispatch an action on it.

## Redux - Combined Reducers

<img src ="https://i.ytimg.com/vi/IfjnLtxOyrU/maxresdefault.jpg">

* combineReducers: helper function turns an object whose values are different reducing functions into a single reducing function you can pass to createStore .

* The resulting reducer calls every child reducer, and gathers their results into a single state object.
* combineReducers will combine all the reducers passed to it into a single reducing function
