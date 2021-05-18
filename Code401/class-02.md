<img src="../assets/logo.png"
 title="LTUC-Abdul Aziz Al Ghurair School of Advanced Computing" width="200" />  &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; <span style="font-family:Papyrus; font-size:25px;color:rgb(60, 179, 113)">**Welcome to Read: 02**</span>

---
<br>

<span style="font-family:Courier New; font-size:20px;color:rgb(60, 179, 113)"> **Readings: Express** </span>

<span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)">In this Read: 02, I will talk about those topics:
</span>

- <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)">Review, Research, and Discussion.
</span>
- <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)"> Vocabulary Terms.
</span>
- <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)"> Preparation.

<br>

---
<br>

<span style="font-family:Courier New; font-size:20px;color:rgb(60, 179, 113)">**Review, Research, and Discussion** </span>

- <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)">What’s the difference between PUT and PATCH?</span><br>
  - <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)">The main difference between the PUT and PATCH method is that the PUT method uses the request URI to supply a modified version of the requested resource which replaces the original version of the resource, whereas the PATCH method supplies a set of instructions to modify the resource. If the PATCH document is larger than the size of the new version of the resource sent by the PUT method then the PUT method is preferred.
    </span>
        > For further information clicks =>[here](https://en.wikipedia.org/wiki/Patch_verb#:~:text=The%20main%20difference%20between%20the,instructions%20to%20modify%20the%20resource.)

- <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)">Provide links to 3 services or tools that allow you to “mock” an API for development like json-server?</span><br>
  - <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)">Postman.
    </span>
  - <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)">Stoplight .
    </span>
  - <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)">Nock .
    </span>
        > For further information clicks =>[here](https://developers.amadeus.com/blog/helpful-tools-to-create-mock-servers)

- <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)">Compare and contrast Swagger and APIDoc.js 1 Which HTTP status codes should be sent with each type of (un)successful API call?</span><br>
  - <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)">Popularity: By comparing stats,  swagger-ui is more popular then apidocjs.
    </span>
  - <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)">Consistency: If we already using swagger for our Dotnetcore service, then implementing swagger tool will consist more from Info and UI prospective.
    </span>
  - <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)">Maintenance: For apidocjs will have to modify documentation for each affected method/endpoints if service changed. In swagger we can limit changes. But by implementing apidocjs we can isolate the layer.
    </span>
        > For further information clicks =>[here](https://www.asptricks.net/2019/04/apidoc-vs-swagger-for-node-app.html)

- <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)">Compare and contrast SOAP and ReST</span><br>
  - <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)">Soap;SOAP provides the following advantages when compared to REST:
    </span>
    - <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)">Language, platform, and transport independent (REST requires use of HTTP)
    </span>
    - <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)">Works well in distributed enterprise environments (REST assumes direct point-to-point communication)
    </span>
    - <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)">Standardized
    </span>
    - <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)">Provides significant pre-build extensibility in the form of the WS* standards
    </span>
    - <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)">Built-in error handling
    </span>
    - <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)">Automation when used with certain language products
    </span>

  - <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)">REST;REST is easier to use for the most part and is more flexible. It has the following advantages over SOAP:
    </span>
    - <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)">No expensive tools require to interact with the web service
    </span>
    - <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)">Smaller learning curve
    </span>
    - <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)">Efficient (SOAP uses XML for all messages, REST can use smaller message formats)
    </span>
    - <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)">Fast (no extensive processing required)
    </span>
    - <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)">Closer to other web technologies in design philosophy
    </span>
        > For further information clicks =>[here](https://smartbear.com/blog/soap-vs-rest-whats-the-difference/)

---
<br>

<span style="font-family:Courier New; font-size:20px;color:rgb(60, 179, 113)">**Vocabulary Terms** </span>

- <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)">Web Server</span><br>
  - <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)">A web server is a computer that runs websites. It's a computer program that distributes web pages as they are requisitioned. The basic objective of the web server is to store, process and deliver web pages to the users. This intercommunication is done using Hypertext Transfer Protocol (HTTP).
    </span>
    > For further information clicks =>[here](https://economictimes.indiatimes.com/definition/web-server#:~:text=Definition%3A%20A%20web%20server%20is,Hypertext%20Transfer%20Protocol%20(HTTP).)

- <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)">Express</span><br>
  - <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)">Is a back end web application framework for Node.js, released as free and open-source software under the MIT License. It is designed for building web applications and APIs. It has been called the de facto standard server framework for Node.js.
    </span>
    > For further information clicks =>[here](https://en.wikipedia.org/wiki/Express.js#:~:text=js%2C%20or%20simply%20Express%2C%20is,standard%20server%20framework%20for%20Node.)

- <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)">Routing</span><br>
  - <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)">Routing is the process of moving a packet of data from source to destination. The principles of routing can apply to many networks such as circuit-switched networks and computer networks. Routing is typically performed by a specialized device known as a router.
    </span>
    > For further information clicks =>[here](https://www.webopedia.com/definitions/routing/)

---
<br>

<span style="font-family:Courier New; font-size:20px;color:rgb(60, 179, 113)">**Preparation** </span>

- <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)">Express/Node</span><br>
  - <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)">**Node** (or more formally Node.js) is an open-source, cross-platform runtime environment that allows developers to create all kinds of server-side tools and applications in JavaScript. The runtime is intended for use outside of a browser context (i.e. running directly on a computer or server OS). As such, the environment omits browser-specific JavaScript APIs and adds support for more traditional OS APIs including HTTP and file system libraries. <br>
  **Express** is the most popular Node web framework, and is the underlying library for a number of other popular Node web frameworks. While Express itself is fairly minimalist, developers have created compatible middleware packages to address almost any web development problem. There are libraries to work with cookies, sessions, user logins, URL parameters, POST data, security headers, and many more.
    </span>
    > For further information clicks =>[here](https://developer.mozilla.org/en-US/docs/Learn/Server-side/Express_Nodejs/Introduction) 

- <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)">About npm</span><br>
  - <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)">npm is the world's largest software registry. Open source developers from every continent use npm to share and borrow packages, and many organizations use npm to manage private development as well.
    </span>
    > For further information clicks =>[here](https://docs.npmjs.com/about-npm) 

- <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)">TDD</span><br>
  - <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)">“Test-driven development” refers to a style of programming in which three activities are tightly interwoven: coding, testing (in the form of writing unit tests) and design (in the form of refactoring).
    </span>
    > For further information clicks =>[here](https://www.agilealliance.org/glossary/tdd/#q=~(infinite~false~filters~(postType~(~'page~'post~'aa_book~'aa_event_session~'aa_experience_report~'aa_glossary~'aa_research_paper~'aa_video)~tags~(~'tdd))~searchTerm~'~sort~false~sortDirection~'asc~page~1)) 

- <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)">CI/CD</span><br>
  - <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)">Continuous integration (CI) and continuous delivery (CD) embody a culture, set of operating principles, and collection of practices that enable application development teams to deliver code changes more frequently and reliably. The implementation is also known as the CI/CD pipeline. 
    </span>
    > For further information clicks =>[here](https://www.infoworld.com/article/3271126/what-is-cicd-continuous-integration-and-continuous-delivery-explained.html) 
    
---
<br>

[<img src="assets/main.gif">](README)
<br>

| <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)"> **Read** </span> |  <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)"> **Title** </span>  |   <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)"> **ToGo** </span>  |
| ----------- | ----------- | ----------- |
| <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)"> Read: 01 </span>      | <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)">Pre-Work - Code 401: Advanced Javascript Development</span>       |[<img src="assets/taphere.gif">](class-01)|
| <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)"> Read: 02 </span>      | <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)">Readings: Express</span>       |[<img src="assets/taphere.gif">](class-02)|
| <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)"> Read: 03 </span>      | <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)">Readings: Express REST API</span>       |[<img src="assets/taphere.gif">](class-03)|