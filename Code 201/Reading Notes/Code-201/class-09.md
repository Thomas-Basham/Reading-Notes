# Class 09

## From the Duckett HTML book

    Chapter 7: “Forms” (p.144-175)

    in html, use <form></form> to make a form element where the controls are stored inside

    every form element requires an action attribute. attribute = url for the page on the server that wil recieve the info in the form when it's submitted

    forms are sent through either 2 methods : get or post

    <form action="url"method="get">
      <p>enter text here</p>
      </form>

    other elements like text text area inside form tag

    attributes like password, username, value, checked(value), and select can be used to make multiple different types of forms

    Label form controls using <Label> element

    Label each form control

    you con group form controls together in the <fieldset> element



    Chapter 14: “Lists, Tables & Forms” (pp.330-357)

    ordered lists display numbers

    unordered lists display bullets

    use list style-style-position: outside/inside to let text wrap arround the bullet or stay alligned 

    you can show or hide empty cells by  empty-cells:show/hide

    style buttons using color, text-shadow, border-bottom, background-color.

    style curser in css

    forms are easier to use if the form controls are vertically aligned using css

## From the Duckett JS book

    Chapter 6: “Events” (pp.243-292)

    Events occur in the browser while the user is browsing. They can be used to trigger a function in your javascript code

    three steps involved to get event to trigger javascript code
      1. select the element node(s) you want
      2. indicate which event on the selected node(s) will trigger a response 
      3. state the code you want to run when the even occurs

    Three was to bind an event to an element
      1. html event handlers(bad practice)
      2. traditional DOM event handlers
          element.onevent = functionName;
      3. DOM level 2 event listeners (favored way). can deal with more than one function at a time.
        element.addEventsListener('event', functionName [, boolean]); 
        boolean is usally set to false

    IE5-8 does not support the addEventListener() method. It uses it's own method called attatchEvent()

    events flow from nested elements to containing parent elements

    when an event occurs, the event object tells you information about the event and the element it happened on. 

    the event object is passed to any function that is the event handler or listener 

    The most commonly used events are W3C DOM events
