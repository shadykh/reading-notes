<img src="https://asac.ltuc.com/wp-content/themes/asac/images/logo.png" alt="Kitten"
	title="LTUC-Abdul Aziz Al Ghurair School of Advanced Computing" width="200" />  &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; <span style="font-family:Papyrus; font-size:25px;color:rgb(60, 179, 113)">**Welcome to Read: 13**</span><br>

---

<br>

<span style="font-family:Courier New; font-size:20px;color:rgb(60, 179, 113)"> **Read: 13 - "Local Storage"** </span> <br>

<span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)">In this Read: 13, I will talk only about: 
</span><br>
- <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)"> Local Storage.</span><br><br>


---

<br><br>

<span style="font-family:Courier New; font-size:25px;color:rgb(60, 179, 113)"> Local Storage </span><br>
<span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)">What is the Local Storage?</span><br>
<span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)"> The operating system typically provides an abstraction layer for storing and retrieving application-specific data like preferences or runtime state. These values may be stored in the registry, INI files, XML files, or some other place according to platform convention. If your native client application needs local storage beyond key/value pairs, you can embed your own database, invent your own file format, or any number of other solutions. <br> Historically, web applications have had none of these luxuries. Cookies were invented early in the web’s history, and indeed they can be used for persistent local storage of small amounts of data. <br> But they have three potentially dealbreaking downsides: </span> <br>

- <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)">Cookies are included with every HTTP request, thereby slowing down your web application by needlessly transmitting the same data over and over.</span><br>


- <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)">Cookies are included with every HTTP request, thereby sending data unencrypted over the internet (unless your entire web application is served over SSL)</span><br>

- <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)">Cookies are limited to about 4 KB of data — enough to slow down your application (see above), but not enough to be terribly useful</span><br>

- <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)">What we really want is:</span><br>
    - <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)">A lot of storage space.</span><br>
    - <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)">On the client.</span><br>
    - <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)">That persists beyond a page refresh.</span><br>
    - <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)">Isn’t transmitted to the server.</span><br>


<span style="font-family:Courier New; font-size:25px;color:rgb(60, 179, 113)">HTML5 Storage</span><br>
<span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)">HTML5 Storage” is a specification named Web Storage, which was at one time part of the HTML5 specification proper, but was split out into its own specification for uninteresting political reasons. Certain browser vendors also refer to it as “Local Storage” or “DOM Storage.”</span><br>
<span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)">It’s a way for web pages to store named key/value pairs locally, within the client web browser. Like cookies, this data persists even after you navigate away from the web site, close your browser tab, exit your browser, or what have you. Unlike cookies, this data is never transmitted to the remote web server (unless you go out of your way to send it manually). </span> <br>

- <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)">HTML5 STORAGE SUPPORT</span><br>
    ![support](https://raw.githubusercontent.com/shadykh/reading-notes/main/Code201/assets/support.PNG)<br><br>

- <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)">Check for HTML5 Storage</span><br>
    ```
    function supports_html5_storage() {
        try {
            return 'localStorage' in window && window['localStorage'] !== null;
        } catch (e) {
            return false;
        }
    }
    ```
    <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)">OR</span><br>
    ```
    if (Modernizr.localstorage) {
        // window.localStorage is available!
    } else {
        // no native support for HTML5 storage :(
        // maybe try dojox.storage or a third-party solution
    }
    ``` 
<br>
<span style="font-family:Courier New; font-size:25px;color:rgb(60, 179, 113)">USING HTML5 STORAGE</span><br>
<span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)">HTML5 Storage is based on named key/value pairs. You store data based on a named key, then you can retrieve that data with the same key. The named key is a string. The data can be any type supported by JavaScript, including strings, Booleans, integers, or floats. However, the data is actually stored as a string. If you are storing and retrieving anything other than strings, you will need to use functions like parseInt() or parseFloat() to coerce your retrieved data into the expected JavaScript datatype.</span><br>

```
interface Storage {
getter any getItem(in DOMString key);
 setter creator void setItem(in DOMString key, in any data);
 };    
```

<br>
<span style="font-family:Courier New; font-size:25px;color:rgb(60, 179, 113)">TRACKING CHANGES TO THE HTML5 STORAGE AREA</span><br>
<span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)">If you want to keep track programmatically of when the storage area changes, you can trap the storage event. The storage event is fired on the window object whenever setItem(), removeItem(), or clear() is called and actually changes something. For example, if you set an item to its existing value or call clear() when there are no named keys, the storage event will not fire, because nothing actually changed in the storage area.</span><br>

```
if (window.addEventListener) {
  window.addEventListener("storage", handle_storage, false);
} else {
  window.attachEvent("onstorage", handle_storage);
};  
```
- <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)">STORAGEEVENT OBJECT</span><br>
    ![storobj](https://raw.githubusercontent.com/shadykh/reading-notes/main/Code201/assets/storobj.PNG)<br><br>


> For more information please see the reference [1].


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
| <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)"> Read: 14a </span>      | <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)"> CSS Transforms, Transitions, and Animations </span>       |[<img src="assets/uc.gif">](UC)|
| <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)"> Read: 14b </span>      | <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)"> What Google Learned About Teams </span>       |[<img src="assets/uc.gif">](UC)|


<br>

---

<br>

| <span style="font-family:Courier New; font-size:13px;color:rgb(60, 179, 113)"> **Number** </span> |  <span style="font-family:Courier New; font-size:13px;color:rgb(60, 179, 113)"> **References** </span>  |
| ----------- | ----------- |
| <span style="font-family:Courier New; font-size:13px;color:rgb(60, 179, 113)"> [1] </span>      | <span style="font-family:Courier New; font-size:13px;color:rgb(60, 179, 113)"> http://diveinto.html5doctor.com/storage.html </span>       |