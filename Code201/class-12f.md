<img src="https://asac.ltuc.com/wp-content/themes/asac/images/logo.png" alt="Kitten"
	title="LTUC-Abdul Aziz Al Ghurair School of Advanced Computing" width="200" />  &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; <span style="font-family:Papyrus; font-size:25px;color:rgb(60, 179, 113)">**Welcome to Read: 12**</span><br>

---

<br>

<span style="font-family:Courier New; font-size:20px;color:rgb(60, 179, 113)"> **Read: 12 - "Docs for the HTML `<canvas>` Element & Chart.js"** </span> <br>

<span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)">In this Read: 12, I will talk only about: 
</span><br>
- <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)"> Chart.</span><br><br>


---

<br><br>

<span style="font-family:Courier New; font-size:25px;color:rgb(60, 179, 113)"> Chart </span><br>
<span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)">What is the Chart?</span><br>
<span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)"> JCharts are far better for displaying data visually than tables and have the added benefit that no one is ever going to press-gang them into use as a layout tool. They’re easier to look at and convey data quickly, but they’re not always easy to create. <br>
A great way to get started with charts is with Chart.js, a JavaScript plugin that uses HTML5’s canvas element to draw the graph onto the page. It’s a well documented plugin that makes using all kinds of bar charts, line charts, pie charts and more, incredibly easy.</span> <br>

- <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)">Setting up</span><br>

    ![drawing](https://raw.githubusercontent.com/shadykh/reading-notes/main/Code201/assets/drawing.PNG)<br><br>

- <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)">Drawing a line chart</span><br>

    ![drawCan](https://raw.githubusercontent.com/shadykh/reading-notes/main/Code201/assets/drawCan.PNG)<br><br>
    ![line](https://raw.githubusercontent.com/shadykh/reading-notes/main/Code201/assets/line.PNG)<br><br>

- <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)">Drawing a pie chart</span><br>

    ![pie1](https://raw.githubusercontent.com/shadykh/reading-notes/main/Code201/assets/pie1.PNG)<br><br>
    ![pie2](https://raw.githubusercontent.com/shadykh/reading-notes/main/Code201/assets/pie2.PNG)<br><br>
    
> For more information please see the reference [1].

---

<br><br>

<span style="font-family:Courier New; font-size:25px;color:rgb(60, 179, 113)"> The `<canvas>` element </span><br>
<span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)"> At first sight a `<canvas>` looks like the `<img>` element, with the only clear difference being that it doesn't have the src and alt attributes. Indeed, the `<canvas>` element has only two attributes, width and height. These are both optional and can also be set using DOM properties. When no width and height attributes are specified, the canvas will initially be 300 pixels wide and 150 pixels high. The element can be sized arbitrarily by CSS, but during rendering the image is scaled to fit its layout size: if the CSS sizing doesn't respect the ratio of the initial canvas, it will appear distorted.</span> <br>

- <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)">Fallback content</span><br>
    - <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)">The `<canvas>` element differs from an `<img>` tag in that, like for `<video>`, `<audio>`, or `<picture>` elements, it is easy to define some fallback content, to be displayed in older browsers not supporting it, like versions of Internet Explorer earlier than version 9 or textual browsers. You should always provide fallback content to be displayed by those browsers. <br>
    Providing fallback content is very straightforward: just insert the alternate content inside the `<canvas>` element. Browsers that don't support `<canvas>` will ignore the container and render the fallback content inside it. Browsers that do support `<canvas>` will ignore the content inside the container, and just render the canvas normally.</span><br>

- <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)">Required `</canvas>` tag</span><br>
    - <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)">As a consequence of the way fallback is provided, unlike the `<img>` element, the `<canvas>` element requires the closing tag (`</canvas>`). If this tag is not present, the rest of the document would be considered the fallback content and wouldn't be displayed. <br> If fallback content is not needed, a simple `<canvas id="foo" ...></canvas>` is fully compatible with all browsers that support canvas at all.</span><br>

> For more information please see the references [2].

---

<br><br>

<span style="font-family:Courier New; font-size:25px;color:rgb(60, 179, 113)"> Drawing shapes with canvas </span><br>


- <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)">The grid</span><br>

    ![grid](https://raw.githubusercontent.com/shadykh/reading-notes/main/Code201/assets/grid.PNG)<br><br>

- <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)">Drawing rectangles</span><br>

    ![drawrec](https://raw.githubusercontent.com/shadykh/reading-notes/main/Code201/assets/drawrec.PNG)<br><br>

 - <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)">Rectangular shape example</span><br>

    ![recexa](https://raw.githubusercontent.com/shadykh/reading-notes/main/Code201/assets/recexa.PNG)<br><br>   

> For more information please see the references [3].


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
| <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)"> Read: 07 </span>      | <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)"> HTML Tables; JS Constructor Functions </span>       |[<img src="assets/taphere.gif">](class-07)|
| <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)"> Read: 08 </span>      | <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)"> More CSS Layout </span>       |[<img src="assets/taphere.gif">](class-08)|
| <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)"> Read: 09 </span>      | <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)"> Forms and Events </span>       |[<img src="assets/taphere.gif">](class-09)|
| <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)"> Read: 10 </span>      | <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)"> JS Debugging </span>       |[<img src="assets/taphere.gif">](class-10)|
| <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)"> Read: 11 </span>      | <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)"> Assorted Topics </span>       |[<img src="assets/taphere.gif">](class-11)|
| <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)"> Read: 12 </span>      | <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)"> Docs for the HTML canvas Element & Chart.js </span>       |[<img src="assets/taphere.gif">](class-12)|
| <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)"> Read: 13 </span>      | <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)"> Local Storage </span>       |[<img src="assets/uc.gif">](UC)|
| <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)"> Read: 14a </span>      | <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)"> CSS Transforms, Transitions, and Animations </span>       |[<img src="assets/uc.gif">](UC)|
| <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)"> Read: 14b </span>      | <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)"> What Google Learned About Teams </span>       |[<img src="assets/uc.gif">](UC)|



---
<br>

| <span style="font-family:Courier New; font-size:13px;color:rgb(60, 179, 113)"> **Number** </span> |  <span style="font-family:Courier New; font-size:13px;color:rgb(60, 179, 113)"> **References** </span>  |
| ----------- | ----------- |
| <span style="font-family:Courier New; font-size:13px;color:rgb(60, 179, 113)"> [1] </span>      | <span style="font-family:Courier New; font-size:13px;color:rgb(60, 179, 113)"> https://www.webdesignerdepot.com/2013/11/easily-create-stunning-animated-charts-with-chart-js/ </span>       |
| <span style="font-family:Courier New; font-size:13px;color:rgb(60, 179, 113)"> [2] </span>      | <span style="font-family:Courier New; font-size:13px;color:rgb(60, 179, 113)"> https://developer.mozilla.org/en-US/docs/Web/API/Canvas_API/Tutorial/Basic_usage </span>       |
| <span style="font-family:Courier New; font-size:13px;color:rgb(60, 179, 113)"> [3] </span>      | <span style="font-family:Courier New; font-size:13px;color:rgb(60, 179, 113)"> https://developer.mozilla.org/en-US/docs/Web/API/Canvas_API/Tutorial/Drawing_shapes </span>       |