<img src="https://asac.ltuc.com/wp-content/themes/asac/images/logo.png" alt="Kitten"
	title="LTUC-Abdul Aziz Al Ghurair School of Advanced Computing" width="200" />  &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; <span style="font-family:Papyrus; font-size:25px;color:rgb(60, 179, 113)">**Welcome to Read: 10**</span>

---
<br>

<span style="font-family:Courier New; font-size:20px;color:rgb(60, 179, 113)"> **The Call Stack and Debugging** </span>


<span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)">In this Read: 10, I will talk about those topics: 
</span>
- <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)">Call stack.
- <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)">Debugging.
<br>

---
<br>

<span style="font-family:Courier New; font-size:20px;color:rgb(60, 179, 113)">**Call stack** </span><br>
<span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)">A call stack is a mechanism for an interpreter (like the JavaScript interpreter in a web browser) to keep track of its place in a script that calls multiple functions — what function is currently being run and what functions are called from within that function, etc.<br>
</span> 

- <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)">What It Is and Why It's Necessary</span><br>


    - <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)">An understanding of the call stack will give clarity to how “function hierarchy and execution order” works in the JavaScript engine. The call stack is primarily used for function invocation (call). Since the call stack is single, function(s) execution, is done, one at a time, from top to bottom. It means the call stack is synchronous. <br> <br>
    In Asynchronous JavaScript, we have a callback function, an event loop, and a task queue. The callback function is acted upon by the call stack during execution after the call back function has been pushed to the stack by the event loop.</span><br>

- <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)">Temporarily store</span><br>


    - <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)">When a function is invoked (called), the function, its parameters, and variables are pushed into the call stack to form a stack frame. This stack frame is a memory location in the stack. The memory is cleared when the function returns as it is pop out of the stack.</span><br>

- <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)">In summary</span><br>

    - <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)">The key takeaways from the call stack are:</span><br>
        - <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)">It is single-threaded. Meaning it can only do one thing at a time.</span><br>
        - <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)">Code execution is synchronous.</span><br>
        - <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)">A function invocation creates a stack frame that occupies a temporary memory.</span><br>
        - <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)">It works as a LIFO — Last In, First Out data structure.</span><br>        


---
<br>

<span style="font-family:Courier New; font-size:20px;color:rgb(60, 179, 113)">**Debugging** </span><br>
<span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)">Debugging is the process of detecting and removing of existing and potential errors (also called as 'bugs') in a software code that can cause it to behave unexpectedly or crash.Sometimes it takes more time to debug a program than to code it.<br>
</span> 

- <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)">Types of error messages</span><br>


    - <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)">Reference errors</span><br>
        - <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)">This is as simple as when you try to use a variable that is not yet declared you get this type os errors.</span><br> 
        `console.log(foo) // Uncaught ReferenceError: foo is not defined `
        - <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)">This is also a common thing when using const and let, they are hoisted like var and function but there is a time between the hoisting and being declared so when you try to access them a reference error occurs, the fact that this happens to let and const is called Temporal Dead Zone (TDZ).</span><br> 
        `foo = 'Hello' // Uncaught ReferenceError: foo is not defined let foo `

    - <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)">Syntax errors</span><br>
        - <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)">This occurs when you have something that cannot be parsed in terms of syntax, like when you try to parse an invalid object using JSON.parse.</span><br> 
        `JSON.parse( {'foo': 'bar'} ) // Uncaught SyntaxError: Unexpected token o in JSON at position 1 `


    - <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)">Range errors</span><br>
        - <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)">Try to manipulate an object with some kind of length and give it an invalid length and this kind of errors will show up..</span><br> 
        ```
            var foo= []
            foo.length = foo.length -1
            // Uncaught RangeError: Invalid array length
        ```
    - <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)">Type errors</span><br>
        - <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)">This types of errors show up when the types (number, string and so on) you are trying to use or access are incompatible, like accessing a property in an undefined type of variable.</span><br> 
        ```
            var foo = {}
            foo.bar // undefined
            foo.bar.baz 
            // Uncaught TypeError: Cannot read property
             'baz' of undefined
        ```

- <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)">Debugging</span><br>


    - <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)">To debug your JS code, the easiest and maybe the most common way its to simply console.log() the variables you want to check or, by using chrome developer tools, open your page with your JS code (press cmd+o in macOS or Ctrl+o in Windows) and choose your file to debug, click the line you wanna debug and refresh your page again (F5).<br> If the line you selected was run you will be able to see what has happened before that point and you can try and evaluate the next lines to check if everything is outputting what you are expecting.<br> The breakpoint can also be achieved by putting a debugger statement in your code in the line you want to break.</span><br>
    ![Debugging](https://miro.medium.com/max/625/1*ByuRUFwh_Nul0ZOOx4QVRg.png)




> For further infromation about Call Stack please click [here](https://developer.mozilla.org/en-US/docs/Glossary/Call_stack) Or [here](https://www.freecodecamp.org/news/understanding-the-javascript-call-stack-861e41ae61d4/). <br>  <br>

> For further infromation about Debugging please click [here](https://codeburst.io/javascript-error-messages-debugging-d23f84f0ae7c).
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
| <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)"> Read: 12 </span>      | <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)"> Components </span>       |[<img src="assets/taphere.gif">](class-12f)|
| <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)"> Read: 13 </span>      | <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)"> Update/Delete </span>       |[<img src="assets/taphere.gif">](class-13)|
| <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)"> Read: 14a </span>      | <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)"> DB Normalization </span>       |[<img src="assets/taphere.gif">](class-14a)|
| <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)"> Read: 14b </span>      | <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)"> Project Ideas & APIs </span>       |[<img src="assets/taphere.gif">](class-14b)|
| <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)"> Read: 15 </span>      | <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)"> Diversity and Inclusion </span>       |[<img src="assets/taphere.gif">](class-14b)|




