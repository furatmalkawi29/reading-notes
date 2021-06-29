# `<Login />` and `<Auth />`

## Review, Research, and Discussion


* Why is the Context API useful?
  * Context provides a way to pass data through the component tree without having to pass props down manually at every level. 

  
* Can a component outside of a provider get its context?
  * It can get global context, cannot get Context.Provider.

* What are some common use cases for using the Context API?
 * Useful for sharing data that can be considered global, such as currently authenticated user, or theme settings for the application.

* Describe “Context Hell”
 * Context API has virtually no boilerplate in comparison to Redux, adding Context Providers makes for messy and unreadable code.


## Vocabulary Terms

### global state :
  * Keeping a state at the top level of an application and providing access methods to all child levels without the need to pass props. Global state should only keep states that concern the entire app, such as theme, language, or other app-wide settings.

### global context :
  * Context provides a way to share values and data between components without having to explicity pass a prop through every level of the tree. Designed to share data that can be considered "global" for a tree of React components, such as the current authenticated user, theme, or preferred language.

### provider :
  * Every Context object comes with a Provider React component that allows consuming components to subscribe to context changes. Provider component accepts a value prop to be passed to consuming components that are descendants of this Provider. One Provider can be connected to many consumers. Providers can be nested to override values deeper within the tree. 

### consumer :
  * Consumers are decendants of a Provider that will re-render whenever the Provider's value prop changes. The propagation from Provider to its descendant consumers (including .contextType and useContext) is not subject to the shouldComponentUpdate method, so the consumer is updated even when an ancestor component skips an update.

## Role-Based Access Control

<img src ="https://docs.oracle.com/cd/E65459_01/admin.1112/e65449/content/images/admin/rbac/rbac_overview.png">

* Role-Baed Access Control (RBAC):
 * As the name suggests, RBAC is a system that allow different access to users based on their roles.
 * It is used for protection of credentials.
 * Access is based on the roles and not on the users.

* RBAC implementation:
 * Define the resources that you need to limit access to.
 * Define what roles you need for which resources.
 * Assign people to those roles.
 * Be careful when changing roles or adding new ones.
 * Audit your system.