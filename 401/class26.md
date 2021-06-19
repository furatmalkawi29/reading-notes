# Review, Research, and Discussion

1. Name 5 Javascript UI Frameworks (other than React)

1. Ext JS
2. Angular
3. Vue 
4. Svelte 3
5. Ember

2. What’s the difference between a framework and a library?

- Frameworks and libraries are both code written by someone else that helps you perform some common tasks in an easier way . 

- The difference is in the inversion of control :
A framework tells the developer what they need, the developer is controlled by framework . A library doesn’t. The programmer calls the library functions where and when they need it.

 <br><br>

# Terms

- rendering : 

When you open a website in your browser, the server sends some data to your machine. Now this data can be in multiple formats such as HTML, XML, JSON etc 

HTML and XML data can be parsed by browser to create a visual effect. Hence the browser parses the HTML response from the server and shows it on your screen. This is called as rendering.
(parsing is turning HTML elements are into a “DOM tree” )

- templetes : 
 refers to a web technology technique that defines the presentation (layout and style) of web pages. These forms are then filled in by a template engine (or processor). 

 - state :

 The state is an instance of React Component Class can be defined as an object of a set of observable properties that control the behavior of the component. In other words, the State of a component is an object that holds some information that may change over the lifetime of the component.


 <br><br>

## Summery :

* JSX produces React “elements”.
* React embraces the fact that rendering logic is inherently coupled with other UI logic: how events are handled, how the state changes over time, and how the data is prepared for display.

* React separates concerns with loosely coupled units called “components” that contain both.


* React doesn’t require using JSX, but most people find it helpful as a visual aid when working with UI inside the JavaScript code.
* It also allows React to show more useful error and warning messages.
* You can put any valid JavaScript expression inside the curly braces in JSX. 
* After compilation, JSX expressions become regular JavaScript function calls and evaluate to JavaScript objects.
* If a tag is empty, you may close it immediately with `/>`.
* JSX tags may contain children.
* ` React.createElement()` performs a few checks to help you write bug-free code but essentially it creates an object.


* An element describes what you want to see on the screen.
* React elements are plain objects, and are cheap to create.
* Applications built with just React usually have a single root DOM node.
* To render a React element into a root DOM node, pass both to `ReactDOM.render()`.
* React elements are immutable : Once you create an element, you can’t change its children or attributes.

