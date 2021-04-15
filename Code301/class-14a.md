<img src="https://asac.ltuc.com/wp-content/themes/asac/images/logo.png" alt="Kitten"
	title="LTUC-Abdul Aziz Al Ghurair School of Advanced Computing" width="200" />  &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; <span style="font-family:Papyrus; font-size:25px;color:rgb(60, 179, 113)">**Welcome to Read: 14a**</span>

---
<br>

<span style="font-family:Courier New; font-size:20px;color:rgb(60, 179, 113)"> **Database Normalization** </span>


<span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)">In this Read: 14a, I will talk about this topic: 
</span>
- <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)">Database Normalization.
<br>

---
<br>

<span style="font-family:Courier New; font-size:20px;color:rgb(60, 179, 113)">**Database Normalization** </span><br>
<span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)">Database normalization is a process used to organize a database into tables and columns.  The main idea with this is that a table should be about a specific topic and only supporting topics included.<br>
</span> 

- <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)">Reasons for Database Normalization</span><br>

    - <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)">There are three main reasons to normalize a database.  **The first** is to minimize duplicate data, **the second** is to minimize or avoid data modification issues, and **the third** is to simplify queries. </span><br>

- <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)">Data Duplication and Modification Anomalies</span><br>

    - <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)">Notice that for each SalesPerson we have listed both the SalesOffice and OfficeNumber. There are duplicate salesperson data. Duplicated information presents two problems:<br>
        - It increases storage and decrease performance. <br>
        - It becomes more difficult to maintain data changes. </span><br>

- <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)">Search and Sort Issues</span><br>

    - <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)"> The last reason we’ll consider is making it easier to search and sort your data.</span><br>

- <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)">Definition of Database Normalization</span><br>

    - <span style="font-family:Courier New; font-size:15px;color:rgb(60, 179, 113)">There are three common forms of database normalization: 1st, 2nd, and 3rd normal form. They are also abbreviated as 1NF, 2NF, and 3NF respectively. There are several additional forms, such as BCNF, but I consider those advanced, and not too necessary to learn in the beginning. <br>
    The forms are progressive, meaning that to qualify for 3rd normal form a table must first satisfy the rules for 2nd normal form, and 2nd normal form must adhere to those for 1st normal form. Before we discuss the various forms and rules in detail, let’s summarize the various forms:<br>
        - First Normal Form – The information is stored in a relational table with each column containing atomic values. There are no repeating groups of columns. <br>
        - Second Normal Form – The table is in first normal form and all the columns depend on the table’s primary key.<br> 
        - Third Normal Form – the table is in second normal form and all of its columns are not transitively dependent on the primary key
        </span><br>



<br><br>

> For further infromation please click [here](https://www.essentialsql.com/get-ready-to-learn-sql-database-normalization-explained-in-simple-english/).

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






