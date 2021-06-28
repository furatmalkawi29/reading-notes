# Custom Hooks

## Review, Research, and Discussion

* What does a component’s lifecycle refer to?
  *  Lifecycle of a component is series of methods that are invoked in different stages of the component's existence. Lifecycle methods give ways to interact with component logic before/during/after being used in the DOM.
  
* Why do you sometimes need to “wrap” functions in useCallback when called from within useEffect
  * useCallback() is often used in conjunction with useEffect() because it allows you to prevent the re-creation of a function.

* Why are functional components preferred over class components?
 * Props.children is a special prop, automatically passed to every component that can be used to render the content included between the opening and closing tags when invoking a component. 

* What is wrong with the following code?
 * Functional components are much easier to read and test, they have less code, easier to separate container and presentational components.




## Vocabulary Terms

### state hook :
  * useState(), similar to this.setState() in a class except it doesn't merge the old and new state together. The only argument to useState() is the initial state. Allows us to add a state powered variable to our application.
### effect hook :
  * useEffect(), adds the ability to perform side effects (data fetching, subscriptions, or manually changing the DOM from React components) from a function component. Serves the same purpose as componentDidMount, componentDidUpdate, and componentWillUnmount in React classes but unified into a single API. Allows us to define properties that will trigger or not trigger React API features.
### reducer hook :
  *  alternative to useState(), accepts a reducer of type (state, action) => newState, and returns the current state paired with a dispatch method.




# Custom Hooks

It is a JS function his name starts with `use` and that may call other Hooks.

---------------------

A custom Hook doesn't need to have a specific signature.

 We can decide if  it takes as arguments.
 it's look like any Js function

---------------------

useReducer is usually preferable to useState when you have complex state logic that involves multiple sub-values or when the next state depends on the previous one.

 useReducer also lets you optimize performance for components that trigger deep updates because you can pass dispatch down instead of callbacks.


<img src ="https://diarybydhanushka.dev/wp-content/uploads/2020/02/custom-hooks.png">

* Hooks let us organize the logic inside a component into reusable isolated units
* Hooks apply the React philosophy (explicit data flow and composition) inside a component, rather than just between the components
* Hooks don’t introduce unnecessary nesting into your component tree. They also don’t suffer from the drawbacks of mixins
* Hooks let you always use functions instead of having to constantly switch between functions, classes, higher-order components, and render props
* Hooks let you use React features (like state) from a function — by doing a single function call. React provides a few built-in Hooks exposing the “building blocks” of React: state, lifecycle, and context.
* Built-in React Hooks like useState and useEffect serve as the basic building blocks
* The only argument passed to the useState() Hook is the initial state, if you want to store two different values in state, you call useState() twice
useState() returns a pair of values: the current state and a function that updates it
* Hooks are fully encapsulated — each time you call a Hook, it gets isolated local state within the currently executing component
* They’re not a way to share state — but a way to share stateful logic
* Each Hook may contain some local state and side effects. You can pass data between multiple Hooks just like you normally do between functions. They can take arguments and return values because they are JavaScript functions.
* Unlike render props or higher-order components, Hooks don’t create a “false hierarchy” in your render tree. They’re more like a flat list of “memory cells” attached to a component. No extra layers.


