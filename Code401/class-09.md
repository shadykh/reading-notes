# Reading: OAuth 2

## OAuth 2 
The OAuth 2 spec can be a bit confusing to read, so I've written this post to help describe the terminology in a simplified format. The core spec leaves many decisions up to the implementer, often based on security tradeoffs of the implementation. Instead of describing all possible decisions that need to be made to successfully implement OAuth 2, this post makes decisions that are appropriate for most implementations.

## Roles
The Third-Party Application: "Client"
    - The client is the application that is attempting to get access to the user's account. It needs to get permission from the user before it can do so.

The API: "Resource Server"
    - The resource server is the API server used to access the user's information.

The Authorization Server
    - This is the server that presents the interface where the user approves or denies the request. In smaller implementations, this may be the same server as the API server, but larger scale deployments will often build this as a separate component.

The User: "Resource Owner"
    - The resource owner is the person who is giving access to some portion of their account.

## Authorization
The first step of OAuth 2 is to get authorization from the user. For browser-based or mobile apps, this is usually accomplished by displaying an interface provided by the service to the user.

OAuth 2 provides several "grant types" for different use cases. The grant types defined are:
    - Authorization Code for apps running on a web server, browser-based and mobile apps
    - Password for logging in with a username and password (only for first-party apps)
    - Client credentials for application access without a user present
    - Implicit was previously recommended for clients without a secret, but has been superseded by using the Authorization Code grant with PKCE.

## Abstract Protocol Flow
Now that you have an idea of what the OAuth roles are, let’s look at a diagram of how they generally interact with each other:
    - ![Abstract Protocol Flow](https://assets.digitalocean.com/articles/oauth/abstract_flow.png)

Here is a more detailed explanation of the steps in the diagram:

    - The application requests authorization to access service resources from the user
    - If the user authorized the request, the application receives an authorization grant
    - The application requests an access token from the authorization server (API) by presenting authentication of its own identity, and the authorization grant
    - If the application identity is authenticated and the authorization grant is valid, the authorization server (API) issues an access token to the application. Authorization is complete.
    - The application requests the resource from the resource server (API) and presents the access token for authentication
    - If the access token is valid, the resource server (API) serves the resource to the application


  - > For further information clicks =>[here](https://aaronparecki.com/oauth-2-simplified/) OR [here](https://www.digitalocean.com/community/tutorials/an-introduction-to-oauth-2)



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