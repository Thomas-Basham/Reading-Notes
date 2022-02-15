# Class-07

## Read

[Domain-Modeling](https://github.com/codefellows/domain_modeling#domain-modeling)

    Process of creating a conceptual model of code for a specific problem

    From the article:
    When modeling a single entity that'll have many instances, build self-contained objects with the same attributes and behaviors.
    Model its attributes with a constructor function that defines and initializes properties.
    Model its behaviors with small methods that focus on doing one job well.
    Create instances using the new keyword followed by a call to a constructor function.
    Store the newly created object in a variable so you can access its properties and methods from outside.
    Use the this variable within methods so you can access the object's properties and methods from inside.

## From the Duckett HTML book

    Chapter 6: “Tables” (pp.126-145)

        <table> element is used to create a table

        <tr> tag indicates the start of each row

        <td> element (table data) represents each cell 

        <th> element represents heading for collumn or row

        <td colspan="2"> and <td rowspan="2"> are both attributes to maket collumns or rows span 2 spaces

        <thead>  where headings o f the table should sit

        <tbody>  

        <tfoot> where the footers go 

## From the Duckett JS Book

    Chapter 3: “Functions, Methods, and Objects” (pp.106-144)

        Create a blank object with constructor notation

        add propreties and methods to that object using dot notation

        the . is the member operator

        the = is the assignment operator 

        the keyword this is used inside functions and objects

        it refers to one object, usually the object in it's function 

        When a function is defined inside an object, it becomes a method

        in object literal notation, properties and methods of an object are given in curly braces 

        good for when you are storing data between applications

        good for global config of objects that set up info for a page

        arrays are objects

        the browser window is an object and is the top-most object. 

        Document Object Model DOM 

        document object is topmost object in DOM 

        it represents the web page loaded into the current browser

        document. title     property for title of current document

        document.write()     method that writes text to document

        use properties and methods of string object on string values

        each character in a string is automatically given a number, called an index number. this starts at 0 

        math object has properties and methods for mathematical constants and functions

        Math.round() rounds number to the nearest integer
             .floor() rounds down
             .ceil() rounds up
