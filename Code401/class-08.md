# Reading: Access Control (ACL)

## Review, Research, and Discussion

- When is Basic Authorization used vs. Bearer Authorization?
  - Basic Authorization
    - The use case for this are integration with reporting tools like PowerBI and Tableau.
  - Bearer Authorization
    - It is the recommended Authentication methods whenever possible. It is ideal when scripting, when developing external app or when doing integration with external tools.
  - > For further information clicks =>[here](https://community.mega.com/t5/REST-API/Basic-Auth-vs-Bearer-Token/td-p/23476)

- What does the JSON Web Token package do?
  - Usend information that can be verified and trusted by means of a digital signature. It comprises a compact and URL-safe JSON object, which is cryptographically signed to verify its authenticity, and which can also be encrypted if the payload contains sensitive information.
  - > For further information clicks =>[here](https://www.toptal.com/web/cookie-free-authentication-with-json-web-tokens-an-example-in-laravel-and-angularjs)

- What considerations should we make when creating and storing a SECRET?
  - Never store unencrypted secrets in .git repositories
    - Avoid git add * commands on git
    - Add sensitive files in .gitignore
    - Don’t rely on code reviews to discover secrets
    - Use automated secrets scanning on repositories
  - Don’t share your secrets unencrypted in messaging systems like slack
  - Store secrets safely
    - Use encryption to store secrets within .git repositories
    - Use environment variables
    - Use "Secrets as a service" solutions
  - Restrict API access and permissions
    - Default to minimal permission scope for APIs
    - Whitelist IP addresses where appropriate
    - Use short-lived secrets
  - > For further information clicks =>[here](https://blog.gitguardian.com/secrets-api-management/)

## Vocabulary

- encryption
  - is the method by which information is converted into secret code that hides the information's true meaning. The science of encrypting and decrypting information is called cryptography.
  - > For further information clicks =>[here](https://searchsecurity.techtarget.com/definition/encryption#:~:text=Encryption%20is%20the%20method%20by,encrypted%20data%20is%20called%20ciphertext.)  
- token
  -  is a piece of a two-factor authentication security device that may be used to authorize the use of computer services.
  - > For further information clicks =>[here](https://en.wikipedia.org/wiki/Software_token#:~:text=A%20software%20token%20(a.k.a.%20soft,phone%20and%20can%20be%20duplicated.))
- bearer 
  - s an opaque string, not intended to have any meaning to clients using it. Some servers will issue tokens that are a short string of hexadecimal characters, while others may use structured tokens such as JSON Web Tokens.
  - > For further information clicks =>[here](https://oauth.net/2/bearer-tokens/#:~:text=Bearer%20Tokens%20are%20the%20predominant,such%20as%20JSON%20Web%20Tokens.)
- secret
  - is private to you which means you will never reveal that to the public or inject inside the JWT token
  - > For further information clicks =>[here](https://medium.com/jspoint/so-what-the-heck-is-jwt-or-json-web-token-dca8bcb719a6#:~:text=JWT%20is%20created%20with%20a,key%20stored%20on%20the%20server.)
- JSON Web Token
  - is an open standard (RFC 7519) that defines a compact and self-contained way for securely transmitting information between parties as a JSON object. This information can be verified and trusted because it is digitally signed. JWTs can be signed using a secret (with the HMAC algorithm) or a public/private key pair using RSA or ECDSA.
  - > For further information clicks =>[here](https://jwt.io/introduction)


## Preparation

- RBAC
  - What is RBAC?
    - Role-based access control (RBAC) is a policy-neutral access-control mechanism defined around roles and privileges. The components of RBAC such as role-permissions, user-role and role-role relationships make it simple to perform user assignments. A study by NIST has demonstrated that RBAC addresses many needs of commercial and government organizations.[5] RBAC can be used to facilitate administration of security in large organizations with hundreds of users and thousands of permissions. Although RBAC is different from MAC and DAC access control frameworks, it can enforce these policies without any complication.

  - Benefits of RBAC??
    - the assignment of access rights becomes systematic and repeatable.
    - it is much easier to audit user rights, and to correct any issues identified.
    - it can in reality be easy to implement, and will make the ongoing management of access rights much easier and more secure.

  - RBAC implementation 
    - Inventory your systems
        - Figure out what resources you have for which you need to control access, if you don't already have them listed. Examples would include an email system, customer database, contact management system, major folders on a file server, etc. 
    - Analyze your workforce and create roles
        - You need to group your workforce members into roles with common access needs. Avoid the temptation to have too many roles defined. Keep them as simple and stratified as possible.
    - Assign people to roles
        - Now that you have a list of roles and their access rights, figure out which role(s) each employee belongs in, and set their access accordingly. 
    - Never make one-off changes
      - Resist any temptation to make a one-off change for an employee with unusual needs. If you begin doing this, your RBAC system will quickly begin to unravel. Change the roles as required or add new ones when really necessary. 
    - Audit
        - Periodically review your roles, the employees assigned to them, and the access permitted for each. If you discover, for example, that a role has unnecessary access to a particular system, change the role and adjust the access level for all employees in that role.  

  - > For further information clicks =>[here](https://www.csoonline.com/article/3060780/5-steps-to-simple-role-based-access-control.html)

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