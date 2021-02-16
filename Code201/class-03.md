<img src="https://asac.ltuc.com/wp-content/themes/asac/images/logo.png" alt="Kitten"
	title="LTUC-Abdul Aziz Al Ghurair School of Advanced Computing" width="200" />  &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; <span style="font-family:Papyrus; font-size:25px;color:rgb(60, 179, 113)">**Welcome to Read: 03**</span>

---
<br>

<span style="font-family:Courier New; font-size:20px;color:rgb(60, 179, 113)"> **Read: 03 "HHTML Lists, CSS Boxes, JS Control Flow"** </span>

<span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)">In this Read: 02, I will talk about those topics: 
</span>
- <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)">Lists.
</span> 
- <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)"> Boxes. 
</span>
- <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)">Decisions and Loops. 
</span> 
<br>

<span style="font-family:Courier New; font-size:20px;color:rgb(60, 179, 113)">**Lists**<br> </span>
<span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)"> When you want to go to the mall to buy your monthly stuff for your home, your write down those stuffs on paper as a list of stuffs.<br><br>
Why you do that? Because lists make the things more organized and ordered. And here in html we have three types of lists.<br></span>

- <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)">**Ordered lists:** are lists where each item in the list is
numbered (there are a characters that indicate order).<br></span> 
    - It starts with `<ol>` tag to open a list, then you use `<li>` tag to put your items there.
      ```
      <ol>
        <li>Fisrt item</li>
        <li>Second item</li>
        <li>Third item</li>
      </ol>
       ```
- <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)">**Unordered lists:** are lists that begin with a bullet point.<br></span> 
    - It starts with `<ul>` tag to open a list, then you use `<li>` tag to put your items there.
      ```
      <ul>
        <li>Fisrt item</li>
        <li>Second item</li>
        <li>Third item</li>
      </ul>
       ```
- <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)">**Definition lists:** are made up of a set of terms along with the definitions for each of those terms.[1]<br></span> 
    - It starts with `<dl>` tag to open a list, then you use `<dt>`to contain the term being defined (the definition term) and use `<dd>`to contain the definition.
      ```
      <dl>
        <dt>Html</dt>
        <dd> Is the standard markup language for Web pages. </dd>
      </dl>
       ```
- <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)">**Nested lists:** are made up of a list inside list.<br></span>
    - An example
      ```
      <ul>
        <li>Fisrt item</li>
        <li>Second item</li>
        <ul>
            <li>First</li>
            <li>Second</li>
        </ul>
      </ul>
       ```
---
<span style="font-family:Courier New; font-size:20px;color:rgb(60, 179, 113)">**Boxes** </span>
<span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)"><span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)"><br>
In the CSS, if you want to do some styling at heading for example, it deals with them as box levels, make a heading as a box. Those boxes we can do some styling and setting for them, here we will have some of them.<br></span>
- <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)">**Box Dimensions:** width, height. <br></span>

    ```
        div.box {
        height: 250px;
        width: 250px;
        background-color: #black;}
    ```
- <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)">**Border, margin& Padding**. <br></span>
![border](https://blog.hubspot.com/hs-fs/hubfs/dyno-mapper-sitemap-generator.png?width=566&name=dyno-mapper-sitemap-generator.png)
![margin](https://blog.hubspot.com/hs-fs/hubfs/dyno-mapper-sitemap-generator.png?width=566&name=dyno-mapper-sitemap-generator.png)
<br>
> For more information please see the Duckett, J. (2014). JavaScript &amp; jQuery ; HTML &amp; CSS. In JavaScript &amp; jQuery ; HTML &amp; CSS (p.300-329). Indianapolis, IN: John Wiley &amp; Sons.
---

<span style="font-family:Courier New; font-size:20px;color:rgb(60, 179, 113)">**Decisions and Loops: Switch**<br> </span>
<span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)"> A switch statement starts with a variable called the switch value. Each case indicates a possible value for this variable and the code that should run if the variable matches that value.[2]<br><br>
Here we will have an example from a lab was done by me.<br></span>

```
let aeroEng = prompt('The first question: Is Shady Enginner?','yes/no,y/n');

switch (aeroEng.toLowerCase()) {
case 'yes':
  alert('Yes \''+ userName + '\' your answer is correct, Shady is an Aeronautical Engineer.');
  //console.log('Answer for Q1: yes \'',userName,'\' your answer is correct, Shady is an Aeronautical Engineer.');
  break;
case 'y':
  alert('Yes \''+ userName + ' your answer is correct, Shady is an Aeronautical Engineer.');
  //console.log('Answer for Q1: yes \'',userName,'\' your answer is correct, Shady is an Aeronautical Engineer.');
  break;
default:
  alert('What is the wrong \''+ userName + '\' you do not answer with yes/no! Please, stick with the rules');
  break;
}
```
> Here if the user enter 'yes', we will enter the **switch**, and check the cases; case by case, when the first one apply, we enter it and run the statments inside that case.<br>

---
<br>

[<img src="assets/main.gif">](../README)

<br>


| <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)"> **Read** </span> |  <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)"> **Title** </span>  |   <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)"> **ToGo** </span>  |
| ----------- | ----------- | ----------- |
| <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)"> Read: 01 </span>      | <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)"> Introductory HTML and JavaScript </span>       |[<img src="assets/taphere.gif">](class-01)|
| <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)"> Read: 02 </span>      | <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)"> HTML Text, CSS Introduction, and Basic JavaScript Instructions </span>       |[<img src="assets/taphere.gif">](class-02)|
| <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)"> Read: 03 </span>      | <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)"> HTML Lists, CSS Boxes, JS Control Flow </span>       |[<img src="assets/taphere.gif">](class-03)|
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
| <span style="font-family:Courier New; font-size:13px;color:rgb(60, 179, 113)"> [1] </span>      | <span style="font-family:Courier New; font-size:13px;color:rgb(60, 179, 113)"> Duckett, J. (2014). JavaScript &amp; jQuery ; HTML &amp; CSS. In JavaScript &amp; jQuery ; HTML &amp; CSS (p. 63). Indianapolis, IN: John Wiley &amp; Sons. </span>       |
| <span style="font-family:Courier New; font-size:13px;color:rgb(60, 179, 113)"> [2] </span>      | <span style="font-family:Courier New; font-size:13px;color:rgb(60, 179, 113)"> Duckett, J. (2014). JavaScript &amp; JQuery: Interactive front-end web development. In JavaScript &amp; JQuery: Interactive Front-End Web Development (p. 164). John Wiley &amp; Sons. </span>       |