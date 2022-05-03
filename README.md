03 / 05

Learned about the DOM (Document Object Model)

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
