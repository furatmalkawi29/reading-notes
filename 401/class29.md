# Routing

## Review, Research, and Discussion

* Do child components have direct access to props/state from the parent?
  *  have access to state from the parent (this.state) when in a class, and have access to props as a functional component.
  
* When a component “wraps” another component, how does the child component’s output get rendered?
  * when there is an update to state.

* Can a component, such as `<Content />`, which is a child also be used as a standalone component elsewhere in the application?
 * no ,standalone components have no parents to get props from or children to pass props to.

* What trick can a parent use to share all props with it’s children
 * pass all the props with the spread operator: `<ChildComponent {...props}>`


## Vocabulary Terms

### props.children :
  * we use `props.children` on components that represent ‘generic boxes’ and that ‘don’t know their children ahead of time’.
### composition :
  * omposition give you all the flexibility you need to customize a component’s look and behavior in an explicit and safe way.



## Routing

<img src ="https://i.morioh.com/c794445099.png">

* React Router is a collection of navigational components that compose declaratively with your application. 
* React Router v4 is a pure React rewrite of the popular React package.
* To build it you need to install `react-router`, `react-router-dom`, and `react-router-native`.
* Determine which type of router to use, `<BrowserRouter>` and `<HashRouter>`.
* Render router component in the App render function.
* React Router Component: - `<Route path=''/> <Switch> .`