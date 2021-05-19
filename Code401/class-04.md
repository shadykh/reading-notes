# Readings: Data Modeling

## Review, Research, and Discussion

- Name 3 advantages to Test Driven Development
- Better program design and higher code quality
- Detailed project documentation
- TDD reduces the time required for project development
- > For further information clicks =>[here](https://www.codica.com/blog/test-driven-development-benefits/)

- In what case would you need to use beforeEach() or afterEach() in a test suite?
- beforeEach()/afterEach() automatically run before and after each tests, which 1. removes the explicit calls from the tests themselves, and 2. invites inexperienced users to share state between tests.
- > For further information clicks =>[here](https://medium.com/@_ericelliott/the-difference-is-beforeeach-aftereach-automatically-run-before-and-after-each-tests-which-1-b53a3ba5c344)

- What is one downside of Test Driven Development?
- Tests got to be maintained when requirements change
  - The strongest argument against TDD is that the tests need to be maintained because the code has got to. Whenever requirements change, you would like to vary the code and tests. But you’re working with TDD. this suggests that you simply got to change the tests first then make the tests pass. So, actually, this disadvantage is that the same as before when writing code that apparently takes an extended time.y takes a long time.
  - > For further information clicks =>[here](https://www.geeksforgeeks.org/advantages-and-disadvantages-of-test-driven-development-tdd/)

- What’s the primary difference between ES6 Classes and Constructor/Prototype Classes?
  - The most important difference between class- and prototype-based inheritance is that a class defines a type which can be instantiated at runtime, whereas a prototype is itself an object instance.
  - A class constructor creates an instance of the class. A constructor in JavaScript is just a plain old function that returns an object.
  - >For further information clicks =>[here](https://www.toptal.com/javascript/es6-class-chaos-keeps-js-developer-up#:~:text=Prototypes%20vs.,is%20itself%20an%20object%20instance.&text=A%20class%20constructor%20creates%20an%20instance%20of%20the%20class.)

- Why REST?
  - REST aims to make caching easier. Since the server is stateless and each request can be processed individually.
  - REST APIs provides a great deal of flexibility. Data is not tied to resources or methods, so REST can handle multiple types of calls, return different data formats and even change structurally with the correct implementation of hypermedia. This flexibility allows developers to build an API that meets your needs while also meeting the needs of very diverse customers.
  - >For further information clicks =>[here](https://www.mulesoft.com/resources/api/restful-api) OR [here](https://www.freecodecamp.org/news/benefits-of-rest/#:~:text=REST%20aims%20to%20make%20caching,usually%20treat%20them%20as%20such.)

## Vocabulary Terms

- functional programming
  - Is the process of building software by composing pure functions, avoiding shared state, mutable data, and side-effects. Functional programming is declarative rather than imperative, and application state flows through pure functions. Contrast with object oriented programming, where application state is usually shared and colocated with methods in objects.
  - >For further information clicks =>[here](<https://medium.com/javascript-scene/master-the-javascript-interview-what-is-functional-programming-7f218c68b3a0#:~:text=Functional%20programming%20(often%20abbreviated%20FP,state%20flows%20through%20pure%20functions>.))

- object-oriented programming (OOP)
  - Is a fundamental programming paradigm used by nearly every developer at some point in their career. OOP is the most popular programming paradigm and is taught as the standard way to code for most of a programmers educational career.
  - >For further information clicks =>[here](https://www.educative.io/blog/object-oriented-programming)

- Test Driven Development (TDD)
  - Is an evolutionary approach to development which combines test-first development where you write a test before you write just enough production code to fulfill that test and refactoring. What is the primary goal of TDD? One view is the goal of TDD is specification and not validation (Martin, Newkirk, and Kess 2003). In other words, it’s one way to think through your requirements or design before your write your functional code (implying that TDD is both an important agile requirements and agile design technique). Another view is that TDD is a programming technique.
  - >For further information clicks =>[here](http://agiledata.org/essays/tdd.html)

- Continuous Integration (CI)
  - Is the practice of automating the integration of code changes from multiple contributors into a single software project. It’s a primary DevOps best practice, allowing developers to frequently merge code changes into a central repository where builds and tests then run. Automated tools are used to assert the new code’s correctness before integration.
  - >For further information clicks =>[here](https://www.atlassian.com/continuous-delivery/continuous-integration)

- REST
  - Representational state transfer (REST) is a software architectural style which uses a subset of HTTP. It is commonly used to create interactive applications that use Web services. A Web service that follows these guidelines is called RESTful. Such a Web service must provide its Web resources in a textual representation and allow them to be read and modified with a stateless protocol and a predefined set of operations.
  - >For further information clicks =>[here](https://en.wikipedia.org/wiki/Representational_state_transfer)

- Data Model
  - A data model (or datamodel) is an abstract model that organizes elements of data and standardizes how they relate to one another and to the properties of real-world entities. For instance, a data model may specify that the data element representing a car be composed of a number of other elements which, in turn, represent the color and size of the car and define its owner.
  - >For further information clicks =>[here](https://en.wikipedia.org/wiki/Data_model#:~:text=A%20data%20model%20(or%20datamodel,properties%20of%20real%2Dworld%20entities.))

## Preparation Materials

- SQL vs NoSQL
  - SQL databases are primarily called as Relational Databases (RDBMS); whereas NoSQL database are primarily called as non-relational or distributed database.
  - SQL databases are table based databases whereas NoSQL databases are document based, key-value pairs, graph databases or wide-column stores. This means that SQL databases represent data in form of tables which consists of n number of rows of data whereas NoSQL databases are the collection of key-value pair, documents, graph databases or wide-column stores which do not have standard schema definitions which it needs to adhered to.
  - SQL databases have predefined schema whereas NoSQL databases have dynamic schema for unstructured data.
  - SQL databases are vertically scalable whereas the NoSQL databases are horizontally scalable. SQL databases are scaled by increasing the horse-power of the hardware. NoSQL databases are scaled by increasing the databases servers in the pool of resources to reduce the load.
  - SQL databases uses SQL ( structured query language ) for defining and manipulating the data, which is very powerful. In NoSQL database, queries are focused on collection of documents. Sometimes it is also called as UnQL (Unstructured Query Language). The syntax of using UnQL varies from database to database.
  - >For further information clicks =>[here](https://www.thegeekstuff.com/2014/01/sql-vs-nosql-db/?utm_source=tuicool)

- NOSQL DATA MODELING TECHNIQUES
  - The basic principles of NoSQL data modeling.
    - Conceptual Techniques
      - Denormalization
      - Aggregates
      - Application Side Joins
    - General Modeling Techniques
      - Atomic Aggregates
      - Enumerable Keys
      - Dimensionality Reduction
      - Index Table
      - Composite Key Index
      - Aggregation with Composite Keys
      - Inverted Search – Direct Aggregation
    - Hierarchy Modeling Techniques
      - Tree Aggregation
      - Adjacency Lists
      - Materialized Paths
      - Nested Sets
      - Nested Documents Flattening: Numbered Field Names
      - Nested Documents Flattening: Proximity Queries
      - Batch Graph Processing
  - >For further information clicks =>[here](https://highlyscalable.wordpress.com/2012/03/01/nosql-data-modeling-techniques/)

<br>

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
