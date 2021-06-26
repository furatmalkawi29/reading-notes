# Hooks API

# Hooks API

## Review, Research, and Discussion

* Why do we not need more .html pages in a multi-page React app?
  * react-router-dom allows to register multiple URLs and their corresponding components in one of the parent nodes of the DOM tree. Then, depending on the URL entered certain nodes are rendered to the DOM and others are not. Single-page-applications still need to get data for different components as components render.
  
* If we wanted a component to show up on every page, where would we put it and why?
  * Inside the <BrowserRouter />, outside a <Route /> -> this will allow it to render on all pages regardless of a specified route.

* What does props.children contain?
 * Props.children is a special prop, automatically passed to every component that can be used to render the content included between the opening and closing tags when invoking a component. 




## Vocabulary Terms

### Composition :
  * the act of combining parts or elements to form a whole.
### Children / Child Components :
  * components that are nested within a parent React component.
### Hash Routing :
  *  Using the anchor part of the URL to simulate different content.
### Link Routing :


A Hook is a special function that lets you `hook into` React features. For example, useState is a Hook that lets you add React state to function components. We’ll learn other Hooks later.


Functions can’t have local React state inside them. You can’t extract behavior like `watch window size and update the state` or “animate a value over time” from a class component without restructuring your code or introducing an abstraction like Observables. Both approaches hurt the simplicity that we like about React.


Hooks solve exactly that problem. Hooks let you use React features (like state) from a function — by doing a single function call. React provides a few built-in Hooks exposing the “building blocks” of React: state, lifecycle, and context.

 Since Hooks are regular JavaScript functions, you can combine built-in Hooks provided by React into your own `custom Hooks`. This lets you turn complex problems into one-liners and share them across your application .

  Hooks are fully encapsulated — each time you call a Hook, it gets isolated local state within the currently executing component

 They’re not a way to share state — but a way to share stateful logic