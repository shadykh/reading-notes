# Reading: React Native

## Review, Research, and Discussion

- Compare and Contrast Redux Toolkit with Redux “Ducks”?
  - Redux Toolkit’s it’s helps to simplify common Redux use cases.
  - Ducks is a modular pattern that collocates actions, action types and reducers.
- What is the principle advantage of Redux Toolkit?
  - Redux Toolkit makes it easier to write good Redux applications and speeds up development, by baking in our recommended best practices, providing good default behaviors, catching mistakes, and allowing you to write simpler code. Redux Toolkit is beneficial to all Redux users regardless of skill level or experience. It can be added at the start of a new project, or used as part of an incremental migration in an existing project.

---

## Vocabulary

- redux toolkit slices
  - A function that accepts an initial state, an object full of reducer functions, and a "slice name", and automatically generates action creators and action types that correspond to the reducers and state. This API is the standard approach for writing Redux logic.
- namespace
  - In computing, a namespace is a set of signs that are used to identify and refer to objects of various kinds. A namespace ensures that all of a given set of objects have unique names so that they can be easily identified. Namespaces are commonly structured as hierarchies to allow reuse of names in different contexts.

---

## Preparation

- React Native
  - React Native combines the best parts of native development with React, a best-in-class JavaScript library for building user interfaces.
  - Use a little—or a lot. You can use React Native today in your existing Android and iOS projects or you can create a whole new app from scratch.
  - React primitives render to native platform UI, meaning your app uses the same native platform APIs other apps do.
  - Many platforms, one React. Create platform-specific versions of components so a single codebase can share code across platforms. With React Native, one team can maintain two platforms and share a common technology—React.
  - React Native lets you create truly native apps and doesn't compromise your users' experiences. It provides a core set of platform agnostic native components like View, Text, and Image that map directly to the platform’s native UI building blocks.
  - React components wrap existing native code and interact with native APIs via React’s declarative UI paradigm and JavaScript. This enables native app development for whole new teams of developers, and can let existing native teams work much faster.
- Expo
  - Expo is a framework and a platform for universal React applications. It is a set of tools and services built around React Native and native platforms that help you develop, build, deploy, and quickly iterate on iOS, Android, and web apps from the same JavaScript/TypeScript codebase.
  - Expo is an open-source platform for making universal native apps for Android, iOS, and the web with JavaScript and React.
- ExpoKit
  - ExpoKit is an Objective-C and Java library that allows you to use the Expo platform and your existing Expo project as part of a larger standard native project -- one that you would normally create using Xcode, Android Studio, or react-native init.
  - If you created an Expo project and you want a way to add custom native modules, this guide will explain how to use ExpoKit for that purpose.
  - Normally, Expo apps are written in pure JS and never "drop down" to the native iOS or Android layer. This is core to the Expo philosophy and it's part of what makes Expo fast and powerful to use.
  - However, there are some cases where advanced developers need native capabilities outside of what Expo offers out-of-the-box. The most common situation is when a project requires a specific Native Module which is not supported by React Native Core or the Expo SDK.
  - In this case, Expo allows you to eject your pure-JS project from the Expo iOS/Android clients, providing you with native projects that can be opened and built with Xcode and Android Studio. Those projects will have dependencies on ExpoKit, so everything you already built will keep working as it did before.
  - We call this "ejecting" because you still depend on the Expo SDK, but your project no longer lives inside Expo Go. You control the native projects, including configuring and building them yourself.

- > For further information clicks =>[here](https://reactnative.dev/docs/getting-started) OR [here](https://docs.expo.io/get-started/errors/)

---

<br>

[<img src="assets/main.gif">](README)
<br>

| <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)"> **Read** </span> | <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)"> **Title** </span>                                          | <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)"> **ToGo** </span> |
| ----------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------- |
| <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)"> Read: 01 </span> | <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)">Pre-Work - Code 401: Advanced Javascript Development</span> | [<img src="assets/taphere.gif">](class-01)                                                      |
| <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)"> Read: 02 </span> | <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)">Readings: Express</span>                                    | [<img src="assets/taphere.gif">](class-02)                                                      |
| <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)"> Read: 03 </span> | <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)">Readings: Express REST API</span>                           | [<img src="assets/taphere.gif">](class-03)                                                      |
| <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)"> Read: 04 </span> | <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)">Readings: Data Modeling</span>                              | [<img src="assets/taphere.gif">](class-04)                                                      |
| <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)"> Read: 06 </span> | <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)">Readings: Authentication</span>                             | [<img src="assets/taphere.gif">](class-06)                                                      |
| <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)"> Read: 07 </span> | <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)">Reading: Bearer Authorization</span>                        | [<img src="assets/taphere.gif">](class-07)                                                      |
| <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)"> Read: 08 </span> | <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)">Reading: Access Control (ACL)</span>                        | [<img src="assets/taphere.gif">](class-08)                                                      |
| <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)"> Read: 09 </span> | <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)">Reading: OAuth 2</span>                                     | [<img src="assets/taphere.gif">](class-09)                                                      |
| <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)"> Read: 11 </span> | <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)">Readings: Event Driven Applications</span>                  | [<img src="assets/taphere.gif">](class-11)                                                      |
| <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)"> Read: 12 </span> | <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)">Readings: Socket.io</span>                                  | [<img src="assets/taphere.gif">](class-12)                                                      |
| <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)"> Read: 13 </span> | <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)">Readings: Message Queues</span>                             | [<img src="assets/taphere.gif">](class-13)                                                      |
| <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)"> Read: 14 </span> | <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)">Readings: Event Driven Architecture</span>                  | [<img src="assets/taphere.gif">](class-14)                                                      |
| <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)"> Read: 16 </span> | <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)">Readings: AWS: Cloud Servers</span>                         | [<img src="assets/taphere.gif">](class-16)                                                      |
| <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)"> Read: 17 </span> | <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)">Readings: AWS: S3 and Lambda</span>                         | [<img src="assets/taphere.gif">](class-17)                                                      |
| <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)"> Read: 18 </span> | <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)">Readings: AWS: API, Dynamo and Lambda</span>                | [<img src="assets/taphere.gif">](class-18)                                                      |
| <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)"> Read: 18 </span> | <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)">Readings: AWS: Events</span>                                | [<img src="assets/taphere.gif">](class-19)                                                      |
| <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)"> Read: 26 </span> | <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)">Reading: Component Based UI</span>                          | [<img src="assets/taphere.gif">](class-26)                                                      |
| <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)"> Read: 27 </span> | <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)">Reading: Props and State</span>                             | [<img src="assets/taphere.gif">](class-27)                                                      |
| <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)"> Read: 28 </span> | <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)">Readings: Component Composition</span>                      | [<img src="assets/taphere.gif">](class-28)                                                      |
| <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)"> Read: 29 </span> | <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)">Readings: Routing</span>                                    | [<img src="assets/taphere.gif">](class-29)                                                      |
| <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)"> Read: 31 </span> | <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)">Reading: Hooks API</span>                                   | [<img src="assets/taphere.gif">](class-31)                                                      |
| <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)"> Read: 32 </span> | <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)">Reading: Custom Hooks</span>                                | [<img src="assets/taphere.gif">](class-32)                                                      |
| <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)"> Read: 33 </span> | <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)">Reading: Context API</span>                                 | [<img src="assets/taphere.gif">](class-33)                                                      |
| <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)"> Read: 34 </span> | <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)">Reading: `<Login />` and `<Auth />`</span>                  | [<img src="assets/taphere.gif">](class-34)                                                      |
| <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)"> Read: 36 </span>      | <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)">Reading: Application State with Redux</span>       |[<img src="assets/taphere.gif">](class-36)|
| <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)"> Read: 37 </span>      | <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)">Readings: Redux - Combined Reducers</span>       |[<img src="assets/taphere.gif">](class-37)|
| <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)"> Read: 38 </span>      | <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)">Readings: Redux - Asynchronous Actions</span>       |[<img src="assets/taphere.gif">](class-38)|
| <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)"> Read: 39 </span>      | <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)">Readings: Redux - Additional Topics</span>       |[<img src="assets/taphere.gif">](class-39)|
| <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)"> Read: 41 </span>      | <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)"> Reading: React Native </span>       |[<img src="assets/taphere.gif">](class-41)|
