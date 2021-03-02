<img src="https://asac.ltuc.com/wp-content/themes/asac/images/logo.png" alt="Kitten"
	title="LTUC-Abdul Aziz Al Ghurair School of Advanced Computing" width="200" />  &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; <span style="font-family:Papyrus; font-size:25px;color:rgb(60, 179, 113)">**Welcome to Read: 14a**</span><br>

---

<br>

<span style="font-family:Courier New; font-size:20px;color:rgb(60, 179, 113)"> **Read: 14a - CSS Transforms, Transitions, and Animations"** </span> <br>

<span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)">In this Read: 14a, I will talk only about: 
</span><br>
- <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)"> CSS Transforms, Transitions, and Animations.</span><br><br>


---

<br><br>

<span style="font-family:Courier New; font-size:25px;color:rgb(60, 179, 113)"> Transforms </span><br>
<span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)">With CSS3 came new ways to position and alter elements. Now general layout techniques can be revisited with alternative ways to size, position, and change elements. All of these new techniques are made possible by the `transform` property. </span> <br>

- <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)">Transform Syntax</span><br>
    * <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)">The actual syntax for the transform property is quite simple, including the transform property followed by the value. The value specifies the transform type followed by a specific amount inside parentheses.</span><br>
    ```
        div {
        -webkit-transform: scale(1.5);
        -moz-transform: scale(1.5);
        -o-transform: scale(1.5);
            transform: scale(1.5);
        }
    ```

- <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)">2D Transforms</span><br>
    * <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)">2D Rotate</span><br>
    ```
        .box-1 {
        transform: rotate(20deg);
        }
        .box-2 {
        transform: rotate(-55deg);
        }

     ```
    ![2drotate](https://raw.githubusercontent.com/shadykh/reading-notes/main/Code201/assets/2drotate.PNG)<br><br>

- <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)">2D Scale</span><br>

    ```
        .box-1 {
        transform: scale(.75);
        }
        .box-2 {
        transform: scale(1.25);
        }

    ```
    ![2dscale](https://raw.githubusercontent.com/shadykh/reading-notes/main/Code201/assets/2dscale.PNG)<br><br>

- <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)">2D Translate</span><br>

    ```
        .box-1 {
        transform: translateX(-10px);
        }
        .box-2 {
        transform: translateY(25%);
        }
        .box-3 {
        transform: translate(-10px, 25%);
        }
    ```
    ![2dTranslate](https://raw.githubusercontent.com/shadykh/reading-notes/main/Code201/assets/2dTranslate.PNG)<br><br>

- <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)">2D Skew</span><br>

        ```
        .box-1 {
        transform: skewX(5deg);
        }
        .box-2 {
        transform: skewY(-20deg);
        }
        .box-3 {
        transform: skew(5deg, -20deg);
        }
        ```
    ![2dSkew](https://raw.githubusercontent.com/shadykh/reading-notes/main/Code201/assets/2dSkew.PNG)<br><br>



> For more information please see the reference [1].

<br>

---

<br><br>

<span style="font-family:Courier New; font-size:25px;color:rgb(60, 179, 113)"> Transitions </span><br>
<span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)">One evolution with CSS3 was the ability to write behaviors for transitions and animations. Front end developers have been asking for the ability to design these interactions within HTML and CSS, without the use of JavaScript or Flash, for years. Now their wish has come true. <br> With CSS3 transitions you have the potential to alter the appearance and behavior of an element whenever a state change occurs, such as when it is hovered over, focused on, active, or targeted. </span> <br>

- <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)">Transitional Properties</span><br>
    * <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)">It is important to note, not all properties may be transitioned, only properties that have an identifiable halfway point. Colors, font sizes, and the alike may be transitioned from one value to another as they have recognizable values in-between one another.<br> A handful of the more popular transitional properties include the following: </span><br>
        ![TransitionalProperties](https://raw.githubusercontent.com/shadykh/reading-notes/main/Code201/assets/TransitionalProperties.PNG)<br><br>       

- <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)">Transition Duration</span><br>

    ```
        .box {
        background: #2db34a;
        border-radius: 6px;
        transition-property: background, border-radius;
        transition-duration: .2s, 1s;
        transition-timing-function: linear;
        }
        .box:hover {
        background: #ff7b29;
        border-radius: 50%;
        }
    ```

- <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)">Transition Timing</span><br>

    ```
    .box {
    background: #2db34a;
    border-radius: 6px;
    transition-property: background, border-radius;
    transition-duration: .2s, 1s;
    transition-timing-function: linear, ease-in;
    }
    .box:hover {
    background: #ff7b29;
    border-radius: 50%;
    }
    ```


- <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)">Transition Delay</span><br>
    ```
    .box {
    background: #2db34a;
    border-radius: 6px
    transition-property: background, border-radius;
    transition-duration: .2s, 1s;
    transition-timing-function: linear, ease-in;
    transition-delay: 0s, 1s;
    }
    .box:hover {
    background: #ff7b29;
    border-radius: 50%;
    }
    ```

> For more information please see the reference [2].

<br>


---

<br><br>

<span style="font-family:Courier New; font-size:25px;color:rgb(60, 179, 113)"> 8 SIMPLE CSS3 TRANSITIONS </span><br>
<span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)">Just a couple of lines of code will give you an awesome transition effect that will excite your users, increase engagement and ultimately, when used well, increase your conversions. What’s more, these effects are hardware accelerated, and a progressive enhancement that you can use right now.<br>Here are 8 really simple effects that will add life to your UI and smiles to your users’ faces. </span> <br>

- <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)">Fade in</span><br>

    ```
    .fade
    {
            opacity:0.5;
    }
    .fade:hover
    {
            opacity:1;
    }
    ```
    ![fadeIn](https://raw.githubusercontent.com/shadykh/reading-notes/main/Code201/assets/fadeIn.PNG)<br><br>

- <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)">Change color</span><br>

    ```
    .color:hover
    {
            background:#53a7ea;
    }
    ```
    ![changeColor](https://raw.githubusercontent.com/shadykh/reading-notes/main/Code201/assets/changeColor.PNG)<br><br>

- <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)">Grow</span><br>

    ```
    .grow:hover
    {
            -webkit-transform: scale(1.3);
            -ms-transform: scale(1.3);
            transform: scale(1.3);
    }
    ```
    ![grow](https://raw.githubusercontent.com/shadykh/reading-notes/main/Code201/assets/grow.PNG)<br><br>

- <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)">Rotate elements</span><br>

    ```
    .rotate:hover
    {
            -webkit-transform: rotateZ(-30deg);
            -ms-transform: rotateZ(-30deg);
            transform: rotateZ(-30deg);
    }
    ```
    ![rotate](https://raw.githubusercontent.com/shadykh/reading-notes/main/Code201/assets/rotate.PNG)<br><br>

- <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)">Square to circle</span><br>

    ```
    .circle:hover
    {
            border-radius:50%;
    }
    ```
    ![SqToCi](https://raw.githubusercontent.com/shadykh/reading-notes/main/Code201/assets/SqToCi.PNG)<br><br>

- <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)">3D shadow</span><br>

    ```
    .threed:hover
    {
            box-shadow:
                    1px 1px #53a7ea,
                    2px 2px #53a7ea,
                    3px 3px #53a7ea;
            -webkit-transform: translateX(-3px);
            transform: translateX(-3px);
    }
    ```
    ![3dShadow](https://raw.githubusercontent.com/shadykh/reading-notes/main/Code201/assets/3dShadow.PNG)<br><br>

- <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)">Inset border</span><br>

    ```
    .border:hover
    {
            box-shadow: inset 0 0 0 25px #53a7ea;
    }
    ```
    ![insetBorder](https://raw.githubusercontent.com/shadykh/reading-notes/main/Code201/assets/insetBorder.PNG)<br><br>


> For more information please see the reference [3].

> Review the following examples on CSS animations of today Read:
> - https://codepen.io/retyui/pen/ByoaXV
> - https://codepen.io/akshaychauhan/pen/oAfae
> - https://codepen.io/kieranfivestars/pen/MYdQxX
> - https://codepen.io/dp_lewis/pen/gCfBv

<br>

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
| <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)"> Read: 12 </span>      | <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)"> Docs for the HTML canvas Element & Chart.js </span>       |[<img src="assets/taphere.gif">](class-12f)|
| <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)"> Read: 13 </span>      | <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)"> Local Storage </span>       |[<img src="assets/taphere.gif">](class-13)|
| <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)"> Read: 14a </span>      | <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)"> CSS Transforms, Transitions, and Animations </span>       |[<img src="assets/taphere.gif">](class-14a)|
| <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)"> Read: 14b </span>      | <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)"> What Google Learned About Teams </span>       |[<img src="assets/taphere.gif">](class-14b)|


<br>

---

<br>

| <span style="font-family:Courier New; font-size:13px;color:rgb(60, 179, 113)"> **Number** </span> |  <span style="font-family:Courier New; font-size:13px;color:rgb(60, 179, 113)"> **References** </span>  |
| ----------- | ----------- |
| <span style="font-family:Courier New; font-size:13px;color:rgb(60, 179, 113)"> [1] </span>      | <span style="font-family:Courier New; font-size:13px;color:rgb(60, 179, 113)"> https://learn.shayhowe.com/advanced-html-css/css-transforms/ </span>       |
| <span style="font-family:Courier New; font-size:13px;color:rgb(60, 179, 113)"> [1] </span>      | <span style="font-family:Courier New; font-size:13px;color:rgb(60, 179, 113)"> https://learn.shayhowe.com/advanced-html-css/transitions-animations/ </span>       |
| <span style="font-family:Courier New; font-size:13px;color:rgb(60, 179, 113)"> [1] </span>      | <span style="font-family:Courier New; font-size:13px;color:rgb(60, 179, 113)"> https://www.webdesignerdepot.com/2014/05/8-simple-css3-transitions-that-will-wow-your-users </span>       |