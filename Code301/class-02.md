<img src="https://asac.ltuc.com/wp-content/themes/asac/images/logo.png" alt="Kitten"
	title="LTUC-Abdul Aziz Al Ghurair School of Advanced Computing" width="200" />  &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; <span style="font-family:Papyrus; font-size:25px;color:rgb(60, 179, 113)">**Welcome to Read: 02**</span>

---
<br>

<span style="font-family:Courier New; font-size:20px;color:rgb(60, 179, 113)"> **jQuery, Events, and The DOM** </span>


<span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)">In this Read: 02, I will talk about those topics: 
</span>
- <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)">Pair Programming.
</span> 
- <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)"> jQuery. 
</span>
<br>

<span style="font-family:Courier New; font-size:20px;color:rgb(60, 179, 113)">**Pair Programming** </span>
<span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)"><br>
Pair programming touches on all four skills: developers explain out loud what the code should do, listen to others’ guidance, read code that others have written, and write code themselves. <br>
During a five-hour paired lab session, Code Fellows students work on all four of these language-specific skills. The abilities they foster will serve them well in completing assignments, in their own communication and learning, in interviews, and in readiness for a job at a company that utilizes this agile practice. <br><br>
</span> 

- <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)">Why pair program?</span><br>

    - <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)">Greater efficiency</span><br>

    - <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)">Engaged collaboration</span><br>

    - <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)">Learning from fellow students</span><br>

    - <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)">Social skills</span><br>

    - <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)">Job interview readiness</span><br>

    - <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)">Work environment readiness</span><br>

---

<span style="font-family:Courier New; font-size:20px;color:rgb(60, 179, 113)">**jQuery** </span> <br>
<span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)"><br>**jQuery** offers a simple way to achieve a variety of common JavaScript tasks quickly and consistently, across all major
browsers and without any fallback code needed..<br><br>
</span> 

- <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)">WHY USE JQUERY?</span><br>

    - <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)">SIMPLE SELECTORS</span><br>

    - <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)">COMMON TASKS IN LESS CODE</span><br>

    - <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)">CROSS-BROWSER COMPATIBILITY</span><br>

- <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)">jQuery's motto is "Write less, do more," because it allows you to achieve the same goals but in fewer lines of code than you would need to write with plain JavaScript.</span><br>

- <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)">GETTING ELEMENT CONTENT</span><br>

    - <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)"> `.html()` When this method is used to retrieve information from a jQuery selection, it retrieves only the HTML
    inside the first element in the matched set, along with any of its descendants. </span> 

    - <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)"> `.text()` When this method is used to retrieve the text from a jQuery selection, it returns the content from every element in the jQuery selection, along with the text from any descendants. </span> 


- <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)">UPDATING ELEMENTS</span><br>

    - <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)"> `.html()` This method gives every element in the matched set the same new content. The new content may include HTML. </span> 

    - <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)"> `.text()` This method gives every element in the matched set the same new text content. Any markup would be shown as text. </span> 

    - <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)"> `.replaceWith()` This method replaces every element in a matched set with new content. It also returns the replaced elements.</span> 

    - <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)"> `.remove()` This method removes all of the elements in the matched set.</span> 


- <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)">INSERTING ELEMENTS</span><br>
<span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)">Inserting new elements involves two steps:<br></span>
    - <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)">Create the new elements in a jQuery object.<br> </span> 
        - <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)">The following statement creates a variable called $newFragment and stores a jQuery object in it. The jQuery object is set to contain an empty. <br> 
        `<li>element:var $newFragment = $('<li>'};`</span> 
    - <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)">Use a method to insert the content into the page.</span>
        - <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)">`.before()` This method inserts content before the selected element(s) .</span> 
        - <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)">`.after()` This method inserts content after the selected element(s).</span> 
        - <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)">`.prepend()` This method inserts content inside the selected element(s), after the opening tag</span> 
        - <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)">`.append()` This method inserts content inside the selected element(s), before the closing tag.</span> 


> For further infromation please see the : **avaScript and jQuery book by Jon Duckett**

---

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






