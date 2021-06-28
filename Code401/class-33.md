# Reading: Context API

## Review, Research, and Discussion

- Describe use cases for `useMemo()` and `useReducer()`
  - `useMemo()`
    - Returns a memoized value.
  - `useReducer()`
    - When you have complex state logic that involves multiple sub-values or when the next state depends on the previous one.

- Why do custom hooks need the use prefix?
  - Its name should always start with use so that you can tell at a glance that the rules of Hooks apply to it.

- What do custom hooks usually do?
  - Custom hooks allow us to have cleaner functional components, remove logic from the UI layer, and prevent code duplication by bringing common use cases to reusable hooks.

- Using any list of custom hooks, research and name one that you think will be useful in your applications!
  - useArray hook
    - Building a todo list was never this simple. We provide the array in the hook and get access to these methods and array in the todos object below.
      - ![imge](https://miro.medium.com/max/700/1*V95Z8EecOdh01Pste56KfA.png)
        - > For further information clicks =>[here](https://blog.bitsrc.io/10-react-custom-hooks-you-should-have-in-your-toolbox-aa27d3f5564d)

- Describe how a hook that fetches API data might work?
  
  - First, we’re going to import stuff we’re going to use and create a function.
    import React, {useState, useEffect} from "react"

    ```
    const App = () => {
    return <div> Fetched data will be displayed here</div>
    }
    ```
  - The next step is to add a useState hook and to define the name of the state - in our case, that's data. Then, we define the function we’ll use later on to update the state - setData.
    In the end, we set the initial value of our state, which is null</strong in our case.

    ```
    import React, {useState, useEffect} from "react"

    const App = () => {
    const [data, setData] = useState(null)
    return <div> Fetched data will be displayed here</div>
    }
    ```
  - After adding our useState hook to handle the data, the next step is to make the fetch request.

  - First, we’re going to create a constant fetchURL, in case we need to reuse our endpoint to fetch other data, except for posts. You can check here what else you can fetch and play with.

  - Then we create an arrow function named getData and inside of that function, we’re going to call fetch().
    Inside fetch, we’re going to provide a previously defined constant fetchURL and add /posts, since we’re fetching posts.

    ```
    import React, {useState, useEffect} from "react"
    const fetchURL = "https://jsonplaceholder.typicode.com"
    const App = () => {
    const [data, setData] = useState(null)
    const getData = () =>
        fetch(`${fetchURL}/posts`)
        .then((res) => res.json())

    return <div> Fetched data will be displayed here</div>
    }
    ```
  - After defining our request, it's time to bring in useEffect. Then we’re calling our getData() function inside of the useEffect hook to set it to the local state.

  - At the end of useEffect, we added an empty array [], because that way, useEffect runs only once.

    ```
    import React, {useState, useEffect} from "react"
    const fetchURL = "https://jsonplaceholder.typicode.com"
    const App = () => {
    const [data, setData] = useState(null)
    const getData = () =>
        fetch(`${fetchURL}/posts`)
        .then((res) => res.json())

    useEffect(() => {
        getData().then((data) => setData(data))
    }, [])
    return <div> Fetched data will be displayed here</div>
    }
    ```
  - At this point, we have everything ready to show the data inside our div. We’re going to use a map() function to iterate through this array of data.

      - > For further information clicks =>[here](https://dev.to/madara/fetching-data-with-react-hooks-and-fetch-api-beginners-guide-2ick)
---

## Vocabulary

- state hook
  - useState is a Hook that lets you add React state to function components.

- effect hook
  - The Effect Hook lets you perform side effects in function components: import React, { useState, useEffect } from 'react'; function Example() { const [count, setCount] = useState(0); // Similar to componentDidMount and componentDidUpdate: useEffect(() => { // Update the document title using the browser API document.

- reducer
  - A reducer is a function that determines changes to an application's state. It uses the action it receives to determine this change. We have tools, like Redux, that help manage an application's state changes in a single store so that they behave consistently.
  - reducer hook
    - The useReducer is a hook I use sometimes to manage the state of the application. ... It acts as an alternate hook to the useState hook to manage complex state in your application. The useReducer hook uses the same concept as the reducers in Redux. It is basically a pure function, with no side-effects.

---

## Preparation

- Context
  - Context provides a way to pass data through the component tree without having to pass props down manually at every level.
  - In a typical React application, data is passed top-down (parent to child) via props, but such usage can be cumbersome for certain types of props (e.g. locale preference, UI theme) that are required by many components within an application. Context provides a way to share values like these between components without having to explicitly pass a prop through every level of the tree
- When to Use Context ?
  - Context is designed to share data that can be considered “global” for a tree of React components, such as the current authenticated user, theme, or preferred language.

- Before You Use Context
  - Context is primarily used when some data needs to be accessible by many components at different nesting levels. Apply it sparingly because it makes component reuse more difficult.

  - If you only want to avoid passing some props through many levels, component composition is often a simpler solution than context.


  - > For further information clicks =>[here](https://reactjs.org/docs/context.html#when-to-use-context) OR [here](https://medium.com/swlh/snackbars-in-react-an-exercise-in-hooks-and-context-299b43fd2a2b)

---
<br>

[<img src="assets/main.gif">](README)
<br>

| <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)"> **Read** </span> |  <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)"> **Title** </span>  |   <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)"> **ToGo** </span>  |
| ----------- | ----------- | ----------- |
| <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)"> Read: 01 </span>      | <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)">Pre-Work - Code 401: Advanced Javascript Development</span>       |[<img src="assets/taphere.gif">](class-01)|
| <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)"> Read: 02 </span>      | <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)">Readings: Express</span>       |[<img src="assets/taphere.gif">](class-02)|
| <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)"> Read: 03 </span>      | <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)">Readings: Express REST API</span>       |[<img src="assets/taphere.gif">](class-03)|
| <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)"> Read: 04 </span>      | <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)">Readings: Data Modeling</span>       |[<img src="assets/taphere.gif">](class-04)|
| <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)"> Read: 06 </span>      | <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)">Readings: Authentication</span>       |[<img src="assets/taphere.gif">](class-06)|
| <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)"> Read: 07 </span>      | <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)">Reading: Bearer Authorization</span>       |[<img src="assets/taphere.gif">](class-07)|
| <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)"> Read: 08 </span>      | <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)">Reading: Access Control (ACL)</span>       |[<img src="assets/taphere.gif">](class-08)|
| <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)"> Read: 09 </span>      | <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)">Reading: OAuth 2</span>       |[<img src="assets/taphere.gif">](class-09)|
| <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)"> Read: 11 </span>      | <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)">Readings: Event Driven Applications</span>       |[<img src="assets/taphere.gif">](class-11)|
| <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)"> Read: 12 </span>      | <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)">Readings: Socket.io</span>       |[<img src="assets/taphere.gif">](class-12)|
| <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)"> Read: 13 </span>      | <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)">Readings: Message Queues</span>       |[<img src="assets/taphere.gif">](class-13)|
| <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)"> Read: 14 </span>      | <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)">Readings: Event Driven Architecture</span>       |[<img src="assets/taphere.gif">](class-14)|
| <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)"> Read: 16 </span>      | <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)">Readings: AWS: Cloud Servers</span>       |[<img src="assets/taphere.gif">](class-16)|
| <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)"> Read: 17 </span>      | <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)">Readings: AWS: S3 and Lambda</span>       |[<img src="assets/taphere.gif">](class-17)|
| <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)"> Read: 18 </span>      | <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)">Readings: AWS: API, Dynamo and Lambda</span>       |[<img src="assets/taphere.gif">](class-18)|
| <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)"> Read: 18 </span>      | <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)">Readings: AWS: Events</span>       |[<img src="assets/taphere.gif">](class-19)|
| <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)"> Read: 26 </span>      | <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)">Reading: Component Based UI</span>       |[<img src="assets/taphere.gif">](class-26)|
| <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)"> Read: 27 </span>      | <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)">Reading: Props and State</span>       |[<img src="assets/taphere.gif">](class-27)|
| <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)"> Read: 28 </span>      | <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)">Readings: Component Composition</span>       |[<img src="assets/taphere.gif">](class-28)|
| <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)"> Read: 29 </span>      | <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)">Readings: Routing</span>       |[<img src="assets/taphere.gif">](class-29)|
| <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)"> Read: 31 </span>      | <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)">Reading: Hooks API</span>       |[<img src="assets/taphere.gif">](class-31)|
| <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)"> Read: 32 </span>      | <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)">Reading: Custom Hooks</span>       |[<img src="assets/taphere.gif">](class-32)|
| <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)"> Read: 33 </span>      | <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)">Reading: Context API</span>       |[<img src="assets/taphere.gif">](class-33)|
