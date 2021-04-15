<img src="https://asac.ltuc.com/wp-content/themes/asac/images/logo.png" alt="Kitten"
	title="LTUC-Abdul Aziz Al Ghurair School of Advanced Computing" width="200" />  &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; <span style="font-family:Papyrus; font-size:25px;color:rgb(60, 179, 113)">**Welcome to Read: 13**</span>

---
<br>

<span style="font-family:Courier New; font-size:20px;color:rgb(60, 179, 113)"> **SENDING FORM DATA** </span>


<span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)">In this Read: 13, I will talk about this topic: 
</span>
- <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)">SENDING FORM DATA.
<br>

---
<br>

<span style="font-family:Courier New; font-size:20px;color:rgb(60, 179, 113)">**SENDING FORM DATA** </span><br>
<span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)">Once the form data has been validated on the client-side, it is okay to submit the form. But what happens when a user submits a form — where does the data go, and how do we handle it when it gets there? We also look at some of the security concerns associated with sending form data.<br>
</span> 

- <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)">Client/server architecture</span><br>

    - <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)">At it's most basic, the web uses a client/server architecture that can be summarized as follows. a client (usually a web browser) sends a request to a server (most of the time a web server like Apache, Nginx, IIS, Tomcat, etc.), using the HTTP protocol. The server answers the request using the same protocol.<br> An HTML form on a web page is nothing more than a convenient user-friendly way to configure an HTTP request to send data to a server. This enables the user to provide information to be delivered in the HTTP request.</span><br>
        ![Client/server](https://developer.mozilla.org/en-US/docs/Learn/Forms/Sending_and_retrieving_form_data/client-server.png)

- <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)">On the client side: defining how to send the data</span><br>

    - <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)">The `<form>` element defines how the data will be sent. All of its attributes are designed to let you configure the request to be sent when a user hits a submit button. The two most important attributes are `action` and `method`.</span><br>

    - <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)">The action attribute</span><br>
        - <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)">The action attribute defines where the data gets sent. Its value must be a valid relative or absolute URL. If this attribute isn't provided, the data will be sent to the URL of the page containing the form — the current page.</span><br>

    - <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)">The method attribute</span><br>
        - <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)">The method attribute defines how data is sent. The HTTP protocol provides several ways to perform a request; HTML form data can be transmitted via a number of different methods, the most common being the GET method and the POST method</span><br>
        - <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)">The GET method</span><br>
            - <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)">The GET method is the method used by the browser to ask the server to send back a given resource: "Hey server, I want to get this resource." In this case, the browser sends an empty body. Because the body is empty, if a form is sent using this method the data sent to the server is appended to the URL.</span><br>

        - <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)">The POST method</span><br>
            - <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)">The POST method is a little different. It's the method the browser uses to talk to the server when asking for a response that takes into account the data provided in the body of the HTTP request: "Hey server, take a look at this data and send me back an appropriate result." If a form is sent using this method, the data is appended to the body of the HTTP request.</span><br>




<br><br>

> For further infromation please click [here](https://developer.mozilla.org/en-US/docs/Learn/Forms/Sending_and_retrieving_form_data).

<br>


<br>

---
<br>

[<img src="assets/main.gif">](README)
<br>

| <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)"> **Read** </span> |  <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)"> **Title** </span>  |   <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)"> **ToGo** </span>  |
| ----------- | ----------- | ----------- |
| <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)"> Read: 01 </span>      | <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)"> SMACSS and Responsive Web Design </span>       |[<img src="assets/taphere.gif">](class-01)|
| <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)"> Read: 02 </span>      | <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)"> jQuery, Events, and The DOM </span>       |[<img src="assets/taphere.gif">](class-02)|
| <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)"> Read: 03 </span>      | <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)"> Flexbox and Templating </span>       |[<img src="assets/taphere.gif">](class-03)|
| <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)"> Read: 04 </span>      | <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)"> Responsive Web Design and Regular Expressions </span>       |[<img src="assets/taphere.gif">](class-04)|
| <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)"> Read: 05 </span>      | <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)"> Heroku Deployment </span>       |[<img src="assets/taphere.gif">](class-05)|
| <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)"> Read: 06 </span>      | <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)"> Node, Express, and APIs </span>       |[<img src="assets/taphere.gif">](class-06)|
| <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)"> Read: 07 </span>      | <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)"> APIs continued </span>       |[<img src="assets/taphere.gif">](class-07)|
| <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)"> Read: 08 </span>      | <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)"> SQL </span>       |[<img src="assets/taphere.gif">](class-08)|
| <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)"> Read: 09 </span>      | <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)"> Refactoring </span>       |[<img src="assets/taphere.gif">](class-09)|
| <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)"> Read: 10 </span>      | <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)"> The Call Stack and Debugging </span>       |[<img src="assets/taphere.gif">](class-10)|
| <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)"> Read: 11 </span>      | <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)"> EJS </span>       |[<img src="assets/taphere.gif">](class-11)|
| <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)"> Read: 12 </span>      | <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)"> Components </span>       |[<img src="assets/taphere.gif">](class-12)|
| <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)"> Read: 13 </span>      | <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)"> Update/Delete </span>       |[<img src="assets/taphere.gif">](class-13)|
| <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)"> Read: 14a </span>      | <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)"> DB Normalization </span>       |[<img src="assets/taphere.gif">](class-14a)|
| <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)"> Read: 15 </span>      | <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)"> Diversity and Inclusion </span>       |[<img src="assets/taphere.gif">](class-15)|






