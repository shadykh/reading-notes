<img src="../assets/logo.png"
 title="LTUC-Abdul Aziz Al Ghurair School of Advanced Computing" width="200" />  &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; <span style="font-family:Papyrus; font-size:25px;color:rgb(60, 179, 113)">**Welcome to Read: 03**</span>

---
<br>

<span style="font-family:Courier New; font-size:20px;color:rgb(60, 179, 113)"> **Readings: Express REST API** </span>

<span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)">In this Read: 03, I will talk about those topics:
</span>

- <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)">Review, Research, and Discussion.
</span>
- <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)"> Vocabulary Terms.
</span>
- <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)"> Preparation.

<br>

---
<br>

---
<br>

<span style="font-family:Courier New; font-size:20px;color:rgb(60, 179, 113)">**Review, Research, and Discussion** </span>

- <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)">Name 3 real world use cases where you’d want to change the request with custom middleware</span><br>
  - <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)">Translator.
    </span>
  - <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)">Accumulating-Duplicating Data.
    </span>
  - <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)">API Security.
    </span>
      - > For further information clicks =>[here](https://www.freecodecamp.org/news/what-is-middleware-with-example-use-cases/)

- <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)">True or false: The route handler is middleware?</span><br>
  - <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)">In Express, there is no hard and fast distinction between the two. Someone would generally call something middleware that examines a bunch of different requests and usually prepares the request for further processing. Someone would generally call something a route handler that is targeted at a specific URL (or type of URL) and whose main purpose is to send a response back to the client for that URL.
    </span>
    - > For further information clicks =>[here](https://stackoverflow.com/questions/58925276/what-is-the-difference-between-a-route-handler-and-middleware-function-in-expres)

- <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)">At what point in the request lifecycle can you “inject” middleware?</span><br>
  - <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)">any point of the request life cycle.
    </span>
      - > For further information clicks =>[here](https://dev.to/teamhive/creating-a-transaction-interceptor-using-nest-js-2inb)

- <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)">What can cause express to error with “Request headers sent twice, cannot start a second response”</span><br>
  - <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)">Soap;SOAP provides the following advantages when compared to REST:
    </span>
    - <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)">ٍSending response twice. So, you are getting the error second time because the the response is already send.
    </span>
      - > For further information clicks =>[here](https://stackoverflow.com/questions/58816095/node-js-express-cannot-set-headers-after-they-are-sent-to-the-client)


---
<br>

<span style="font-family:Courier New; font-size:20px;color:rgb(60, 179, 113)">**Vocabulary Terms** </span>

- <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)">Middleware</span><br>
  - <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)">Middleware is software that bridges gaps between other applications, tools, and databases in order to provide unified services to users. 
    </span>
  - > For further information clicks =>[here](https://www.talend.com/resources/what-is-middleware/#:~:text=Middleware%20is%20software%20that%20bridges,software%20platforms%20and%20devices%20together.)

- <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)">Request Object</span><br>
  - <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)">The request object allows you to submit a POST or GET request to an URL. Essentially it provides a way to make REST API requests to another URL. An example scenario is if you need to submit form information to a 3rd party as well as save it within the CMS.
    </span>
  - > For further information clicks =>[here](https://www.branchcms.com/learn/docs/developer/twig/request-object)

- <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)">Response Object</span><br>
  - <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)">It is the object which communicates between the server and the output which is sent to the client.
    </span>
  - > For further information clicks =>[here](https://www.4guysfromrolla.com/webtech/faq/Beginner/faq3.shtml#:~:text=One%20of%20the%20most%20important,is%20sent%20to%20the%20client.)

- <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)">Test Driven Development</span><br>
  - <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)">Test Driven Development (TDD) is software development approach in which test cases are developed to specify and validate what the code will do. In simple terms, test cases for each functionality are created and tested first and if the test fails then the new code is written in order to pass the test and making code simple and bug-free.
    </span>
  - > For further information clicks =>[here](https://www.guru99.com/test-driven-development.html)

- <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)">Behavioral Testing</span><br>
  - <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)">Behavioural Testing is a testing of the external behaviour of the program, also known as black box testing. It is usually a functional testing.
    </span>
  - > For further information clicks =>[here](https://www.tutorialspoint.com/software_testing_dictionary/behaviour_testing.htm#:~:text=Behavioural%20Testing%20is%20a%20testing,is%20usually%20a%20functional%20testing.)
---
<br>

<span style="font-family:Courier New; font-size:20px;color:rgb(60, 179, 113)">**Preparation** </span>

- <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)">Classes</span><br>
  - <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)">Classes are a template for creating objects. They encapsulate data with code to work on that data. Classes in JS are built on prototypes but also have some syntax and semantics that are not shared with ES5 class-like semantics. Classes are in fact "special functions", and just as you can define function expressions and function declarations, the class syntax has two components: class expressions and class declarations.
    </span>
    > For further information clicks =>[here](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Classes) 

- <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)">Routing</span><br>
  - <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)">Routing refers to how an application’s endpoints (URIs) respond to client requests. For an introduction to routing, see Basic routing. <br> You define routing using methods of the Express app object that correspond to HTTP methods; for example, app.get() to handle GET requests and app.post to handle POST requests. For a full list, see app.METHOD. You can also use app.all() to handle all HTTP methods and app.use() to specify middleware as the callback function (See Using middleware for details).
    </span>
    > For further information clicks =>[here]https://expressjs.com/en/guide/routing.html) 

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