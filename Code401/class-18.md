# Readings: AWS: API, Dynamo and Lambda

## Review, Research, and Discussion

- What are serverless functions?
  - A serverless function is a programmatic function written by a software developer for a single purpose. It's then hosted and maintained on infrastructure by cloud computing companies. These companies take care of code maintenance and execution so that developers can deploy new code faster and easier.
  - > For further information clicks =>[here](https://blog.hubspot.com/website/serverless-functions)

- If you were to create a system that emulated Lambda functions, how would you do it?
  - To create a Lambda function with the console
    - Open the Functions page on the Lambda console.
    - Choose Create function.
    - Under Basic information, do the following:
    - For Function name, enter my-function.
    - For Runtime, confirm that Node.js 14.x is selected. Note that Lambda provides runtimes for .NET (PowerShell,C#) Go, Java, Node.js, Python, and Ruby.
    - Choose Create function.
    - Lambda creates a Node.js function and an execution role that grants the function permission to upload logs. The Lambda function assumes the execution role when you invoke your function, and uses the execution role to create credentials for the AWS SDK and to read data from event sources.
  - > For further information clicks =>[here](https://docs.aws.amazon.com/lambda/latest/dg/getting-started-create-function.html)

- Describe how a CDN works?
  - A CDN (Content Delivery Network) is a highly-distributed platform of servers that helps minimize delays in loading web page content by reducing the physical distance between the server and the user. This helps users around the world view the same high-quality content without slow loading times.
  - The goal of the CDN is to reduce latency – the delay between submitting a request for a web page and the web page fully loading on your device – by reducing the physical distance that the request has to travel.
  - CDNs store a cached version of your website content in multiple geographical locations around the world, which are known as “points of presence” (PoPs). These PoPs will contain their own caching servers and will be responsible for delivering that content in the user’s location.

  - User-agents, which are essentially devices running web browsers, make requests for content needed to render web pages such as HTML, images, CSS, and JavaScript files. For most CDNs, each request for content will cause the end user to be mapped to an optimally-located CDN server and the server will respond with the cached (pre-saved) version of the requested files. If it fails to locate the files, it will look for the content on the other servers in the CDN platform and send the response to the end user. However, when content is unavailable or stale, the CDN will act as a request proxy to the origin server and store the fetched content to serve future requests.

  - Although the delivery of website content is a common use case for CDNs, it is not the only type of content that a CDN can deliver. In fact, CDNs deliver an incredible variety of content that includes: 4K and HD-quality video; audio streams; software downloads such as apps, games, and OS updates; data records that contain medical and financial information; and much more. Potentially any data that can be digitized can be delivered through a CDN.
  - > For further information clicks =>[here](https://www.akamai.com/us/en/cdn/what-is-a-cdn.jsp)

## Vocabulary

- Serverless functions
  - Is a programmatic function written by a software developer for a single purpose. It's then hosted and maintained on infrastructure by cloud computing companies. These companies take care of code maintenance and execution so that developers can deploy new code faster and easier.
  - > For further information clicks =>[here](https://blog.hubspot.com/website/serverless-functions)  
- Cloud storage
  - It allows you to save data and files in an off-site location that you access either through the public internet or a dedicated private network connection. Data that you transfer off-site for storage becomes the responsibility of a third-party cloud provider.
  - > For further information clicks =>[here](https://www.ibm.com/cloud/learn/cloud-storage)
- CDN
  - (Content Delivery Network) is a highly-distributed platform of servers that helps minimize delays in loading web page content by reducing the physical distance between the server and the user. This helps users around the world view the same high-quality content without slow loading times.
  - > For further information clicks =>[here](https://www.akamai.com/us/en/cdn/what-is-a-cdn.jsp)

## Preparation

- Amazon API Gateway
  - What is Amazon API Gateway?
    - Amazon API Gateway is a managed service that allows developers to define the HTTP endpoints of a REST API or a WebSocket API and connect those endpoints with the corresponding backend business logic. It also handles authentication, access control, monitoring, and tracing of API requests.

    - Many Serverless applications use Amazon API Gateway, which conveniently replaces the API servers with a managed serverless solution.
  - How does API Gateway work?
    - API Gateway sits between the backend services of your API and your API’s users, handling the HTTP requests to your API endpoints and routing them to the correct backends. It provides a set of tools that help you manage your API definitions and the mappings between endpoints and their respective backend services. It can also generate API references from your definitions and make them available to your users as API documentation.
    - > For further information clicks =>[here](https://www.serverless.com/amazon-api-gateway)

- DynamoDB
  - What is DynamoDB?
    - DynamoDB is a hosted NoSQL database offered by Amazon Web Services (AWS). It offers:
      - reliable performance even as it scales;
      - a managed experience, so you won't be SSH-ing into servers to upgrade the crypto libraries;
      - a small, simple API allowing for simple key-value access as well as more advanced query patterns.
  - DynamoDB is a particularly good fit for the following use cases:
    - Applications with large amounts of data and strict latency requirements.
      - As your amount of data scales, JOINs and advanced SQL operations can slow down your queries. With DynamoDB, your queries have predictable latency up to any size, including over 100 TBs!

    - Serverless applications using AWS Lambda.
      - AWS Lambda provides auto-scaling, stateless, ephemeral compute in response to event triggers. DynamoDB is accessible via an HTTP API and performs authentication & authorization via IAM roles, making it a perfect fit for building Serverless applications.
    - Data sets with simple, known access patterns.
      - If you're generating recommendations and serving them to users, DynamoDB's simple key-value access patterns make it a fast, reliable choice.

  - > For further information clicks =>[here](https://www.dynamodbguide.com/what-is-dynamo-db/)

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
