# Component Composition
## Review, Research, and Discussion

* Can a parent component access the state of a child component?
  * Assign Refs for the child component in the parent component, then using Refs can access the child's state.
  
* What can be passed along in a prop variable?
  * variables, objects functions that needs to be passed. 

* How can a child component “know” the state of another component?
 * pass the component's state to it's child components as props.



## Vocabulary Terms

### component props :
  * a keyword in React stands for `properties`, can be any information that needs to be passed to another component.

### component state :
  * The state is an instance of React Component Class can be defined as an object of a set of observable properties that control the behavior of the component.


### application state :
  * is interface between data and the representation of this data with UI elements on the front-end. State is able to keep the data of different components in sync because each state update will rerender all relevant components.




## react basics recap

 * The Component Lifecycle : it details the life of a component, components are born, do some things , and then they die.

* A component can only be in one stage at a time. It starts with mounting and moves onto updating. It stays updating perpetually until it gets removed from the virtual DOM. Then it goes into the unmounting phase and gets removed from the DOM.
* Higher-Order Components: is a function that takes a component and returns a new component.

* Each component in React has a lifecycle which you can monitor and manipulate during its three main phases. The three phases are: Mounting, Updating, and Unmounting.
* You can think of React lifecycle methods as the series of events that happen from the birth of a React component to its death.
* `setState()` in only these React lifecycle methods: `componentDidMount` , `componentDidUpdate` and `componentWillReceiveProps` .


## Components and Props

<img src ="https://www.gatsbyjs.com/static/c058cc46416d6b9d5d27e571c885c936/6569d/component-with-props.png">


* Components let you split the UI into independent, reusable pieces, and think about each piece in isolation
* Conceptually, components are like JavaScript functions. They accept arbitrary inputs (called “props”) and return React elements describing what should appear on the screen.
* Components can refer to other components in their output
* Whether you declare a component as a function or a class, it must never modify its own props
* All React components must act like pure functions (do not attempt to change their inputs and always return the same result for the same inputs) with respect to their props

## props.children
* we use `props.children` on components that represent ‘generic boxes’ and that ‘don’t know their children ahead of time’.

## Component Composition

<img src ="https://res.cloudinary.com/practicaldev/image/fetch/s--yV_Dmfcz--/c_imagga_scale,f_auto,fl_progressive,h_500,q_auto,w_1000/https://cl.ly/21e6473eebb8/Image%252525202019-05-03%25252520at%252525205.30.33%25252520PM.png">

* Props and composition give you all the flexibility you need to customize a component’s look and behavior in an explicit and safe way.
* Pass a function when you can to update state multiple times.


mounting :
Mounting is the phase in which our React component mounts on the DOM (i.e., is created and inserted into the DOM). This phase comes onto the scene after the initialization phase is completed. In this phase, our component renders the first time. The methods that are available in this phase are:
componentWillMount()
componentDidMount()

lifecycle during mounting : the constructor runs > it initialize the component state > the other methods runs > the render method runs > the component mount on the dom > componentDidMount () method runs : asynchronous calls to databases or manipulate the dom directly

updating :
This phase is triggered every time state or props change.

lifecycle during updating : state or props changes > getDerivedStateFromProps is called > shouldComponentUpdate runs >compares states and props and returns either true and continue rendering or false and ends the rendering > getSnapshotBeforeUpdate runs > componentDidUpdate runs : asynchronous calls to databases or manipulate the dom directly