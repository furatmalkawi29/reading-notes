
# Context API

## Review, Research, and Discussion


* Describe use cases for useMemo() and useReducer()
  * The useMemo() hook is often used to optimize when doing expensive calculations while rendering. userReducer() can be used for managing state objects that contain multiple sub-values. UseReducer is an alternative to useState, usually preferable when you have complex state logic that involves multiple sub-values or when the next state depends on the previous one. 

  
* Why do custom hooks need the use prefix?
  * Should start with use so that you can tell at a glance that the rules of Hooks apply to it.

* What do custom hooks usually do?
 * Allow you to extract and share logic in a way that was not possible with class components. 

* Using any list of custom hooks, research and name one that you think will be useful in your applications
 * The useDocumentTitle custom hook seems like it could be helpful in updating the page title/browser tab..

* Describe how a hook that fetches API data might work
  * useEffect can make a network requeset on component render, when the fetch resolves, it can set the response from the server to the local state using the setState function, which will cause the component to render to update the DOM with the data.



## Vocabulary Terms

### reducer :
  * Will always return only one value, that value can be a number, string, an array, or an object. Great for applying a bit of logic to a group of values and ending up with another single result. Reducers will not mutate your initial value, rather they return something else.



## Context API


* Context provides a way to pass data through the component tree without having to pass props down manually at every level.
* It share global data between all components of the tree.
* Before You Use Context Context is primarily used when some data needs to be accessible by many components at different nesting levels.
* If you only want to avoid passing some props through many levels, component composition is often a simpler solution than context.