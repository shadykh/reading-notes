# Readings: AWS: Events

## Review, Research, and Discussion

- Describe the similarities between AWS API Gateway + Lambda functions and an ExpressJS Server ?
  - They will handle http request endpoints.

- List the AWS Database offerings and talk about the pros and cons of each
  - Amazon RDS
    - Amazon Relational Database Service or Amazon RDS is a managed cloud database service from AWS. It is a service designed to simplify the creation, operation, management, and scaling of a relational database for use as an application backend. AWS launched the RDS service initially in October 2009 with support for MySQL.

| Pros | Cons |
| ----------- | ----------- |
| Automated Patching | Patching forces a downtime |
| Automated Backups | No scale-out for write workloads |
| Encryption at rest and in-transit | Downtime required for scaling operations |
| Significant improvement over on-premise databases | No automated performance tuning |
| Integrated with rest of the AWS ecosystem | Not a zero-administration database |
| No hardware maintenance needed | No automated partition management |
| Simplified scaling in comparison to on-premise databases | No automated compression management |
| Automated log shipping and read read replica | No root access to the server |
| Simplified disaster recovery and automatic failover | No native support as a read replica for on-premise Databases |
| Automated additional storage allocation | CPU and Storage performance is not guaranteed |
| Point in time recovery | Zero data loss is not guaranteed |

- > For further information clicks =>[here](https://sarasanalytics.com/blog/amazon-rds-pros-and-cons)

- What’s the difference between a FIFO and a standard queue?
  - Standard queues guarantee that a message is delivered at least once and duplicates can be introduced into the queue.
  - FIFO queues ensure a message is delivered exactly once and remains available until a consumer processes and deletes it; duplicates are not introduced into the queue.

  - > For further information clicks =>[here](https://medium.com/awesome-cloud/aws-difference-between-sqs-standard-and-fifo-first-in-first-out-queues-28d1ea5e153#:~:text=Standard%20queues%20guarantee%20that%20a,not%20introduced%20into%20the%20queue.)

- How can the server be assured a message was properly received?
  - The message oriented architecture is a solution where nodes communicate by sending messages. The key factor in this approach is an ability to communicate in an asynchronous way. This kind of information exchange gives wide possibilities to manage both time and delivery path. When a traditional synchronous model takes place, client has to wait being blocked until server replies or a timeout mechanism occurs (if applicable).

  - > For further information clicks =>[here](http://blog.softexploration.com/message-oriented-middleware/client-server-message-oriented-communication.html)

## Vocabulary

- Serverless API
  - Serverless is a cloud computing execution model where the cloud provider dynamically manages the allocation and provisioning of servers. A serverless application runs in stateless compute containers that are event-triggered, ephemeral (may last for one invocation), and fully managed by the cloud provider.
  - > For further information clicks =>[here](https://hackernoon.com/what-is-serverless-architecture-what-are-its-pros-and-cons-cc4b804022e9)  

- DynamoDB vs MongoDB
| DynamoDB | MongoDB |
| ----------- | ----------- |
| MongoDB is vendor agnostic, Open Source, and can be deployed anywhere | DynamoDB is only available on AWS |
| MongoDB can be self installed or fully managed with MongoDB Atlas | DynamoDB is a fully managed AWS service |
| DynamoDB uses tables, items and attributes | MongoDB uses JSON-like documents |
| DynamoDB supports limited data types and smaller item sizes | MongoDB supports more data types and has fewer size restrictions |
  - > For further information clicks =>[here](https://www.xplenty.com/blog/dynamodb-vs-mongodb-differences/)

- Dynamoose vs Mongoose
  - Dynamoose used by the AWS, Mongoose used by the Express
  - > For further information clicks =>[here](https://www.akamai.com/us/en/cdn/what-is-a-cdn.jsp)

## Preparation

- SQS and SNS Basics
  - SNS is a distributed publish-subscribe system. Messages are pushed to subscribers as and when they are sent by publishers to SNS.
  - SQS is distributed queuing system. Messages are not pushed to receivers. Receivers have to poll or pull messages from SQS.

  - The Amazon Simple Queue Service (SQS) and the Amazon Simple Notification Service (SNS) are important “glue” components for scalable, cloud-based applications (see the Reference Architectures in the AWS Architecture Center to learn more about how to put them to use in your own applications).

    - > For further information clicks =>[here](https://aws.amazon.com/blogs/aws/queues-and-notifications-now-best-friends/) or [here](https://stackoverflow.com/questions/13681213/what-is-the-difference-between-amazon-sns-and-amazon-sqs)




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

