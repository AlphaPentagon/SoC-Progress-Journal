03 / 05

Today was a tough day.  New partners for pair programming (although we are in a three) and a lot to cover. Learned about the DOM (Document Object Model).  
I had some prior experience, but nearly out of my comfort zone!  Was a lot to take in and we jumped between different workshops.  In the evening I completed
the remainder of the tasks and felt much more comfortable with it.

Learning log:

DOM (Document Object Model)

Specifically
- HTML is like the blueprint
- DOM is the building
- DOM has a tree like structure

You can use console.dir method to display the properties of a JS object

e.g. console.dir("h1") - would show all of the properties of the "h1" object

You can then use various methods to interact with these properties.

document.querySelector();

    - This will select the specified element
    - e.g. document.querySelector("h1") would select the h1 element
    - can store this result in a variable e.g. let mainTitle = document.querySelector("h1")

    Caveats 

    - querySelector with a class will just give you the first instance of that class
    - use querySelectorAll to select all the class items, or elements

document.querySelectorAll();

    - selects all the elements matching the one specified
    - stores them in a "node list"
    - can be accessed in the same way as an array
        - e.g. selectedElement[0] would select the first element of that node list

.innerText = "";

    - can be used to change the text of the element
        - e.g. mainTitle.innerText = "changedTitleText"

document.createElement();

    - creates a new element

.appendChild();

    - appends the specificed element as a child of the parent
        - e.g. document.parent.appencChild("child")l

.removeChild();

    - as above, but removes the child

Callback functions 
    - functions without the () on the end 
    - doesn't call the function straight away - only when told to

Event objects
    - how JS stores all of the data of the event
    - can use .addEventListener("event", callbackFunction);
        - e.g. .addEventListener("click", changeTitleColor);  

04/05 - May the 4th be with you...

Really enjoyed today.  Getting to know my new partners better and I'm adopting a bit of a leadership / teacher role, which I am not used to but enjoying
(but is also challenging).  Got to know about APIs and JSONs, as well as asynchronous coding.  Feels like the things we learnt in Wk1 and yesterday are now being built upon
and cemented.

Learned about asynchronous coding and JS methods
    - setTimeout();
    - setInterval();
    - clearInterval();

APIs (Application Programming Interface)
    - a way for data to be exposed so you can interact with it

Fetch API
    - fetch() method
    - front end only
    - can us to request data from an API
    - fetch(resource) / resource = API URL as a string
        -returns a promise
            - promise that data will be delivered
        
await
    - Always await a promise!
        - waits for the promise to be delivered
        - must be used in an async function
        - e.g async function(){
            let response = async fetch("URL");
        }

json
    - use .json to unpack the data from the response
    - use 'await' before the .json method to receive the unpacked data and not the promise
    - e.g. let data = await response.json();

Http
    - Hyper Text Transfer Protocol
    - lof of different requests
    - most common request is 'Get' request
    - fetch method uses the 'Get' request as default

JSON statement
    - turn an object into a JSON
        - you 'stringify it'
        - the 'key' is a string
    - turn JSON into an object
        - parsing it

Promise states
    - Pending
        - Resolved
        - Rejected


