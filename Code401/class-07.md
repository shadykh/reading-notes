# Readings: Authentication

## Review, Research, and Discussion

- Write the following steps in the correct order
  - Ask the client if they want to sign in via a third party
  - Register your application to get a client_id and client_secret
  - Make a request to a third-party API endpoint
  - Receive access token
  - Receive authorization code
  - Redirect to a third party authentication endpoint
  - Make a request to the access token endpoint

- What can you do with an authorization code?
  - Used with sucre login

- What can you do with an access token?
  - Used with sucre login

- What’s a benefit of using OAuth instead of your own basic authentication?
  - Because it is a delegated authorization framework for REST/APIs. It enables apps to obtain limited access (scopes) to a user's data without giving away a user's password. It decouples authentication from authorization and supports multiple use cases addressing different device capabilities.
  - > For further information clicks =>[here](https://www.oauth.com/oauth2-servers/access-tokens/#:~:text=Access%20tokens%20are%20the%20thing,in%20transit%20and%20in%20storage.)

## Vocabulary

- Client ID
  - is a public identifier for apps. Even though it’s public, it’s best that it isn’t guessable by third parties, so many implementations use something like a 32-character hex string. It must also be unique across all clients that the authorization server handles.
  - > For further information clicks =>[here](https://www.oauth.com/oauth2-servers/client-registration/client-id-secret/#:~:text=The%20client_id%20is%20a%20public,that%20the%20authorization%20server%20handles.)  
- Client Secret
  - A client secret is a secret known only to your application and the authorization server. It protects your resources by only granting tokens to authorized requestors.
  - > For further information clicks =>[here](https://en.wikipedia.org/wiki/Singleton_pattern#:~:text=In%20software%20engineering%2C%20the%20singleton,mathematical%20concept%20of%20a%20singleton.)
- Authentication Endpoint
  - is an authentication mechanism used to verify the identity of a network's external or remote connecting device. These endpoint devices include laptops, smartphones, tablets, and servers. This method ensures that only valid or authorized endpoint devices are connected to a network.
  - > For further information clicks =>[here](https://www.iotone.com/term/end-point-authentication/t219)
- Access Token Endpoint
  - is where apps make a request to get an access token for a user. This section describes how to verify token requests and how to return the appropriate response and errors. Authorization Code. Password Grant. Client Credentials
  - > For further information clicks =>[here](https://www.oauth.com/oauth2-servers/access-tokens/)
- API Endpoint
  - is the point of entry in a communication channel when two systems are interacting. It refers to touchpoints of the communication between an API and a server.
  - > For further information clicks =>[here](https://rapidapi.com/blog/api-glossary/endpoint/#:~:text=In%20simple%20terms%2C%20an%20API,an%20API%20and%20a%20server.&text=An%20API%20endpoint%20is%20basically,of%20a%20server%20or%20service.)
- Authorization Code
  - is a temporary code that the client will exchange for an access token. The code itself is obtained from the authorization server where the user gets a chance to see what the information the client is requesting, and approve or deny the request.
  - > For further information clicks =>[here](https://www.oauth.com/oauth2-servers/server-side-apps/authorization-code/#:~:text=The%20authorization%20code%20is%20a,approve%20or%20deny%20the%20request.)
- Access Token
  - is an object encapsulating the security identity of a process or thread. A token is used to make security decisions and to store tamper-proof information about some system entity.
  - > For further information clicks =>[here](https://en.wikipedia.org/wiki/Access_token#:~:text=An%20access%20token%20is%20an,information%20about%20some%20system%20entity.)

## Preparation

- JWT
  - What is JSON Web Token?
    - JSON Web Token (JWT) is an open standard (RFC 7519) that defines a compact and self-contained way for securely transmitting information between parties as a JSON object. This information can be verified and trusted because it is digitally signed. JWTs can be signed using a secret (with the HMAC algorithm) or a public/private key pair using RSA or ECDSA.
  - When should you use JSON Web Tokens?
    - Authorization
      - This is the most common scenario for using JWT. Once the user is logged in, each subsequent request will include the JWT, allowing the user to access routes, services, and resources that are permitted with that token. Single Sign On is a feature that widely uses JWT nowadays, because of its small overhead and its ability to be easily used across different domains.
    - Information Exchange
      - JSON Web Tokens are a good way of securely transmitting information between parties. Because JWTs can be signed—for example, using public/private key pairs—you can be sure the senders are who they say they are. Additionally, as the signature is calculated using the header and the payload, you can also verify that the content hasn't been tampered with.
  - What is the JSON Web Token structure?
    - Header
    - Payload
    - Signature
    - Example of it:
      - ![example](https://cdn.auth0.com/blog/legacy-app-auth/legacy-app-auth-5.png)

  - > For further information clicks =>[here](https://jwt.io/introduction/)


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
| <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)"> Read: 06 </span>      | <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)">Reading: Bearer Authorization</span>       |[<img src="assets/taphere.gif">](class-07)|
