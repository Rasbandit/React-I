# React I

## Overview

### Slides

- What is react
    - React is a SPA (Single Page Application)
        - Slow initial load time but faster overall application
        - no page flash
    - Component Base Architecture
        - A component is a reusable piece of code.
        - allows you to think of your application in isolation.
        - Break up a page into components
    - Two types of Component
        - Stateful and Stateless
    - State
        - State is the info stored that the component needs
        - Think of state like a country, all countries have the same properties but different values.
        - That is the state of the country
    - JSX
        - JSX is JavaScript XML and it looks like HTML
        - Its how react creates HTML and DOM Elements
        - JSX has some slight differences
    - DOM
        - The DOM is what the browser turns HTML into
        - The Virtual DOM is what react turns into.
        - React updates the Virtual DOM and then the DOM.

### Code

- run `create-react-app`
- overview of the files
    - Package.json
        - stores a list of all the code we need for our project
        - also has `npm start`
        - tied to node_modules
        - npm
            - a community of people who upload their code for the community to use as a whole.
    - node_modules
        - this is where all the code that react needs to run is stored.
        - when we run NPM things it gets stored here
    - public
        - The HTML files we need
        - dont touch these
    - src
        - where we will be doing most of our work.
        - all our react files must be in this folder
    - index.js
        - At the top we have all the `imports` for files/packages we need for this file
        - if there is not a `./` then it is a package
        - no `./` means it is a package we got from npm
        - we can also bring in css files and JS files
            - js files do not need to include the extension.
        - ReactDom.render take in the root component and the element it will be rendered into also.
            - show them the div inside the HTML that gets rendered
    - App.js
        - import React and destructure Component
        - React must be in scope when JSX is written
        - We have a class that extends Component
            - what can we assume because the word extends?
        - the render method returns JSX and that is what gets rendered on the screen
        - Run NPM Start
        - Show them how the elements pane looks
            - compare that to the react dev tools
    - JSX
        - create some more elements and show them on the screen
        - emphasize class name
    - Constructor
        - what does super do?
        - state is an object.
        - react expects it to be named state
        - display information on the screen based off of state
            - uses {}
    - onClick
        - onCLick, make a function console.log when clicked
        - then tie it to setState, increment a number
        - talk about immutability and why we have to go through this process
        - when setState runs it will re run the render method.
    - onChange
        - used on inputs, runs when we type characters
        - generates an event
            - e.target.value
            - value is a property on an HTML element to see what is in the input
        - combine this with setState to put text on the screen
    - .map/list
        - show them how we can dynamically render lists using a map
        - the map returns JSX
        - the array has JSX
        - Can not display an object on the screen
            - json.stringify()
    - Components
        - create a new component that displays basic info
        - Importing Components
        - Must have capitol letter, its how react knows its a component and not a tag
        - export default to get class out of file
        - import to bring it in
        - make the same component but with a functional
        - make the class component have the counter, then put multiple on the screen.
    - Mini Project
        - two inputs and adding items to a list
        - show array immutability, can use push
        - show array spread