<img src="https://asac.ltuc.com/wp-content/themes/asac/images/logo.png" alt="Kitten"
	title="LTUC-Abdul Aziz Al Ghurair School of Advanced Computing" width="200" />  &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; <span style="font-family:Papyrus; font-size:25px;color:rgb(60, 179, 113)">**Welcome to Read: 01**</span>

---
<br>

<span style="font-family:Courier New; font-size:20px;color:rgb(60, 179, 113)"> **Read: 01 "Introductory HTML and JavaScript"** </span>

## **Structure:**
To bulid a web page you need to write the code that turn the wrods into web page, so here we will talk about the bones of the web page which is the **Structure**.

Think about the stories you read in a newspaper: for each
story, there will be a headline, some text, and possibly some
images. If the article is a long piece, there may be subheadings that split the story into separate
sections or quotes from those involved. Structure helps readers understand the stories in the newspaper.

The **HTML** is the langunage used to build a web pages, فاث **HTML** stands for HyperText Markup Language. The **HyperText** part refers to the fact that HTML allows you to create links that allow visitors to move from one page to another quickly and easily. **A markup language** allows you to annotate text, and these annotations provide additional meaning to the contents of a document. If you think of a web page, we add code around the original text we want to display and the browser then uses the code to display the page correctly. So the tags we add are the markup.

So, now I think that we got enhoth talking so let us start coding.
``` 
<html>
    <head>
        <title>This is the Title of the Page</title>
    </head>
    <body>
        <h1>This is the Body of the Page</h1>
        <p>Anything within the body of a web page is
        displayed in the main browser window.</p>
    </body>
</html>
```
This code give you this output:
>
> <html>
> <head>
> <title>This is the Title of the Page</title>
> </head>
> <body>
> <h1>This is the Body of the Page</h1>
> <p>Anything within the body of a web page is
> displayed in the main browser window.</p>
> </body>
> </html>

You can chcek this figure,<br>![SampleHtml](https://slideplayer.com/slide/6303967/21/images/12/Sample+Webpage+HTML+Structure.jpg)

<br>
---
## **Extra Markup**

In HTML5, web page authors do not need to close all tags, and new elements and attributes will be introduced. At the time of writing, the HTML5 specification had not been completed, but the major browser makers had
started to implement many of the new features, and web page authors were rapidly adopting the new markup.

Here we will go farther with the HTML5 commands, and we will have some examples, so keep track us here to get know more info about HTML5.

- DOCTYPE
    - Because there have been several versions of HTML, each web page should begin with a DOCTYPE declaration to tell a browser which version of HTML the page is using.
         ```
          <!DOCTYPE html>
         <html lang="en">
         <head>
             <meta charset="UTF-8">
             <title>Home</title>
         </head>
         ```

- Comments in html
    - If you want to add a comment to your code that will not be visible in the user's browser, you can add the text between these characters:
        ```
        <!-- comment goes here -->
        ```

- ID Attribute
    - Every HTML element can carry the id attribute. It is used to uniquely identify that element from other elements on the page. Its value should start with a letter or an underscore.
        ```
        <p>Water and air. So very commonplace are these
        substances, they hardly attract attention - and
        yet they vouchsafe our very existence.</p>
        <p id="pullquote">Every time I view the sea I feel
        a calming sense of security, as if visiting my
        ancestral home; I embark on a voyage of seeing.
        </p>
        <p>Mystery of mysteries, water and air are right
        there before us in the sea.</p>
        ```
        The reslut is:<br>
            Water and air. So very commonplace are these
            substances, they hardly attract attention - and yet they vouchsafe our very existence.<br>
            <font size="4"> **Every time I view the sea I feel a calming sense of security, as if visiting my ancestral home; I embark on a voyage of seeing.<br>**</font> 
            Mystery of mysteries, water and air are right
            there before us in the sea.

- Class Attribute
    - If you want to add a comment to your code that will not be visible in the user's browser, you can add the text between these characters:
        ```
        <!-- comment goes here -->
        ```

- Meta
    - The `<meta>` element lives inside the `<head>` element and
    contains information about that web page. It is not visible to users but fulfills a number of purposes such as telling search engines about your page, who created it, and whether or not it is time sensitive.

---
## **HTML5 Layout:**

HTML5 is introducing a new set of elements that help define the structure of a page. The new HTML5 give you a better experience with layout building than the old versions, I will mention the differences here.
* `<header>`
    ```
    <!DOCTYPE html>
    <html lang="en">
    <head>
        <meta charset="UTF-8">
        <title>Home</title>
    </head>
    ```
* `<footer>`
    ```
    <footer>
        &copy; LOL team: Shady and Mousa
    </footer>
    ```

* `<nav>`: For navgation.
    ```
    <nav>
            <ul>
                <li>
                    <a href="https://shadykh.github.io/Html/">
                        Home
                    </a>
                    </li>
            </ul>
        </nav>
    ```

* `<article>`
    ```
    <article>
    <p>A five week introduction to traditional
    Japanese vegetarian meals, teaching you a
    selection of rice and noodle dishes.
    </p>
    </article>
    ```
* `<aside>` and `<section>`
    ```
    <aside>
    <section>
    <h2>Popular Recipes</h2>
    <a href="">Yakitori (grilled chicken)</a>
    <a href="">Tsukune (minced chicken patties)</a>
    <a href="">Okonomiyaki (savory pancakes)</a>
    <a href="">Mizutaki (chicken stew)</a>
    </section>
    <section>
    <h2>Contact</h2>
    <p>Yoko's Kitchen<br />
    27 Redchurch Street<br />
    Shoreditch<br />
    London E2 7DP</p>
    </section>
    </aside>
    ```

* `<hgroup>`, `<figure>` and `<figcaption>`
    - `<hgroup>`: For Heading Groups.
    - `<figure>` and `<figcaption>` : For Figures.

    ```
    <article>
    <figure>
    <img src="images/bok-choi.jpg" alt="Bok Choi" />
    <figcaption>Bok Choi</figcaption>
    </figure>
    <hgroup>
    <h2>Japanese Vegetarian</h2>
    <h3>Five week course in London</h3>
    </hgroup>
    <p>A five week introduction to traditional
    Japanese vegetarian meals, teaching you a
    selection of rice and noodle dishes.</p>
    </article>
    ```
    
* `<div>`: For Sectioning Elements.
    ```
    <div class="wrapper">
    <header>
    <h1>Yoko's Kitchen</h1>
    <nav>
    <!-- nav content here -->
    </nav>
    </header>
    <section class="courses">
    <!-- section content here -->
    </section>
    <aside>
    <!-- aside content here -->
    </aside>
    <footer>
    <!-- footer content here -->
    </footer>
    </div><!-- .wrapper -->
    ```
<br>
---
## **Process & Design:**

we will discusses the process that you will  use when you are creating a new website.
Every website should be designed for the target audience—not just for yourself or the site owner. It is therefore very important to understand who your target audience is.

We have two types of your target audience: Individuals or companies. So, you should know the answers for those questions:
> * What are their needs? 
> * Why they will visit your website? 
> * What they are searching for? 
> * How often they will visit your website?

You have the answers for those questions. How is that? When you want to build a website; you decide that because you have something to share with others! So, you know who are those people who wants what you are sharing with them. From this point you should find your ideal audience and study them to know more about them. What they are like, what they are hate and even what they are doing in the morning! Are you kidding me? No, when you know all those details, you will give them the best experience when they visit your website, **because you build this website to be suitable for them not for you!**

After you finished the above step, now you will plan for your website; How it should be? So, there is something called **site map**; which is a diagram of the pages that will be used to structure the site. And there is a technique called **card sorting**; which involves placing each piece of information that a visitor might need to know on a separate piece of paper and then organizing the related information into groups. For an example of a site map please, see the following figure.

![Figure example site map](https://blog.hubspot.com/hs-fs/hubfs/dyno-mapper-sitemap-generator.png?width=566&name=dyno-mapper-sitemap-generator.png)

### **Wireframes** 

is a simple sketch of the key information that needs to go on each page of a site. It shows the hierarchy of the information and how much space it might require. By creating a wireframe, you can ensure that all of the information that needs to be on a page is included. 

You should not include the color scheme, font choices, backgrounds or images for the website in the wireframe. It should focus on what information needs to be on each page and create a visual hierarchy to indicate the most important parts of each page. For an example of a wireframe please, see the following figure.

![Figure example site map](https://d1dlalugb0z2hd.cloudfront.net/handbooks/agile-handbook/wireframe/01-youtube-wireframe-example.png)

### **Organizing your page**

The primary aim of any kind of visual design is to communicate. Organizing and prioritizing information on a page helps users understand its importance and what order to read it in. We have here three main words: **Content**, **Prioritizing** and **Organizing**.

*  **Content** 

	Web pages often have a lot of information to communicate. As an example:
    + A masthead or logo
    + Links to navigate the site
    + Links to related content and other popular articles
    + Login or membership options

* **Prioritizing**

	If everything on a page appeared in the same style, it would be much harder to understand. By making parts of the page look distinct from surrounding content, designers draw attention to those items. Designers create something known as a visual hierarchy to help users focus on the key messages that will draw people's attention, and then guide them to subsequent messages.

* **Organizing**

	Grouping together related content into blocks or chunks makes the page look simpler. By presenting certain types of information in a similar visual style, users will learn to associate that style with a particular type of content.


* **Visual hierarchy**

	Most web users do not read entire pages. You can use contrast to create a visual hierarchy that gets across your key message and helps users find what they are looking for.
    * Size
        > <font size="5">The way</font> to get started is to quit talking and begin doing. - Walt Disney
    * Color
        > <span style="color:orange">The way</span> to get started is to quit talking and begin doing. -Walt Disney
    * Style
        > ***The way*** to get started is to quit talking and begin doing. -Walt Disney

    
* **Grouping**

	Grouping related pieces of information together can make a design easier to comprehend.Here are some ways this can be achieved.


    
* **Similarity**

	We naturally observe similarities in design, and things that are similar are perceived to be more related than things that are dissimilar. Repetition of similar color, size, orientation, texture, font, or shape, suggests that matching elements have similar importance or meaning.

### **Designing Navigation**

Site navigation not only helps people find where they want to go, but also helps them understand what your site is about and how it is organized. Good navigation tends to follow these principles..
* Concise
* Clear
* Selective
* Context
* Interactive
* Consistent

<br>
---
# Programming with JavaScript
### Did you ever used the slideshow or forms in any webpage? How you interact with them? Did you access, modify, program or react to the content in some webpage?
<br>

### I think that you already did those things! This is done by Java Script, yes the language that used to :
- #### Access content.
- #### Modify content.
- #### Program rules.
- #### React to events.
<br>

### Before you learn how to read and write the JavaScript language itself, you need to become familiar with some key concepts in computer programming.  
- ### What is a script and how do I create one?
    - ### **A script** is a series of instructions that a computer can follow to achieve a goal.

- ### How do computers fit in with the world around them?
    - ### Computers create models of the world using data, those models use objects to represent physical things.
- ### How do I write a script for a web page?
    - ### To write a script, you need to first state your goal and then list the tasks that need to be completed in order to achieve it.
## WHAT IS A FUNCTION?
### Functions let you group a series of statements together to perform a specific task. If different parts of a script repeat the same task, you can reuse the function (rather than repeating the same set of st atements).
<br>

### How do we declar a function:
    ```
    function printtest() {
        document.write("test);
    }
    ```

<br>

### How we call a function:
    ```
    printtest();
    ```
---
<br>

> This summry is taken from priveous reading notes. Code 102-Read 03 and Read 04.


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

