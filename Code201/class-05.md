<img src="https://asac.ltuc.com/wp-content/themes/asac/images/logo.png" alt="Kitten"
	title="LTUC-Abdul Aziz Al Ghurair School of Advanced Computing" width="200" />  &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; <span style="font-family:Papyrus; font-size:25px;color:rgb(60, 179, 113)">**Welcome to Read: 05**</span>

---
<br>

<span style="font-family:Courier New; font-size:20px;color:rgb(60, 179, 113)"> **Read: 05 - "HTML Images; CSS Color & Text"** </span>

<span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)">In this Read: 05, I will have those three topics: 
</span>
- <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 13)">Images.
</span> 
- <span style="font-family:Courier New; font-size:15px;color:rgb(250, 179, 113)"> Color. 
</span>
- <span style="font-family:Courier New; font-size:15px;color:rgb(160, 90, 113)"> Text. 
</span>
---
<span style="font-family:Courier New; font-size:25px;color:rgb(60, 179, 13)">Images
</span> <br>
<span style="font-family:Courier New; font-size:15px;color:rgb(60, 130, 13)">Every website you saw until now, I think you release that they are have an images. So, how you can add an image in your webpage. <br></span> 

<span style="font-family:Courier New; font-size:15px;color:rgb(60, 130, 13)">But before you add an image it should be:
<br></span>
	- Be relevant <br>
	- Convey information<br>
	- Convey the right mood<br>
	- Be instantly recognisable<br>
	- Fit the color palette <br>	
<br>
<span style="font-family:Courier New; font-size:20px;color:rgb(60, 179, 13)">Adding Images</span><br>
<span style="font-family:Courier New; font-size:15px;color:rgb(60, 130, 13)">As an example of adding image.<br></span> 
```
<img src="https://asac.ltuc.com/wp-content/themes/asac/images/logo.png" alt="Kitten"
title="LTUC-Abdul Aziz Al Ghurair School of Advanced Computing" width="200" height="450" />
```
> - To add an image into the page
you need to use an `<img>`
element. <br>
> - `src` This tells the browser where it can find the image file.<br>
> - `alt` This provides a text description of the image which describes the image if you cannot see it.<br>
> - `title` You can also use the title attribute with the `<img>` element to provide additional information about the image.<br>
> - `width` This specifies the width of the image in pixels.<br>
> - `height` This specifies the height of the
image in pixels.<br>

<span style="font-family:Courier New; font-size:20px;color:rgb(60, 179, 13)">Three rules for Creating Images</span><br>
![3rules](https://raw.githubusercontent.com/shadykh/reading-notes/main/Code201/assets/3rules.PNG)<br><br>

---
<span style="font-family:Courier New; font-size:25px;color:rgb(250, 179, 113)"> Color </span><br>
<span style="font-family:Courier New; font-size:15px;color:rgb(200, 179, 113)">Can you imagine the life without colors, it will be disaster and depressed life. Without colors we cannot live and enjoy in this life, and so that the website, without colors they will be boring webpages. <br></span> <br>
<span style="font-family:Courier New; font-size:20px;color:rgb(200, 179, 113)">Foreground Color</span><br>
<span style="font-family:Courier New; font-size:15px;color:rgb(200, 179, 113)">The color property allows you to specify the color of text inside an element. You can specify any
color in CSS in one of three ways:</span>
```
/* color name */
h1 {
color: DarkCyan;}
/* hex code */
h2 {
color: #ee3e80;}
/* rgb value */
p {
color: rgb(100,100,90);}
```
>-  rgb values : These express colors in terms of how much red, green and blue are used to make it up. For example: rgb(100,100,90)
>-  hex Codes
These are six-digit codes that represent the amount of red, green and blue in a color,
preceded by a pound or hash # sign. For example: #ee3e80.
> - Color names: There are 147 predefined color names that are recognized 
by browsers. For example: DarkCyan.<br>

<span style="font-family:Courier New; font-size:20px;color:rgb(200, 179, 113)">Background-Color</span><br>
<span style="font-family:Courier New; font-size:15px;color:rgb(200, 179, 113)">CSS treats each HTML element as if it appears in a box, and the background-color propert sets the color of the background for that box. You can specify your choice of background color in the same three ways you can specify foreground colors: RGB values, hex codes, and color names. To understand the colors, see the following photo. </span><br>
![colors](https://raw.githubusercontent.com/shadykh/reading-notes/main/Code201/assets/colors.PNG)<br><br>
<span style="font-family:Courier New; font-size:15px;color:rgb(200, 179, 113)">Contrast</span><br>
![contrast](https://raw.githubusercontent.com/shadykh/reading-notes/main/Code201/assets/ontrast.PNG)<br><br>
<span style="font-family:Courier New; font-size:20px;color:rgb(200, 179, 113)">Opacity</span><br>
<span style="font-family:Courier New; font-size:15px;color:rgb(200, 179, 113)">CSS3 introduces the opacity property which allows you to specify the opacity of an element
and any of its child elements. The value is a number between 0.0 and 1.0 (so a value of 0.5
is 50% opacity and 0.15 is 15% opacity).
The CSS3 rgba property allows you to specify a color, just like you would with an RGB value,
but adds a fourth value to indicate opacity.  </span><br>
![hsl](https://raw.githubusercontent.com/shadykh/reading-notes/main/Code201/assets/hsl.PNG)<br><br>
<span style="font-family:Courier New; font-size:20px;color:rgb(200, 179, 113)">hsl & hsla</span><br>
<span style="font-family:Courier New; font-size:15px;color:rgb(200, 179, 113)">The hsl color property has been introduced in CSS3 as an alternative way to specify colors. The value of the property starts with the letters hsl, followed by individual values inside parentheses for:<br>
hue<br>
This is expressed as an angle
(between 0 and 360 degrees).<br>
saturation<br>
This is expressed as a percentage.
lightness<br>
This is expressed as a
percentage with 0% being white,
50% being normal, and 100%
being black. </span><br>

---
<span style="font-family:Courier New; font-size:25px;color:rgb(160, 90, 113)"> Text 
</span><br>
<span style="font-family:Courier New; font-size:15px;color:rgb(160, 90, 113)"> Of course, every webpage has a text on it, so how we can do styling to the text. We will show here how you do style to text. See the following.  
</span> <br>
<span style="font-family:Courier New; font-size:15px;color:rgb(160, 90, 113)"> Typeface Terminology  </span> <br>
![typeface](https://raw.githubusercontent.com/shadykh/reading-notes/main/Code201/assets/typeface.PNG)<br><br>
![xyz](https://raw.githubusercontent.com/shadykh/reading-notes/main/Code201/assets/xyz.PNG)<br><br>
<span style="font-family:Courier New; font-size:15px;color:rgb(160, 90, 113)"> Choosing A Typeface For Your Website  </span> <br>
![type](https://raw.githubusercontent.com/shadykh/reading-notes/main/Code201/assets/type.PNG)<br><br>
<span style="font-family:Courier New; font-size:15px;color:rgb(160, 90, 113)"> units of Type Size </span> <br>
![unitsize](https://raw.githubusercontent.com/shadykh/reading-notes/main/Code201/assets/unitsize.PNG)<br><br>
<span style="font-family:Courier New; font-size:15px;color:rgb(160, 90, 113)"> Attribute Selectors </span> <br>
![asec](https://raw.githubusercontent.com/shadykh/reading-notes/main/Code201/assets/asec.PNG)<br><br>
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

