### TURNTABL REACT COURSE
> > > By Shadrack and Christiana

##### INTRODUCTION TO REACT
___
##### What is React?
"React is a declarative, efficient, and flexible JavaScript library for building user interfaces."" [React Official Website](https://reactjs.org/)
- React was Built by Facebook and it makes it simple to create interactive user interfaces.
- It was designed for building **Component-Based** applications.
- From a blogpost By [Log Rocket](https://blog.logrocket.com/state-of-javascript-what-are-the-most-in-demand-frontend-frameworks-in-2020/), React has almost 3 million users and a massive developer community
##### Why Learn React?
**The 'State of Javascript' Report**
shows the most in-demand frontend development frameworks based on factors such as awareness, overall happiness, usage by company size and salary range, show of interest, ease of use.
The report shows that the interest of people in **React** moved from **64 - 71** percent over a period of **12 Months**.

This was the Rank `React -> Vuejs -> Angular -> Preact -> Ember -> Svelte`

Read more from [Log Rocket](https://blog.logrocket.com/state-of-javascript-what-are-the-most-in-demand-frontend-frameworks-in-2020/)

For a more complete outlook on the state of JavaScript in 2020,[Read full report.](https://2019.stateofjs.com/)
###### NB: _Of the roughly 21,000 respondents, only 1,155 — about 6 percent — were female. Unfortunately, this may be reflective of the JavaScript developer ecosystem overall, and it needs to change._

**Online Coding tool** - https://codesandbox.io/s/new

**Practice at home** - https://reactjs.org/tutorial/tutorial.html

**Further Reading** - https://reactjs.org/docs/hello-world.html (Main Concepts)

##### What Should You Know Before Learning React?
+ Basics of html, css
+ Javascript basics [DOM, Functions, Events, others]

NB: Don't Worry, if you don't know any of these, we will explain concepts along the line.

#####  What you Need
- Install [**NodeJS**](https://nodejs.org/en/) and NPM - node package manager
- Install a Text Editor(Your Favorite), We will use [**Visual Studio Code**](https://code.visualstudio.com/)

#### BASIC SETUP
**Using CDN**s
You will need React and ReactDOM

Both React and ReactDOM are available over a CDN.
```js
<script crossorigin src="https://unpkg.com/react@16/umd/react.development.js"></script>
<script crossorigin src="https://unpkg.com/react-dom@16/umd/react-dom.development.js"></script>
```
add the above <script> tags to the HTML page right before the closing </body> tag:
 - Basic Usage with **React.createElement**
 ```js
 var h1 = React.createElement('h1', { className: 'cN' }, 'HELLO REACT!');
 var root = document.getElementById('appRoot');
ReactDOM.render(h1, root);
 ```
 - Introducing **JSX** - Javascript XML
 ```js
 var h1 = <h1>HELLO REACT!</h1>
 ReactDOM.render(h1, document.getElementById('root'));
 ```
 
 >>>  Rendering
 
 >>> Understanding Components
 
 >>> Dynamic and Re-Usable Components
 
 >>> Props - Basic usage
 
  >>> Javascript ES6 Aside: **const** and **let**, **arrow functions**
  
  >>> Aside: Javascript Classes
  
  >>> Props - revisit
  
 >>> States

##### States vrs Props
 Similarities
> Both are object

> Both can be used when rendering

> Changes to both cause re-render

Differences
> Props come from above

> State is defined in component itself
---
>Props Can’t be changed by component itself

> State can be Changed by Component itself 

**Default props Value**

`(Component.defaultProps = {key:value})`

PROJECT: Stop-Watch Application
 
 ##### INTERMEDIATE REACT
___
**Using creat-react-app**
Create React App is an officially supported way to create single-page React applications. It offers a modern build setup with NO CONFIGURATION.[Official Site](https://create-react-app.dev/docs/getting-started/)
```js
npx create-react-app my-app
cd my-app
npm start
```
NB:  If you've previously installed `create-react-app` globally via `npm install -g create-react-app`, we recommend you uninstall the package using `npm uninstall -g create-react-app` to ensure that npx always uses the latest version.


**One Component per file**

**Import and Exports**

**Life cycle Components**

**Event Listeners**

PROJECT: Todo Application

##### ADVANCE REACT
___
**React with Redux**

**React Hooks**

**Using APIs**

PROJECT: API Based Application

