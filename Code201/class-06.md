<img src="https://asac.ltuc.com/wp-content/themes/asac/images/logo.png" alt="Kitten"
	title="LTUC-Abdul Aziz Al Ghurair School of Advanced Computing" width="200" />  &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; <span style="font-family:Papyrus; font-size:25px;color:rgb(60, 179, 113)">**Welcome to Read: 06**</span>

---
<br>

<span style="font-family:Courier New; font-size:20px;color:rgb(60, 179, 113)"> **Read: 06 - "JS Object Literals; The DOM"** </span>

<span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)">In this Read: 06, I will have those three topics: 
</span><br>
- <span style="font-family:Courier New; font-size:15px;color:rgb(250, 179, 113)"> Object Literals. 
</span><br>
- <span style="font-family:Courier New; font-size:15px;color:rgb(160, 90, 113)"> Document Object Model. 
</span><br>
---
<span style="font-family:Courier New; font-size:25px;color:rgb(250, 179, 113)"> Object Literals </span><br>
<span style="font-family:Courier New; font-size:15px;color:rgb(200, 179, 113)">WHAT IS AN OBJECT?</span><br>
<span style="font-family:Courier New; font-size:15px;color:rgb(200, 179, 113)">Objects group together a set of variables and functions to create a model of a something you would recognize from the real world. In an object, variables and functions take on new names.</span> <br>
- <span style="font-family:Courier New; font-size:15px;color:rgb(200, 179, 113)">IN AN OBJECT: VARIABLES BECOME KNOWN AS PROPERTIES <br>If a variable is part of an object, it is called a property. Properties tell us about the object, such as
the name of a hotel or the number of rooms it has. Each individual hotel might have a different name and a different number of rooms.</span><br>
- <span style="font-family:Courier New; font-size:15px;color:rgb(200, 179, 113)">IN AN OBJECT: FUNCTIONS BECOME KNOWN AS METHODS<br>
If a function is part of an object, it is called a method. Methods represent tasks that are associated with the object. For example, you can check how many rooms are available by subtracting the number of booked rooms from the total number of rooms.</span><br>

<span style="font-family:Courier New; font-size:15px;color:rgb(200, 179, 113)">Ther is two way to create an object.</span><br>
- <span style="font-family:Courier New; font-size:15px;color:rgb(200, 179, 113)">Literal Notation</span><br>

    - ![LiteralNotation](https://raw.githubusercontent.com/shadykh/reading-notes/main/Code201/assets/LiteralNotation.PNG)<br><br>

- <span style="font-family:Courier New; font-size:15px;color:rgb(200, 179, 113)">Constructor Notation</span><br>

    - ![ConstructorNotation](https://raw.githubusercontent.com/shadykh/reading-notes/main/Code201/assets/ConstructorNotation.PNG)<br><br>

---
<span style="font-family:Courier New; font-size:25px;color:rgb(160, 90, 113)"> Document Object Model </span><br>
<span style="font-family:Courier New; font-size:15px;color:rgb(160, 90, 113)"> The Document Object Model (DOM) specifies how browsers should create a model of an HTML page and how JavaScript can access and update the
contents of a web page while it is in the browser window.
</span> <br>
> <span style="font-family:Courier New; font-size:15px;color:rgb(160, 90, 113)">The DOM is neither part of HTML, nor part of JavaScript; it is a separate set of rules.</span><br>

<span style="font-family:Courier New; font-size:15px;color:rgb(160, 90, 113)">It is implemented by all major browser makers, and covers two primary areas:</span><br>

- ![2dom](https://raw.githubusercontent.com/shadykh/reading-notes/main/Code201/assets/2dom.PNG)<br><br>

<span style="font-family:Courier New; font-size:15px;color:rgb(160, 90, 113)">THE DOM TREE IS A
MODEL OF A WEB PAGE</span><br>
<span style="font-family:Courier New; font-size:15px;color:rgb(160, 90, 113)">As a browser loads a web page, it creates a model of that page. The model is called a DOM tree, and it is stored in the browsers' memory. It consists of four main types of nodes.<br>
Each node is an object with methods and properties.
Scripts access and update this DOM tree (not the source HTML file).
Any changes made to the DOM tree are reflected in the browser.
</span><br>

- ![domtree](https://raw.githubusercontent.com/shadykh/reading-notes/main/Code201/assets/domtree.PNG)<br><br>

<span style="font-family:Courier New; font-size:15px;color:rgb(160, 90, 113)">WORKING WITH THE DOM TREE</span><br>
- <span style="font-family:Courier New; font-size:15px;color:rgb(160, 90, 113)">Step one:ACCESS THE ELEMENTS. <br></span>
    - ![step1](https://raw.githubusercontent.com/shadykh/reading-notes/main/Code201/assets/step1.PNG)<br><br>
- <span style="font-family:Courier New; font-size:15px;color:rgb(160, 90, 113)">Step two: WORK WITH THOSE ELEMENTS.<br></span>
    - ![step2](https://raw.githubusercontent.com/shadykh/reading-notes/main/Code201/assets/step2.PNG)<br><br>

<span style="font-family:Courier New; font-size:15px;color:rgb(160, 90, 113)">NODELISTS: DOM QUERIES THAT RETURN MORE THAN ONE ELEMENT<br>
When a DOM method can return more than one element, it returns a Nodelist (even if it only finds one matching element).<br>Here you can see four different DOM queries that all return a Nodelist. For each query, you can see the elements and their index numbers in the Nodelist that is returned.</span><br>

-  ![nodegit](https://raw.githubusercontent.com/shadykh/reading-notes/main/Code201/assets/nodegit.PNG)<br><br>

<span style="font-family:Courier New; font-size:15px;color:rgb(160, 90, 113)">LOOPING THROUGH A NODELIST</span><br>

-  ![loopnode](https://raw.githubusercontent.com/shadykh/reading-notes/main/Code201/assets/loopnode.PNG)<br><br>

<span style="font-family:Courier New; font-size:15px;color:rgb(160, 90, 113)">TRAVERSING THE DOM<br>When you have an element node, you can select another element in relation to it using these five properties. This is known as traversing the DOM.</span><br>

-  ![TRAVERSING](https://raw.githubusercontent.com/shadykh/reading-notes/main/Code201/assets/TRAVERSING.PNG)<br><br>

<span style="font-family:Courier New; font-size:15px;color:rgb(160, 90, 113)">WHITESPACE NODES<br>Traversing the DOM can be difficult because some browsers add a text node whenever they come across whitespace between elements.</span><br>

-  ![WHITESPACE](https://raw.githubusercontent.com/shadykh/reading-notes/main/Code201/assets/WHITESPACE.PNG)<br><br>

---
<br>

[<img src="assets/main.gif">](README)
<br>

| <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)"> **Read** </span> |  <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)"> **Title** </span>  |   <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)"> **ToGo** </span>  |
| ----------- | ----------- | ----------- |
| <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)"> Read: 01 </span>      | <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)"> Introductory HTML and JavaScript </span>       |[<img src="assets/taphere.gif">](class-01)|
| <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)"> Read: 02 </span>      | <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)"> HTML Text, CSS Introduction, and Basic JavaScript Instructions </span>       |[<img src="assets/taphere.gif">](class-02)|
| <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)"> Read: 03 </span>      | <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)"> HTML Lists, CSS Boxes, JS Control Flow </span>       |[<img src="assets/taphere.gif">](class-03)|
| <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)"> Read: 04 </span>      | <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)"> HTML Links, CSS Layout, JS Functions </span>       |[<img src="assets/taphere.gif">](class-04)|
| <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)"> Read: 05 </span>      | <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)"> HTML Images; CSS Color & Text </span>       |[<img src="assets/taphere.gif">](class-05)|
| <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)"> Read: 06 </span>      | <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)"> JS Object Literals; The DOM </span>       |[<img src="assets/taphere.gif">](class-06)|
| <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)"> Read: 07 </span>      | <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)"> HTML Tables; JS Constructor Functions </span>       |[<img src="assets/uc.gif">](UC)|
| <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)"> Read: 08 </span>      | <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)"> More CSS Layout </span>       |[<img src="assets/uc.gif">](UC)|
| <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)"> Read: 09 </span>      | <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)"> Forms and Events </span>       |[<img src="assets/uc.gif">](UC)|
| <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)"> Read: 10 </span>      | <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)"> JS Debugging </span>       |[<img src="assets/uc.gif">](UC)|
| <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)"> Read: 11 </span>      | <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)"> Assorted Topics </span>       |[<img src="assets/uc.gif">](UC)|
| <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)"> Read: 12 </span>      | <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)"> Docs for the HTML canvas Element & Chart.js </span>       |[<img src="assets/uc.gif">](UC)|
| <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)"> Read: 13 </span>      | <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)"> Local Storage </span>       |[<img src="assets/uc.gif">](UC)|
| <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)"> Read: 14a </span>      | <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)"> CSS Transforms, Transitions, and Animations </span>       |[<img src="assets/uc.gif">](UC)|
| <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)"> Read: 14b </span>      | <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)"> What Google Learned About Teams </span>       |[<img src="assets/uc.gif">](UC)|
<br>

---
| <span style="font-family:Courier New; font-size:13px;color:rgb(60, 179, 113)"> **Number** </span> |  <span style="font-family:Courier New; font-size:13px;color:rgb(60, 179, 113)"> **References** </span>  |
| ----------- | ----------- |
| <span style="font-family:Courier New; font-size:13px;color:rgb(60, 179, 113)"> [] </span>      | <span style="font-family:Courier New; font-size:13px;color:rgb(60, 179, 113)"> Duckett, J. (2014). JavaScript &amp; jQuery ; HTML &amp; CSS. In JavaScript &amp; jQuery ; HTML &amp; CSS . Indianapolis, IN: John Wiley &amp; Sons. </span>       |