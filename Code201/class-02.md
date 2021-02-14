<img src="https://asac.ltuc.com/wp-content/themes/asac/images/logo.png" alt="Kitten"
	title="LTUC-Abdul Aziz Al Ghurair School of Advanced Computing" width="200" />  &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; <span style="font-family:Papyrus; font-size:25px;color:rgb(60, 179, 113)">**Welcome to Read: 02**</span>

---
<br>

<span style="font-family:Courier New; font-size:20px;color:rgb(60, 179, 113)"> **Read: 02 "HTML Text, CSS Introduction, and Basic JavaScript Instructions"** </span>


<span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)">In this Read: 02, I will talk about those topics: 
</span>
- <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)">Text.
</span> 
- <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)"> Introducing CSS. 
</span>
- <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)">Basic JavaScript Instructions. 
</span> 
- <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)">Decisions and Loops. 
</span> 
<br>

<span style="font-family:Courier New; font-size:20px;color:rgb(60, 179, 113)">**Text** </span>
<span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)"><br>
 When you are ready to build up your page you will write some texts, and those text should be stylized to be more attractive for the user to read it.<br><br>
 So, what are the main concepts here?<br>
 **Structural markup:** the elements that you can use to describe both headings and paragraphs.
**Semantic markup:** which provides extra information; such as where emphasis is placed in a sentence, that something you have written is a quotation.[1] <br><br>
</span> 

<span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)">**Structural markup** <br>
We have many structural markup in the Html and CSS, we will mention some of them here.</span> 
- <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)">Headings <br>
	- We use the letter h with numbers from 1 to 6, to style the header.(`<h1>`,`<h2>`,`<h2>`,`<h4>`,`<h5>` and `<h6>`) <br>

		```
		<h1> This is h1 header </h1>
		```
		><h1>This is h1 header </h1>

		```
		<h6> This is h6 header </h6>
		```
		><h6> This is h6 header </h6>
</span> 
<br>

- <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)">Paragraphs <br>
	- We use the `<p>` tag for the paragraph.<br>
	
		```
		<p>
		This is a paragraph
		</p>
		```
	</span> 

- <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)">Bold & Italic <br>
	- We use the `<b>` for **Bold** and `<i>` for *Italic*.</span> 
<br>

<span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)">**Semantic markup** <br>
We have many Semantic markup in the Html and CSS, we will mention some of them here.</span> 

- <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)"> Strong and Emphasis <br>
	- We use the `<strong>` tag to indicate that its
content has strong importance. 
		```
		<strong>
		This is a important text.
		</strong>
		```
		> **This is a important text.**
	- We use `<em>` tag to indicate emphasis that subtly changes the meaning of a sentence.[2]
		```
		<em>
		This is demo
		</em>
		```
		> *This is demo*

</span> 

- <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)"> Quotations <br>
	- We use the `<blockquote>` for longer quotes that take up an entire paragraph.[3]
		```
		<blockquote>
		<p>
		This is a blockquote
		</p>
		</blockquote>
		```
		>This is a blockquote
	- We use the `<q>`  or shorter quotes that sit within a paragraph.[4]
		```
		<p>
		This is <q>a short quote</q>
		</p>
		```
		>This is "a Short quote"
</span> 
---
<br>

<span style="font-family:Courier New; font-size:20px;color:rgb(60, 179, 113)">**Introducing CSS** </span>
<span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)"><br>
 When you bulit your html page, you of course want it to look good when someone visit it, so here come the CSS. <br><br>
 CSS allows you to create rules that specify how the content of an element should appear.[5]
</span> 
- <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)"> We will show you a brief of CSS elemnts:

		```
		p {
			font-family:Courier New; 
		}
		```
	> p is the selector.<br>
	> {} between them is the declaration.<br>
	> font-family is a property.<br>
	> Courier New is a value.
</span> 
- <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)"> You can use CSS externally or internally:<br>
	- <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)"> Externally:<br>

		```
		<link href="css/styles.css" type="text/css"
		rel="stylesheet" />
		```
		>`<link>` element can be used in an HTML document to tell the browser where to find the CSS file used to style the page.[6]<br>
		>`href` This specifies the path to the CSS file.<br>
		>`type` This attribute specifies the type of document 	being linked to.[6]<br>
		>`rel` This specifies the relationship between the HTML page and the file it is linked to.[6]<br>
</span> 
	- <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)"> Internally:<br>


		```
		<style>
		font-family:Courier New; 
		font-size:15px;
		</style>
		```
		>`<style>` include CSS rules within an HTML page, which usually sits inside the `<head>` element of the page.
</span> 
- <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)">There are many way to select element to apply the CSS on them, they called selector[7]:<br>

![Selector](assets/selector.png)
<br>
---
<span style="font-family:Courier New; font-size:20px;color:rgb(60, 179, 113)">**Basic JavaScript Instructions** </span>
<span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)"><br>
 Now to make your page live and it can interact with the user, you should use JavaScript.<br><br>
 JavaScript is a text-based programming language used both on the client-side and server-side that allows you to make web pages interactive. Where HTML and CSS are languages that give structure and style to web pages, JavaScript gives web pages interactive elements that engage a user.[8]<br><br>
In the js we have a lot of concepts that we used here. So, we will mention some of them.
</span> <br>
- <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)"> Statements:<br>
A script is a series of instructions that a computer can follow one-by-one.
Each individual instruction or step is known as a statement.
Statements should end with a semicolon.[9]
</span> 
<br>
- <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)"> Comments:<br>
You should write comments to explain what your code does.
They help make your code easier to read and understand.
This can help you and others who read your code.[10]
</span> <br>
- <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)"> Variable:<br>
A script will have to temporarily store the bits of information it needs to do its job. It can store this data in variables.[11]
	- `var name = "Shady";`
		> name is the variable here, which contain the string value `"Shady"`<br>

	- <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)">There is six rules to name the variables are shown below.
<br>

![Naming](https://github.com/shadykh/reading-notes/blob/main/Code201/assets/naming.PNG?raw=true)

</span>

- <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)"> Data Types:<br>
JavaScript distinguishes between numbers, strings, and true or false values known as Booleans.[12]
	- Numeric: `var num = 5;`
	- String: var name = "Shady";`
	- Boolean: `var checkIf = true;`
</span> <br>
- <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)"> Arrays:<br>
An array is a special type of variable. It doesn't
just store one value; it stores a list of values.[13]
	- Creating an array:<br>
		```
		var colors;
		colors = ['white', 'black'];
		```
	- Accessing items in an array:<br>
		```
		var itemThr ee;
		itemTwo = colors [1] ;
		```
	- Number of items in an array:<br> 
		```
		var numColors ;
		numColors = colors.length;
		```
</span> <br>
- <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)"> Expressions:<br>
An expression evaluates into (results in) a single value. Broadly speaking there are two types of expressions.[14]
	- Expressions that just assign a value to a variable:<br>
		```
		var color = 'blue';
		```
	- Expressions that use two or more values to return a single value:<br>
		```
		var speed = 5 * 6;
		```
</span> <br>
- <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)"> Operators:<br>
Expressions rely on things called operators; they allow programmers to create a single value from one or more values.[15]
<br>

![Operators](assets/operators.png)
</span> <br>
---
<span style="font-family:Courier New; font-size:20px;color:rgb(60, 179, 113)">**Decisions and Loops** </span>
<span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)"><br>
The code can take more than one path, which means the
browser runs different code in different situations. Here we will learn how to create and control the flow of
data in the scripts to handle different situations.
</span> <br>
- <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)"> Decisions making:<br>
There are often several places in a script where decisions are made that determine which lines of code should be run next.[16]<br>
There are two components to a decision:
	- An expression is evaluated, which returns a value.
	- A conditional statement say what to do in a given situation.
		```
		If (name == "Shady"){
			alert("Hi",name);
		} else {
			alert("You are not Shady");
		}
		```
		> (name == "Shady") This is the conditional statement.
</span> 
- <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)"> Comparison Operators:<br>
	- Is equal to `(==)` :<br>
	This operator compare two vaules (numbers, string or booleans) to see if they are the same value.
        - `"Good" == "Bad"` , it's false.
	- Is not equal to `(!=)` :<br>
	This operator compare two vaules (numbers, string or booleans) to see if they are not the same value.
        - `"Good" != "Bad" `, it's true.
	- Strict equal to `(===)` :<br>
	This operator compare two vaules (numbers, string or booleans) to see if they are the same value and type.
        - `"Good" === "Bad" `, it's fasle.
	- Strict not equal to `(!==)` :<br>
	This operator compare two vaules (numbers, string or booleans) to see if they are not the same.
        - `"Good" !== "Bad" `, it's true.
	- Greater than `(>)` :<br>
	This operator check if the left side is greater than than the rgiht side.
        - `( 5 > 4 )` , it's true.
	- Less than `(<)` :<br>
	This operator check if the left side is less than than the rgiht side.
        - `( 4 < 5 )`, it's true.
	- Greater than or equal to`(>=)` :<br>
	This operator check if the left side is greater than than or eqaul the rgiht side.
        - `( 5 >= 5 )` , it's true.
	- Less than or equal to `(<=)` :<br>
	This operator check if the left side greater than than or eqaul the rgiht side.
        - `( 4 <= 2 )` , it's true.

</span> <br>
- <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)"> Logical Operators:<br>
	- Logical and `( && )` :<br>
	This operator test more than one condition.
        - `((5 < 5) && (5 >= 5))` , it's false.
	- Logical or `( || )` :<br>
	This operator test at least one condition.
        - `((5 < 5) || (5 >= 5))` , it's true.
	- Logical not `( ! )` :<br>
	This operator takes a single boolean value an invert it.
        - `!(5 >= 5)` , it's fasle.

<span>

---

<br>
---
<br>

[<img src="assets/main.gif">](../README)

<br>

| <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)"> **Read** </span> |  <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)"> **Title** </span>  |   <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)"> **ToGo** </span>  |
| ----------- | ----------- | ----------- |
| <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)"> Read: 01 </span>      | <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)"> Introductory HTML and JavaScript </span>       |[<img src="assets/taphere.gif">](class-01)|
| <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)"> Read: 02 </span>      | <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)"> HTML Text, CSS Introduction, and Basic JavaScript Instructions </span>       |[<img src="assets/taphere.gif">](class-02)|
| <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)"> Read: 03 </span>      | <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)"> HTML Lists, CSS Boxes, JS Control Flow </span>       |[<img src="assets/uc.gif">](UC)|
| <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)"> Read: 04 </span>      | <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)"> HTML Links, CSS Layout, JS Functions </span>       |[<img src="assets/uc.gif">](UC)|
| <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)"> Read: 05 </span>      | <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)"> HTML Images; CSS Color & Text </span>       |[<img src="assets/uc.gif">](UC)|
| <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)"> Read: 06 </span>      | <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)"> JS Object Literals; The DOM </span>       |[<img src="assets/uc.gif">](UC)|
| <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)"> Read: 07 </span>      | <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)"> HTML Tables; JS Constructor Functions </span>       |[<img src="assets/uc.gif">](UC)|
| <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)"> Read: 08 </span>      | <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)"> More CSS Layout </span>       |[<img src="assets/uc.gif">](UC)|
| <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)"> Read: 09 </span>      | <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)"> Forms and Events </span>       |[<img src="assets/uc.gif">](UC)|
| <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)"> Read: 10 </span>      | <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)"> JS Debugging </span>       |[<img src="assets/uc.gif">](UC)|
| <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)"> Read: 11 </span>      | <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)"> Assorted Topics </span>       |[<img src="assets/uc.gif">](UC)|
| <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)"> Read: 12 </span>      | <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)"> Docs for the HTML canvas Element & Chart.js </span>       |[<img src="assets/uc.gif">](UC)|
| <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)"> Read: 13 </span>      | <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)"> Local Storage </span>       |[<img src="assets/uc.gif">](UC)|
| <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)"> Read: 14a </span>      | <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)"> CSS Transforms, Transitions, and Animations </span>       |[<img src="assets/uc.gif">](UC)|
| <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)"> Read: 14b </span>      | <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)"> What Google Learned About Teams </span>       |[<img src="assets/uc.gif">](UC)|

---

| <span style="font-family:Courier New; font-size:13px;color:rgb(60, 179, 113)"> **Number** </span> |  <span style="font-family:Courier New; font-size:13px;color:rgb(60, 179, 113)"> **References** </span>  |
| ----------- | ----------- |
| <span style="font-family:Courier New; font-size:13px;color:rgb(60, 179, 113)"> [1] </span>      | <span style="font-family:Courier New; font-size:13px;color:rgb(60, 179, 113)"> Duckett, J. (2014). JavaScript &amp; jQuery ; HTML &amp; CSS. In JavaScript &amp; jQuery ; HTML &amp; CSS (p. 41). Indianapolis, IN: John Wiley &amp; Sons. </span>       |
| <span style="font-family:Courier New; font-size:13px;color:rgb(60, 179, 113)"> [2] </span>      | <span style="font-family:Courier New; font-size:13px;color:rgb(60, 179, 113)"> Duckett, J. (2014). JavaScript &amp; jQuery ; HTML &amp; CSS. In JavaScript &amp; jQuery ; HTML &amp; CSS (p. 51). Indianapolis, IN: John Wiley &amp; Sons. </span>       |
| <span style="font-family:Courier New; font-size:13px;color:rgb(60, 179, 113)"> [3] </span>      | <span style="font-family:Courier New; font-size:13px;color:rgb(60, 179, 113)"> Duckett, J. (2014). JavaScript &amp; jQuery ; HTML &amp; CSS. In JavaScript &amp; jQuery ; HTML &amp; CSS (p. 52). Indianapolis, IN: John Wiley &amp; Sons. </span>       |
| <span style="font-family:Courier New; font-size:13px;color:rgb(60, 179, 113)"> [4] </span>      | <span style="font-family:Courier New; font-size:13px;color:rgb(60, 179, 113)"> Duckett, J. (2014). JavaScript &amp; jQuery ; HTML &amp; CSS. In JavaScript &amp; jQuery ; HTML &amp; CSS (p. 52). Indianapolis, IN: John Wiley &amp; Sons. </span>       |
| <span style="font-family:Courier New; font-size:13px;color:rgb(60, 179, 113)"> [5] </span>      | <span style="font-family:Courier New; font-size:13px;color:rgb(60, 179, 113)"> Duckett, J. (2014). JavaScript &amp; jQuery ; HTML &amp; CSS. In JavaScript &amp; jQuery ; HTML &amp; CSS (p. 227). Indianapolis, IN: John Wiley &amp; Sons. </span>       |
| <span style="font-family:Courier New; font-size:13px;color:rgb(60, 179, 113)"> [6] </span>      | <span style="font-family:Courier New; font-size:13px;color:rgb(60, 179, 113)"> Duckett, J. (2014). JavaScript &amp; jQuery ; HTML &amp; CSS. In JavaScript &amp; jQuery ; HTML &amp; CSS (p. 235). Indianapolis, IN: John Wiley &amp; Sons. </span>       |
| <span style="font-family:Courier New; font-size:13px;color:rgb(60, 179, 113)"> [7] </span>      | <span style="font-family:Courier New; font-size:13px;color:rgb(60, 179, 113)"> Duckett, J. (2014). JavaScript &amp; jQuery ; HTML &amp; CSS. In JavaScript &amp; jQuery ; HTML &amp; CSS (p. 238). Indianapolis, IN: John Wiley &amp; Sons. </span>       |
| <span style="font-family:Courier New; font-size:13px;color:rgb(60, 179, 113)"> [8] </span>      | <span style="font-family:Courier New; font-size:13px;color:rgb(60, 179, 113)"> Duckett, J. (2014). JavaScript &amp; JQuery: Interactive front-end web development. In JavaScript &amp; JQuery: Interactive Front-End Web Development (p. 54). John Wiley &amp; Sons. </span>       |
| <span style="font-family:Courier New; font-size:13px;color:rgb(60, 179, 113)"> [9] </span>      | <span style="font-family:Courier New; font-size:13px;color:rgb(60, 179, 113)"> Duckett, J. (2014). JavaScript &amp; JQuery: Interactive front-end web development. In JavaScript &amp; JQuery: Interactive Front-End Web Development (p. 56). John Wiley &amp; Sons. </span>       |
| <span style="font-family:Courier New; font-size:13px;color:rgb(60, 179, 113)"> [10] </span>      | <span style="font-family:Courier New; font-size:13px;color:rgb(60, 179, 113)"> Duckett, J. (2014). JavaScript &amp; JQuery: Interactive front-end web development. In JavaScript &amp; JQuery: Interactive Front-End Web Development (p. 57). John Wiley &amp; Sons. </span>       |
| <span style="font-family:Courier New; font-size:13px;color:rgb(60, 179, 113)"> [11] </span>      | <span style="font-family:Courier New; font-size:13px;color:rgb(60, 179, 113)"> Duckett, J. (2014). JavaScript &amp; JQuery: Interactive front-end web development. In JavaScript &amp; JQuery: Interactive Front-End Web Development (p. 58). John Wiley &amp; Sons. </span>       |
| <span style="font-family:Courier New; font-size:13px;color:rgb(60, 179, 113)"> [12] </span>      | <span style="font-family:Courier New; font-size:13px;color:rgb(60, 179, 113)"> Duckett, J. (2014). JavaScript &amp; JQuery: Interactive front-end web development. In JavaScript &amp; JQuery: Interactive Front-End Web Development (p. 62). John Wiley &amp; Sons. </span>       |
| <span style="font-family:Courier New; font-size:13px;color:rgb(60, 179, 113)"> [13] </span>      | <span style="font-family:Courier New; font-size:13px;color:rgb(60, 179, 113)"> Duckett, J. (2014). JavaScript &amp; JQuery: Interactive front-end web development. In JavaScript &amp; JQuery: Interactive Front-End Web Development (p. 70). John Wiley &amp; Sons. </span>       |
| <span style="font-family:Courier New; font-size:13px;color:rgb(60, 179, 113)"> [14] </span>      | <span style="font-family:Courier New; font-size:13px;color:rgb(60, 179, 113)"> Duckett, J. (2014). JavaScript &amp; JQuery: Interactive front-end web development. In JavaScript &amp; JQuery: Interactive Front-End Web Development (p. 74). John Wiley &amp; Sons. </span>       |
| <span style="font-family:Courier New; font-size:13px;color:rgb(60, 179, 113)"> [15] </span>      | <span style="font-family:Courier New; font-size:13px;color:rgb(60, 179, 113)"> Duckett, J. (2014). JavaScript &amp; JQuery: Interactive front-end web development. In JavaScript &amp; JQuery: Interactive Front-End Web Development (p. 75). John Wiley &amp; Sons. </span>       |
| <span style="font-family:Courier New; font-size:13px;color:rgb(60, 179, 113)"> [16] </span>      | <span style="font-family:Courier New; font-size:13px;color:rgb(60, 179, 113)"> Duckett, J. (2014). JavaScript &amp; JQuery: Interactive front-end web development. In JavaScript &amp; JQuery: Interactive Front-End Web Development (p. 148). John Wiley &amp; Sons. </span>       |