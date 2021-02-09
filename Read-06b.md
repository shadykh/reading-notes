# CSS

### Until now I think you know more about Html and js, and may you have built some basic pages without styling them. So, how you can style your basic page for now.

### You will use the CSS, it  allows you to create rules that specify how the content of an element should appear. 

### CSS works by associating rules with HTML elements. These rules govern how the content of specified elements should be displayed. A CSS rule contains two parts: a **selector** and a **declaration**.
    ```
    p { font-family: Arial;}
    // p is the selector
    // { font-family: Arial;} is the declaration
    ```

### CSS declarations sit inside curly brackets and each is made up of two parts: a **property** and a **value**, separated by a colon. You can specify several properties in one declaration, each separated by a semi-colon.

    ```
    h1, h2, h3 {
    font-family: Arial;
    color: yellow;}
    // font-family and color are the properties
    // Arial and yellow are the values
    ```
### In the below you can find an example of using external css styling:
![image](1.png)
### And this for intrnal css styling:
![image](2.png)

---

## CSS Selectors
![image](3.png)

---

## Colors

### In css we have many ways to use colors in our css style file, and they are:
- rgb values
    - These express colors in terms of how much red, green and blue are used to make it up. For example: rgb(100,100,90).
- hex codes
    - These are six-digit codes that represent the amount of red, green and blue in a color, preceded by a pound or hash # sign. For example: #ee3e80.
- color names
    - There are 147 predefined color names that are recognized by browsers. For example: DarkCyan.

### Contrast
- When picking foreground and background colors, it is important to ensure that there is enough contrast for the text to be legible.
    ![image](4.png)

### Opacity
- CSS3 introduces the opacity property which allows you to specify the opacity of an element and any of its child elements. The value is a number between 0.0 and 1.0 (so a value of 0.5 is 50% opacity and 0.15 is 15% opacity).

### hsl, hsla
- The hsl color property has been introduced in CSS3 as an
alternative way to specify colors. The value of the property starts with the letters hsl, followed by individual values inside parentheses for:
    - **hue** 
        - This is expressed as an angle (between 0 and 360 degrees).
    - **saturation** 
        - This is expressed as a percentage.
    - **lightness** 
        - This is expressed as a percentage with 0% being white, 50% being normal, and 100% being black.
    - **alpha**
        - This is expressed as a number between 0 and 1.0. For example, 0.5 represents 50% transparency, and 0.75 represents 75% transparency.

---
<br>

My website contents|
------------ | 
[Main](https://shadykh.github.io/reading-notes/) | 
[Read: 02a - Learning Markdown](./Read-02a) |
[Read: 02b - Revisions and the Cloud](./Read-02b) |
[Read: 03 - Structure web pages with HTML](Read-03) |
[Read: 04 - Programming with JavaScript](Read-04) |
[Read: 05 - Operators and Loops](Read-05) |
[Read: 06a - Functions](Read-06a) |
[Read: 06b - Design web pages with CSS](Read-06b) |
[Mems](./mems) |
[More about me](./aboutme) | 

<br>
