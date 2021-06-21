# Reading: Props and State

## Review, Research, and Discussion

- Does a deployed React application require a server?
  - No you don’t need a server.

- Why do we prefer to test a React application at the behavior rather than the unit level?
  - The user will deal with the app so it is better to test the whole app behavior.

- What does `npm run build` do?
  - will create an optimized build of your app in the build folder.

- Describe the actual composition / architecture of a React application
  1. Components of the page.
  2. an app which is had the components
  3. an index renders the app

---

## Vocabulary

- BDD
  - Behavior-driven development, in software engineering, behavior-driven development is an agile software development process that encourages collaboration among developers, quality assurance testers, and customer representatives in a software project.  
  - > For further information clicks =>[here](https://en.wikipedia.org/wiki/Behavior-driven_development)  

- Acceptance Tests
  - Acceptance testing, a testing technique performed to determine whether or not the software system has met the requirement specifications. The main purpose of this test is to evaluate the system's compliance with the business requirements and verify if it is has met the required criteria for delivery to end users.
  - > For further information clicks =>[here](https://www.tutorialspoint.com/software_testing_dictionary/acceptance_testing.htm#:~:text=Acceptance%20testing%2C%20a%20testing%20technique,for%20delivery%20to%20end%20users.)

- Mounting
  - Mounting is the phase in which our React component mounts on the DOM (i.e., is created and inserted into the DOM). This method is called just before a component mounts on the DOM or the render method is called. After this method, the component gets mounted.
  - > For further information clicks =>[here](https://www.freecodecamp.org/news/how-to-understand-a-components-lifecycle-methods-in-reactjs-e1a609840630/#:~:text=Mounting%20is%20the%20phase%20in,and%20inserted%20into%20the%20DOM).&text=This%20method%20is%20called%20just,method%2C%20the%20component%20gets%20mounted.)

- build
  - It correctly bundles React in production mode and optimizes the build for the best performance. The build is minified and the filenames include the hashes. Behind the scenes, it uses babel to transpile your code and webpack as the build tool to bundle up your application.
  - > For further information clicks =>[here](https://stackoverflow.com/questions/43830866/what-is-npm-run-build-in-create-react-app)

---

## Preparation

- setState
  - React components can, and often do, have state. State can be anything, but think of things like whether a user is logged in or not and displaying the correct username based on which account is active. Or an array of blog posts. Or if a modal is open or not and which tab within it is active.
  - React components with state render UI based on that state. When the state of components changes, so does the component UI.
  - That makes understanding when and how to change the state of your component important. At the end of this tutorial, you should know how setState works, and be able to avoid common pitfalls that many of us hit when when learning React.
  - > For further information clicks =>[here](https://css-tricks.com/understanding-react-setstate/)

- Handling Events
  - Handling events with React elements is very similar to handling events on DOM elements. There are some syntax differences:
    - React events are named using camelCase, rather than lowercase.
    - With JSX you pass a function as the event handler, rather than a string.
  - > For further information clicks =>[here](https://reactjs.org/docs/handling-events.html)

- Forms
  - Handling events with React elements is very similar to handling events on DOM elements. There are some syntax differences:
    - React events are named using camelCase, rather than lowercase.
    - With JSX you pass a function as the event handler, rather than a string.
  - > For further information clicks =>[here](https://reactjs.org/docs/handling-events.html)

- Handling Events
  - HTML form elements work a bit differently from other DOM elements in React, because form elements naturally keep some internal state.
  - Controlled Components:
    - In HTML, form elements such as `<input>`, `<textarea>`, and `<select>` typically maintain their own state and update it based on user input. In React, mutable state is typically kept in the state property of components, and only updated with setState().
    - We can combine the two by making the React state be the “single source of truth”. Then the React component that renders a form also controls what happens in that form on subsequent user input. An input form element whose value is controlled by React in this way is called a “controlled component”.
  - > For further information clicks =>[here](https://reactjs.org/docs/forms.html)

- State and Lifecycle
  - Each component has several “lifecycle methods” that you can override to run code at particular times in the process. You can use this lifecycle diagram as a cheat sheet. In the list below, commonly used lifecycle methods are marked as bold. The rest of them exist for relatively rare use cases.
    - Mounting
    - These methods are called in the following order when an instance of a component is being created and inserted into the DOM:
      - constructor()
      - static getDerivedStateFromProps()
      - render()
      - componentDidMount()
    - Updating
    - An update can be caused by changes to props or state. These methods are called in the following order when a component is being re-rendered:
      - static getDerivedStateFromProps()
      - shouldComponentUpdate()
      - render()
      - getSnapshotBeforeUpdate()
      - componentDidUpdate()
  - > For further information clicks =>[here](https://reactjs.org/docs/react-component.html)

- Components and Props
  - Components let you split the UI into independent, reusable pieces, and think about each piece in isolation. This page provides an introduction to the idea of components. 
  - > For further information clicks =>[here](https://reactjs.org/docs/components-and-props.html)

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
