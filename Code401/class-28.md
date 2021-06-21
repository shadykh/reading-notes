# Readings: Component Composition

## Review, Research, and Discussion

- Can a parent component access the state of a child component?
  - yes.

- What can be passed along in a prop variable?
  - State.

- How can a child component “know” the state of another component?
  - By using props.


---

## Vocabulary

- component props
  - Props are arguments passed into React components.
  - Props are passed to components via HTML attributes.
  - React Props are like function arguments in JavaScript and attributes in HTML.
  - > For further information clicks =>[here](https://www.w3schools.com/react/react_props.asp)  

- component state
  - The state is an instance of React Component Class can be defined as an object of a set of observable properties that control the behavior of the component. In other words, the State of a component is an object that holds some information that may change over the lifetime of the component.
  - > For further information clicks =>[here](https://www.geeksforgeeks.org/reactjs-state-react/)

- application state
  - State is a JavaScript object. It stores a component's dynamic data and determines the component's behavior. ... State helps in keeping the data of different components in sync since each state update will re-render all relevant components.
  - > For further information clicks =>[here](https://www.unthinkable.co/blog/5-types-of-application-state-in-react-and-how-they-help-in-state-management/)


---

## Preparation

- The Component Lifecycle
  - The component lifecycle is exactly what it sounds like: it details the life of a component. Like us, components are born, do some things during their time here on earth, and then they die .
  - ![The Component Lifecycle](https://cdn-media-1.freecodecamp.org/images/1*U13Mlxz_ktcajaeJCyYkwg.png)
  - A component can only be in one stage at a time. It starts with mounting and moves onto updating. It stays updating perpetually until it gets removed from the virtual DOM. Then it goes into the unmounting phase and gets removed from the DOM.

- Higher-Order Components
  - A higher-order component is a function that takes a component and returns a new component.
  - A good use case for an HOC is authorization. You could write your authentication code in every single component that needs it. It would quickly and unnecessarily bloat your code.

- React State and setState()
  - Most of you have probably used React state, we even used it in our HOC example. But it’s important to understand that when there’s a state change, React will trigger a re-render on that component (unless you specify in shouldComponentUpdate to say otherwise).
  - Now let’s talk about how we change state. The only way you should change state is via the setState method. This method takes an object and merges it into the current state. On top of this, there are a few things you should also know about it.

- React Context
  - The React context API allows you to create global context objects that can be given to any component you make. This allows you to share data without having to pass props down all the way through the DOM tree.

- Stay up to date with React!
  - It’s simply keeping up with the latest releases of React. React has made some serious changes lately and it’s only going to continue to grow and develop.
  - For example, in React 16.3, certain lifecycle methods were deprecated, in React 16.6 we now get async components, and in 16.7 we get hooks which aim to replace class components entirely.
    - > For further information clicks =>[here](https://reactjs.org/docs/handling-events.html)

- props.children
  - The React docs say that you can use props.children on components that represent ‘generic boxes’ and that ‘don’t know their children ahead of time’. For me, that didn’t really clear things up. I’m sure for some, that definition makes perfect sense but it didn’t for me.
  - My simple explanation of what this.props.children does is that it is used to display whatever you include between the opening and closing tags when invoking a component.
  - > For further information clicks =>[here](https://codeburst.io/a-quick-intro-to-reacts-props-children-cb3d2fce4891)

- Composition vs Inheritance
  - React has a powerful composition model, and we recommend using composition instead of inheritance to reuse code between components.
  - Props and composition give you all the flexibility you need to customize a component’s look and behavior in an explicit and safe way. Remember that components may accept arbitrary props, including primitive values, React elements, or functions.
  - If you want to reuse non-UI functionality between components, we suggest extracting it into a separate JavaScript module. The components may import it and use that function, object, or a class, without extending it.

  - > For further information clicks =>[here](https://reactjs.org/docs/composition-vs-inheritance.html)



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
