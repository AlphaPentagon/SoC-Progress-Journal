# Craig's School of Code Progress Journal 💻|📘|📈

## Week 2

### 03 / 05

Today was a tough day.  New partners for pair programming (although we are in a three) and a lot to cover. Learned about the DOM (Document Object Model).  
I had some prior experience, but nearly out of my comfort zone!  Was a lot to take in and we jumped between different workshops.  In the evening I completed
the remainder of the tasks and felt much more comfortable with it.

### Learning log:

**DOM (Document Object Model)**

Specifically
- HTML is like the blueprint
- DOM is the building
- DOM has a tree like structure

You can use console.dir method to display the properties of a JS object

e.g. console.dir("h1") - would show all of the properties of the "h1" object

You can then use various methods to interact with these properties.

**document.querySelector();**

    - This will select the specified element
    - e.g. document.querySelector("h1") would select the h1 element
    - can store this result in a variable e.g. let mainTitle = document.querySelector("h1")

    Caveats 

    - querySelector with a class will just give you the first instance of that class
    - use querySelectorAll to select all the class items, or elements

**document.querySelectorAll();**

    - selects all the elements matching the one specified
    - stores them in a "node list"
    - can be accessed in the same way as an array
        - e.g. selectedElement[0] would select the first element of that node list

**.innerText = "";**

    - can be used to change the text of the element
        - e.g. mainTitle.innerText = "changedTitleText";

**document.createElement();**

    - creates a new element

**.appendChild();**

    - appends the specificed element as a child of the parent
        - e.g. document.parent.appencChild("child");

**.removeChild();**

    - as above, but removes the child

**Callback functions** 
    - functions without the () on the end 
    - doesn't call the function straight away - only when told to

**Event objects**
    - how JS stores all of the data of the event
    - can use `.addEventListener("event", callbackFunction);`
        - e.g. `.addEventListener("click", changeTitleColor); ` 

### 04/05 - May the 4th be with you...

Really enjoyed today.  Getting to know my new partners better and I'm adopting a bit of a leadership / teacher role, which I am not used to but enjoying
(but is also challenging).  Got to know about APIs and JSONs, as well as asynchronous coding.  Feels like the things we learnt in Wk1 and yesterday are now being built upon
and cemented.

Learned about asynchronous coding and JS methods
```
    setTimeout();
    setInterval();
    clearInterval();
```

**APIs (Application Programming Interface)**
    - a way for data to be exposed so you can interact with it

**Fetch API**

    - fetch() method
    - front end only
    - can us to request data from an API
    - fetch(resource) / resource = API URL as a string
        -returns a promise
            - promise that data will be delivered
        
**await**

    - Always await a promise!
        - waits for the promise to be delivered
        - must be used in an async function
        - e.g async function(){
            let response = async fetch("URL");
        }

**json**

    - use .json to unpack the data from the response
    - use 'await' before the .json method to receive the unpacked data and not the promise
    - e.g. let data = await response.json();

**Http**

    - Hyper Text Transfer Protocol
    - lof of different requests
    - most common request is 'Get' request
    - fetch method uses the 'Get' request as default

**JSON statement**

    - turn an object into a JSON
        - you 'stringify it'
        - the 'key' is a string
    - turn JSON into an object
        - parsing it

**Promise states**

    - Pending
        - Resolved
        - Rejected

### 05 / 05

Today we learned about different personality types (I'm an ISFJ, no matter how many times I take and number of different tests...), how they work within teams and how we can mitigate against any potential clashes.

We also took a further dive into APIs, navigating data and learned about the second fetch parameter {method:"",header: "", body {}} to enable us to use other methods, such as POST, PUT and PATCH.

Our team struggled with the afternoon task, which was an escape room puzzle.  We misunderstood the problem and were treating the steps like individual tasks, rather than a whole scenario.  Once we were gently nudged in the right diretion though we were able to use our knowledge to find the hidden data in the API and successfully 'escape the room'.

I had my mentor meeting in the evening which was great - Chris is such a great guy and really understanding.  He has made it clear that our meetings is a safe space for me to say what is challenging me or going well, and that is really helpful.

### 06 / 05

Today was our weekly hackathon project.  Todays task was to use an API to create some sort of game , or interavtive web page.  We chose a trivia API and used it to create a simple frontend game that would ask you 10 random questions and keep score of how well you do.  I especially enjoyed setting up the event listeners on the buttons and getting them to call different functions.  All in all I thought our team worked really well together and we achieved, and learnt alot, throughout the day.  We then presented them to about 30ish people, which was a great chance to practice our presentation skills.

## Week 3

### 09/05

Today we took our first step into UX with a guest speech from Pavaan Buddhdev, who enchanted us with close up magic and tales of UX sorcery.  Then we looked into Agile methodology and the benefits of this over the waterfall method of working.  We met our new pair programmers for the week and then took part in a spot the difference game, but for UI/UX, where we had to determine which of the screenshots of an app looked the 'most correct'.  We did really well, only missing a couple!

Some notes from the day:

- Agile
    - Individuals and interactions over processes and tools
    - Working software over comprehensive documentation
    - Customer collaboration over contract negotiation
    - Responding to change over following a plan

- UX
    - User experience
        - The beginning of the product
- UI
    User Interface
        - How the product's interfaces look and function

### 10/05

Another day of UX, with another guest speech, this time from Javaid Karim and Alex Fairholm from Nester.  They walked us through their UX choices and career paths which was really interesting and insightful.

We looked at UX design thinking as well as user stories and user persona's and were tasked with designing an application process for an imaginary bootcamp.  At the end we got to prototype these design ideas using flow charts.  We also took a look at CSS variables which appear to be super helpful for reusability and updating code efficiently.

Notes:

- UX Design Thinking
    1. Empathise - research user needs
    2. Define - state users needs & problems
    3. Ideate - challenge assumptions & create ideas (can be split further into the dreamer, realist and critic phases)
    4. Prototype - Start to create solutions
    5. Test - try your solutions out

### 11/05

Today we moved into UI territory.  We had a great guest speech from Luke Edwards. who is the Lead UI designer at Immediate Media.  He gave some really good tips on what sets a potential UI design applicant out, including showing enthusiasm through Github projects and demo's.  Real valuable stuff.

Then we took the UX design from the previous day and started to think about how we would design a UI for it.  We learned about colour palletes, principles of design, low fidelity vs high fidelity wireframes, accessibility, and different tools to enable us to design effectively.

At the end of the day we touched on CSS organisation and conventions and specificity.

- Accessibility
    -  Lighthouse, part of the Google dev tools is a great tool to show you how accesible your website is

- Elements & Principles of design
    - Line
    - Shape
    - Direction
    - Size
    - Texture
    - Colour
    - Balance
    - Proximity
    - Alignment
    - Repeating
    - Contrast
    - Space