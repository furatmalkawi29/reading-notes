# React Native

## Review, Research, and Discussion


* Compare and Contrast Redux Toolkit with Redux “Ducks”: Ducks is a way to bundle reducers, action types, and actions into the same file. 
 * Rather than splitting up related code, it can be packaged into redux modules. Redux Toolkit's goal is to help simplify common Redux use cases. It is not intended to be a complete solution for everything you might want to do with Redux, but it should make a lot of Redux-related code you need to write a lot simpler. Redux Toolkit exports several individual functions that you can use in your application, and adds in dependencies on some other packages that are commonly used with Redux. 
* What is the principle advantage of Redux Toolkit.
 *  Helps to solve three major problems with Redux: configuring a Redux store, adding numerous packages to get Redux to things, and removing unnecessary or boilerplate code. 

## Vocabulary Terms

### Redux Toolkit slices :
 * Redux slice is a collection of reducer logic and actions for a single feature of application. Redux state is typically organized into slices, defined by the reducers that are passed to combineReducers.

### Namespace : 
 * Programming paradigm of providing scope to identifiers (names of types, functions, variables, etc) to prevent collisions between them. JavaScript does not provide namespace by default. However, we can replicate this functionality by making a global object which can contain all functions and variables.



## React Native

<img src ="https://www.appstud.com/wp-content/uploads/2018/03/React-Native-Titre.png">

* a framework that enables web developers to create robust mobile applications using their existing JavaScript knowledge.
* In other words: It is an popular JavaScript-based mobile app framework that allows you to build natively-rendered mobile apps for iOS and Android.
* It offers faster mobile development, and more efficient code sharing across iOS, Android, and the Web, without sacrificing the end user's experience or application quality.
* supported by Facebook.

## React Native Vs React

* React Native :
  * uses native components as building blocks.
* React :
  * uses web components as building blocks.

## React Native Pros & Cons 

<img src ="https://a.storyblok.com/f/86602/720x497/6966bc5d94/react-pros-cons.jpg">

## React Native vs Flutter

<img src ="https://nix-united.com/wp-content/uploads/2020/01/pics-for-Email_mailchimp.key-2021-03-15-17-12-03.jpg">

## Building a react native app:

* Install react native and react.
* import { Text, View, StyleSheet, Button } from 'react-native'
* `<View></View>` with style attribute: renders a container.
* `<Text>` Test goes Here `</Text>`: render a text.
* `<Image></Image>`
* StyleSheet.create().