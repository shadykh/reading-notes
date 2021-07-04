# Readings: Redux - Combined Reducers

## Review, Research, and Discussion

- Why choose Redux instead of the Context API for global state?
  - So when using redux we can subscribe to the state or a peace/selection of the state and when the state or the selection of the state changes the subscribed component re-renders.
  - But what does that means? It means if your components are not subscribed to the store they won't re-render after a dispatch.
  - So now with that in mind if you have a lot of components simultaneously updating the global state where changes made by one component might not affect most of the other components. And you have lots and lots of those redux will give a performance edge.
- What is the purpose of a reducer?
  - A reducer is a function that determines changes to an application's state. It uses the action it receives to determine this change. We have tools, like Redux, that help manage an application's state changes in a single store so that they behave consistently.

- What does an action contain?
  - Actions are the only source of information for the store as per Redux official documentation. It carries a payload of information from your application to store.

- Why do we need to copy the state in a reducer?
  - In the documentation of reducers(read it again for details!), redux only requires our reducers to stay pure. If the new state is different, the reducer must create new object, and making a copy is a way to describe the unchanged part.

---

## Vocabulary

- immutable state
  - In object-oriented and functional programming, an immutable object (unchangeable object) is an object whose state cannot be modified after it is created. This is in contrast to a mutable object (changeable object), which can be modified after it is created.
- time travel in redux
  - Time travel is the ability to move back and forth among the previous states of an application and view the results in real time. With Redux, given a specific state and a specific action, the next state of the application is always exactly the same.
- action creator
  - An action creator is merely a function that returns an action object. Redux includes a utility function called bindActionCreators for binding one or more action creators to the store's dispatch() function.
- reducer
  - A reducer is a function that determines changes to an application's state. It uses the action it receives to determine this change. We have tools, like Redux, that help manage an application's state changes in a single store so that they behave consistently.
- dispatch
  - dispatch() is the method used to dispatch actions and trigger state changes to the store. react-redux is simply trying to give you convenient access to it. Note, however, that dispatch is not available on props if you do pass in actions to your connect function.

---

## Preparation

- combineReducers
  - The most common state shape for a Redux app is a plain Javascript object containing "slices" of domain-specific data at each top-level key. Similarly, the most common approach to writing reducer logic for that state shape is to have "slice reducer" functions, each with the same (state, action) signature, and each responsible for managing all updates to that specific slice of state. Multiple slice reducers can respond to the same action, independently update their own slice as needed, and the updated slices are combined into the new state object.
  - Because this pattern is so common, Redux provides the combineReducers utility to implement that behavior. It is an example of a higher-order reducer, which takes an object full of slice reducer functions, and returns a new reducer function.
- There are several important ideas to be aware of when using combineReducers:
  - First and foremost, combineReducers is simply a utility function to simplify the most common use case when writing Redux reducers. You are not required to use it in your own application, and it does not handle every possible scenario. It is entirely possible to write reducer logic without using it, and it is quite common to need to write custom reducer logic for cases that combineReducer does not handle. (See Beyond combineReducers for examples and suggestions.)
  - While Redux itself is not opinionated about how your state is organized, combineReducers enforces several rules to help users avoid common errors. (See combineReducers for details.)
  - One frequently asked question is whether Redux "calls all reducers" when dispatching an action. Since there really is only one root reducer function, the default answer is "no, it does not". However, combineReducers has specific behavior that does work that way. In order to assemble the new state tree, combineReducers will call each slice reducer with its current slice of state and the current action, giving the slice reducer a chance to respond and update its slice of state if needed. So, in that sense, using combineReducers does "call all reducers", or at least all of the slice reducers it is wrapping.
  - multiple combined reducers in various places, which are composed together to create the root reducer.
  - The way Redux works is simple. There is a central store that holds the entire state of the application. Each component can access the stored state without having to send down props from one component to another.

- Notes
  - For any action that is not recognized, it must return the state given to it as the first argument.
  - It must never return undefined. It is too easy to do this by mistake via an early return statement, so combineReducers throws if you do that instead of letting the error manifest itself somewhere else.
  - If the state given to it is undefined, it must return the initial state for this specific reducer. According to the previous rule, the initial state must not be undefined either. It is handy to specify it with ES6 optional arguments syntax, but you can also explicitly check the first argument for being undefined.

  - > For further information clicks =>[here](https://redux.js.org/api/combinereducers/) OR [here](https://redux.js.org/usage/structuring-reducers/using-combinereducers/)

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
