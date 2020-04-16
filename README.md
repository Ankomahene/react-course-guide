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
 
 Rendering is when you want to transform your React component into DOM for the browser to understand and display content
 
 React Uses a **Virtual DOM** to render component and that makes it very fast and efficient
 ```js
ReactDOM.render(element, container[, callback])
 ```
 
 >>> Understanding Components
 
 Components are the building blocks of any React app and a typical React app will have many components. They describe how a section of the **UI (User Interface)** should appear.
 
 ```js
 const HelloWorld = () => <h1>Hello World today!</h1>;
 ```
 Notice that the **HelloWorld** component starts with an uppercase, That's the React Standard way of naming components
 
 To types of Component in React
  - Class based Compoent
```js
class HelloWorld extends React.Component {
  render(){
    return <h1>Hello World Today!</h1>;
  }
}
```
These components are created using ES6’s class syntax
They are sometimes referred to as smart, container or stateful components
Read more about Components [here](https://medium.com/the-andela-way/understanding-react-components-37f841c1f3b)
  - (Stateless*) Functional components
```js
const HelloWorld = () => <h1>Hello World today!</h1>;
```
  
There is * on the "Stateless" becuase since introduction of **React-Hooks** (Which will be covered later in the course), they are no more called **Stateless Functional Components** but Just **Functional Component**. We will know WHY later.
Functional Components are sometimes referred to as **-Presentational component**

##### How do I choose which component type to use?
**Use a class component if you:**
+ need to manage local state
+ need to add lifecycle methods to your component
+ need to add logic for event handlers

**Otherwise, always use a functional component.**


 >>> Dynamic and Re-Usable Components
 
 Read more about Components[here](https://medium.com/the-andela-way/understanding-react-components-37f841c1f3b)
 
 >>> Props - Basic usage
 
 Props are React’s way of making components easily and dynamically customisable. They provide a way of passing properties/data down from one component to another, typically from a parent to a child component
 
  >>> Javascript ES6 Aside: **const** and **let**, **arrow functions**
  
  >>> Aside: Javascript Classes
  
  >>> Props - revisit
  
 >>> State
 
 State is like a data store to the ReactJS component. It is mostly used to update the component when the user performs some action like clicking a button.

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

**React Routing**
Routing means Determining What should happen when a user visits a certain page of your site.

We will use **react-router-dom** since we are building web-apps: 


`npm install react-router-dom`

These are the imports you will need, You can also visite the  [API Site](https://reacttraining.com/react-router/web/api/BrowserRouter) to learn more
```js
import {
  BrowserRouter as Router,
  Switch,
  Route,
  Link
} from "react-router-dom";
```
+ Redirects
+ Request parameters
+ Query strings

> Mini Portfolio Project: Using **React Router**

**One Component per file**

**Import and Exports**

**Life cycle Components**

**Event Listeners**

One thing you will always need to do is to listen to events happening on the application and respond to them,events like **clicks, changes, submits, scroll,** etc. 

In React we do that using **onEventName** where _'EventName'_ is the name of the event, e.g. `onClick, onChange, onSubmit, onMouseOver,` etc.

**React Hooks**
[Visit oficial Site](https://reactjs.org/docs/hooks-intro.html) for more on react hooks
- useState

The reason Why **Functional Components** are no more referred to as state the introduction of `useState` in **react-hooks** 
Previously, the only place to use state was **Class Based Components** as Mentioned Earlier.
So In case you create a functional component and realised along the way that you have to manege state in that component, you had to convert your functional component to Class Based Component.
But with the introduction of `useState`, you can now manage state in your funcional components and that has really made our lives a bit more easier.

```js
const[state, setstate] = useState(initialstate);
```
#### Using the state hook
```js
import React, { useState } from 'react';

function Example() {
  const [count, setCount] = useState(0);
  return (
    <div>
      <p>You clicked {count} times</p>
      <button onClick={() => setCount(count + 1)}>
        Click me
      </button>
    </div>
  );
}
```

#### Equivalent Class Example
```js
class Example extends React.Component {
  constructor(props) {
    super(props);
    this.state = {
      count: 0
    };
  }
  render() {
    return (
      <div>
        <p>You clicked {this.state.count} times</p>
        <button onClick={() => this.setState({ count: this.state.count + 1 })}>
          Click me
        </button>
      </div>
    );
  }
}
```
Let's dive into code for more examples

- useEffect

The Effect Hook lets you perform side effects in function components
Data fetching, setting up a subscription, and manually changing the DOM in React components are all examples of side effects.
```js
useEffect(() => {
    //take action here
  });
```
you can think of useEffect Hook as componentDidMount, componentDidUpdate, and componentWillUnmount combined.

- useReducer

PROJECT: Todo Application

##### ADVANCE REACT
___
**React with Redux**



**Using APIs**

PROJECT: API Based Application

