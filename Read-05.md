# Operators and Loops

### In this notes we will mention the operatoers that used in js, then we will mention the loops with thier types.

## The Operators:
### We have difreent types of operatores; the comparsion operatores and the logical operatores.

### The comparison operatores:
- #### Is equal to:
    - ##### (==) : This operator compare two vaules (numbers, string or booleans) to see if they are the same value.
        - "Good" == "Bad" , it's false.
- #### Is not equal to:
    - ##### (!=) : This operator compare two vaules (numbers, string or booleans) to see if they are not the same value.
        - "Good" != "Bad" , it's true.
- #### Strict equal to:
    - ##### (===) : This operator compare two vaules (numbers, string or booleans) to see if they are the same value and type.
        - "Good" === "Bad" , it's fasle.
- #### Strict not equal to:
    - ##### (!==) : This operator compare two vaules (numbers, string or booleans) to see if they are not the same.
        - "Good" !== "Bad" , it's true.
- #### Greater than:
    - ##### (>) : This operator check if the left side is greater than than the rgiht side.
        - 5 > 4 , it's true.
- #### Less than:
    - ##### (<) : This operator check if the left side is less than than the rgiht side.
        - 4 < 5 , it's true.
- #### Greater than or equal to:
    - ##### (>=) : This operator check if the left side is greater than than or eqaul the rgiht side.
        - 5 >= 5 , it's true.
- #### Less than or equal to:
    - ##### (<=) : This operator check if the left side greater than than or eqaul the rgiht side.
        - 4 <= 2 , it's true.

### The logical operatores:
- #### Logical and (&&):
    - ##### This operator test more than one condition.
        - ((5 < 5) && (5 >= 5)) , it's false.
- #### Logical and (||):
    - ##### (!=) : This operator test at least one condition.
        - ((5 < 5) || (5 >= 5)) , it's true.
- #### Logical not (!):
    - ##### (===) : This operator takes a single boolean value an invert it.
        - !(5 >= 5) , it's fasle.


---

## The Loops:
### We have difreent types of loops; the for and while loops.

- ### For loops:
    the synatx for the for loop:

    ```
    for (init; condition; upadte)
    {
        statement;
    }
    ```
    As an example:

    ```
    var i = 0
    for (i=0; i > 0; i = i+1)
    {
        doucemnt.write(i);
    }
    ```
- ### While loops:
    the synatx for the while loop:

    ```
    while (condition)
    {
        statement;
        updtae;
    }
    ```
    As an example:

    ```
    var i = 0
    for (i > 0)
    {
        doucemnt.write(i);
        i = i+1
    }
    ```
- ### some notes:
    - You can use (i++) insted of (i=i+1), it's the same thing.
    - You can use (i--) insted of (i=i-1), it's the same thing.

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
[Mems](./mems) |
[More about me](./aboutme) | 

<br>
