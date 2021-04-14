# Read: 09 - Forms and Events

## Events/JS
Browsers registers events as a way of telling the script of what is going on. It could be something like: loading, error, etc…
Event handling steps:
1.	Select the element nodes that you want the script to respond to.
2.	Indicate which event on the trigger node will trigger the response.
3.	State the code to run after the event occurs.

Handling events can be one of 3 ways: 
1.	HTML -- bad practice
2.	Traditional DOM.
3.	DOM level 2 event listeners.
DOM handlers are a better practice because the flow of trigger is opposite to HTML. The latter flows from child elements to their containers, which causes problems because for example when you select  an element you select its parent as well, which causes bubbling. 

## Forms/HTML
Forms in HTML are ways to collect information from website visitors. Information can be collected through many ways, such as search boxes, selection from a menu, etc …
How it works?
User enters information --- > information are sent to the server --- > server processes them through a programing language and stores them in a database --- > give back a message to the user

Form general syntax: 

``` 
<form action=”URL where the server receives information” 
method=”get”/””post”> form control appears </form>
```
For each different way of data collecting (password, text, etc…) will have a different syntax of HTML.
