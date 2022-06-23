# CV-html-css
 ## React.js

#### Q1. If you want to import just the Component from the React library, what syntax do you use?

- [ ] `import React.Component from 'react'`
- [ ] `import [ Component ] from 'react'`
- [ ] `import Component from 'react'`
- [x] `import { Component } from 'react'`

#### Q2. If a function component should always render the same way given the same props, what is a simple performance optimization available for it?

- [x] Wrap it in the `React.memo` higher-order component.
- [ ] Implement the `useReducer` Hook.
- [ ] Implement the `useMemo` Hook.
- [ ] Implement the `shouldComponentUpdate` lifecycle method.

#### Q3. How do you fix the syntax error that results from running this code?

```javascript
const person =(firstName, lastName) =>
{
  first: firstName,
  last: lastName
}
console.log(person("Jill", "Wilson"))
```

- [x] Wrap the object in parentheses.
- [ ] Call the function from another file.
- [ ] Add a return statement before the first curly brace.
- [ ] Replace the object with an array.

#### Q4. If you see the following import in a file, what is being used for state management in the component?

`import React, {useState} from 'react';`

- [x] React Hooks
- [ ] stateful components
- [ ] math
- [ ] class components

#### Q5. Using object literal enhancement, you can put values back into an object. When you log person to the console, what is the output?

```javascript
const name = 'Rachel';
const age = 31;
const person = { name, age };
console.log(person);
```

- [ ] `{{name: "Rachel", age: 31}}`
- [x] `{name: "Rachel", age: 31}`
- [ ] `{person: "Rachel", person: 31}}`
- [ ] `{person: {name: "Rachel", age: 31}}`

#### Q6. What is the testing library most often associated with React?

- [ ] Mocha
- [ ] Chai
- [ ] Sinon
- [x] Jest

#### Q7. To get the first item from the array ("cooking") using array destructuring, how do you adjust this line?

```javascript
const topics = ['cooking', 'art', 'history'];
```

- [ ] `const first = ["cooking", "art", "history"]`
- [ ] `const [] = ["cooking", "art", "history"]`
- [ ] `const [, first]["cooking", "art", "history"]`
- [x] `const [first] = ["cooking", "art", "history"]`

#### Q8. How do you handle passing through the component tree without having to pass props down manually at every level?

- [ ] React Send
- [ ] React Pinpoint
- [ ] React Router
- [x] React Context

#### Q9. What should the console read when the following code is run?

```javascript
const [, , animal] = ['Horse', 'Mouse', 'Cat'];
console.log(animal);
```

- [ ] Horse
- [x] Cat
- [ ] Mouse
- [ ] undefined

#### Q10. What is the name of the tool used to take JSX and turn it into createElement calls?

- [ ] JSX Editor
- [ ] ReactDOM
- [ ] Browser Buddy
- [x] Babel

#### Q11. Why might you use useReducer over useState in a React component?

- [ ] when you want to replace Redux
- [x] when you need to manage more complex state in an app
- [ ] when you want to improve performance
- [ ] when you want to break your production app

#### Q12. Which props from the props object is available to the component with the following syntax?

```javascript
<Message {...props} />
```

- [ ] any that have not changed
- [x] all of them
- [ ] child props
- [ ] any that have changed

#### Q13. Consider the following code from React Router. What do you call :id in the path prop?

```javascript
<Route path="/:id" />
```

- [ ] This is a route modal
- [x] This is a route parameter
- [ ] This is a route splitter
- [ ] This is a route link

#### Q14. If you created a component called Dish and rendered it to the DOM, what type of element would be rendered?

```javascript
function Dish() {
  return <h1>Mac and Cheese</h1>;
}

ReactDOM.render(<Dish />, document.getElementById('root'));
```

- [ ] `div`
- [ ] section
- [ ] component
- [x] `h1`

#### Q15. What does this React element look like given the following function? (Alternative: Given the following code, what does this React element look like?)

```javascript
React.createElement('h1', null, "What's happening?");
```

- [ ] `<h1 props={null}>What's happening?</h1>`
- [x] `<h1>What's happening?</h1>`
- [ ] `<h1 id="component">What's happening?</h1>`
- [ ] `<h1 id="element">What's happening?</h1>`

#### Q16. What property do you need to add to the Suspense component in order to display a spinner or loading state?

```javascript
function MyComponent() {
  return (
    <Suspense>
      <div>
        <Message />
      </div>
    </Suspense>
  );
}
```

- [ ] lazy
- [ ] loading
- [x] fallback
- [ ] spinner

#### Q17. What do you call the message wrapped in curly braces below?

```javascript
const message = 'Hi there';
const element = <p>{message}</p>;
```

- [ ] a JS function
- [ ] a JS element
- [x] a JS expression
- [ ] a JSX wrapper

#### Q18. What can you use to handle code splitting?

- [ ] `React.memo`
- [ ] `React.split`
- [x] `React.lazy`
- [ ] `React.fallback`

#### Q19. When do you use `useLayoutEffect`?

- [ ] to optimize for all devices
- [ ] to complete the update
- [ ] to change the layout of the screen
- [x] when you need the browser to paint before the effect runs

#### Q20. What is the difference between the click behaviors of these two buttons (assuming that this.handleClick is bound correctly)?

```javascript
A. <button onClick={this.handleClick}>Click Me</button>
B. <button onClick={event => this.handleClick(event)}>Click Me</button>
```

- [ ] Button A will not have access to the event object on click of the button.
- [ ] Button B will not fire the handler this.handleClick successfully.
- [ ] Button A will not fire the handler this.handleClick successfully.
- [x] There is no difference.

#### Q21. How do you destructure the properties that are sent to the Dish component?

```javascript
function Dish(props) {
  return (
    <h1>
      {props.name} {props.cookingTime}
    </h1>
  );
}
```

- [ ] `function Dish([name, cookingTime]) { return <h1>{name} {cookingTime}</h1>; }`
- [x] `function Dish({name, cookingTime}) { return <h1>{name} {cookingTime}</h1>; }`
- [ ] `function Dish(props) { return <h1>{name} {cookingTime}</h1>; }`
- [ ] `function Dish(...props) { return <h1>{name} {cookingTime}</h1>; }`

#### Q22. When might you use `React.PureComponent`?

- [ ] when you do not want your component to have props
- [ ] when you have sibling components that need to be compared
- [x] when you want a default implementation of `shouldComponentUpdate()`
- [ ] when you do not want your component to have state

#### Q23. Why is it important to avoid copying the values of props into a component's state where possible?

- [ ] because you should never mutate state
- [ ] because `getDerivedStateFromProps()` is an unsafe method to use
- [x] because you want to allow a component to update in response to changes in the props
- [ ] because you want to allow data to flow back up to the parent

#### Q24. What is the children prop?

- [ ] a property that adds child components to state
- [x] a property that lets you pass components as data to other components
- [ ] a property that lets you set an array as a property
- [ ] a property that lets you pass data to child elements

#### Q25. Which attribute do you use to replace innerHTML in the browser DOM?

- [ ] injectHTML
- [x] dangerouslySetInnerHTML
- [ ] weirdSetInnerHTML
- [ ] strangeHTML

#### Q26. Which of these terms commonly describe React applications?

- [x] declarative
- [ ] integrated
- [ ] closed
- [ ] imperative

#### Q27. When using webpack, why would you need to use a loader?

- [ ] to put together physical file folders
- [x] to preprocess files
- [ ] to load external data
- [ ] to load the website into everyone's phone

#### Q28. A representation of a user interface that is kept in memory and is synced with the "real" DOM is called what?

- [x] virtual DOM
- [ ] DOM
- [ ] virtual elements
- [ ] shadow DOM

#### Q29. You have written the following code but nothing is rendering. How do you fix this problem?

```javascript
const Heading = () => {
  <h1>Hello!</h1>;
};
```

- [ ] Add a render function.
- [x] Change the curly braces to parentheses or add a return statement before the `h1` tag.
- [ ] Move the `h1` to another component.
- [ ] Surround the `h1` in a `div`.

#### Q30. To create a constant in JavaScript, which keyword do you use?

- [x] const
- [ ] let
- [ ] constant
- [ ] var

#### Q31. What do you call a React component that catches JavaScript errors anywhere in the child component tree?

- [ ] error bosses
- [ ] error catchers
- [ ] error helpers
- [x] error boundaries

#### Q32. In which lifecycle method do you make requests for data in a class component?

- [ ] constructor
- [x] componentDidMount
- [ ] componentWillReceiveProps
- [ ] componentWillMount

#### Q33. React components are composed to create a user interface. How are components composed?

- [ ] by putting them in the same file
- [x] by nesting components
- [ ] with webpack
- [ ] with code splitting

#### Q34. All React components must act like **\_** with respect to their props.

- [ ] monads
- [x] pure functions
- [ ] recursive functions
- [ ] higher-order functions

#### Q35. What is `[e.target.id]` called in the following code snippet?

```javascript
handleChange(e) {
  this.setState({ [e.target.id]: e.target.value })
}
```

- [ ] a computed property name
- [ ] a set value
- [x] a dynamic key
- [ ] a JSX code string

#### Q36. What is the name of this component?

```javascript
class Clock extends React.Component {
  render() {
    return <h1>Look at the time: {time}</h1>;
  }
}
```

- [x] Clock
- [ ] It does not have a name prop.
- [ ] React.Component
- [ ] Component

#### Q37. What is sent to an `Array.map()` function?

- [x] a callback function that is called once for each element in the array
- [ ] the name of another array to iterate over
- [ ] the number of times you want to call the function
- [ ] a string describing what the function should do

#### Q38. Why is it a good idea to pass a function to `setState` instead of an object?

- [ ] It provides better encapsulation.
- [ ] It makes sure that the object is not mutated.
- [ ] It automatically updates a component.
- [x] `setState` is asynchronous and might result in out of sync values.

**Explanation:** Because `this.props` and `this.state` may be updated asynchronously, you should not rely on their values for calculating the next state.
Read [this article](https://medium.com/@wisecobbler/using-a-function-in-setstate-instead-of-an-object-1f5cfd6e55d1)

#### Q39. What package contains the render() function that renders a React element tree to the DOM?

- [ ] `React`
- [x] `ReactDOM`
- [ ] `Render`
- [ ] `DOM`

#### Q40. How do you set a default value for an uncontrolled form field?

- [ ] Use the `value` property.
- [x] Use the `defaultValue` property.
- [ ] Use the `default` property.
- [ ] It assigns one automatically.

#### Q41. What do you need to change about this code to get it to run?

```js
class clock extends React.Component {
  render() {
    return <h1>Look at the time: {this.props.time}</h1>;
  }
}
```

- [ ] Add quotes around the return value
- [ ] Remove `this`
- [ ] Remove the render method
- [x] Capitalize `clock`

**Explanation:** In JSX, lower-case tag names are considered to be HTML tags.
Read [this article](https://reactjs.org/docs/jsx-in-depth.html#html-tags-vs.-react-components)

#### Q42. Which Hook could be used to update the document's title?

- [x] `useEffect(function updateTitle() { document.title = name + ' ' + lastname; });`
- [ ] `useEffect(() => { title = name + ' ' + lastname; });`
- [ ] `useEffect(function updateTitle() { name + ' ' + lastname; });`
- [ ] `useEffect(function updateTitle() { title = name + ' ' + lastname; });`

#### Q43. What can you use to wrap Component imports in order to load them lazily?

- [ ] `React.fallback`
- [ ] `React.split`
- [x] `React.lazy`
- [ ] `React.memo`

#### Q44. How do you invoke setDone only when component mounts, using hooks?

```javascript
function MyComponent(props) {
  const [done, setDone] = useState(false);

  return <h1>Done: {done}</h1>;
}
```

- [ ] `useEffect(() => { setDone(true); });`
- [x] `useEffect(() => { setDone(true); }, []);`
- [ ] `useEffect(() => { setDone(true); }, [setDone]);`
- [ ] `useEffect(() => { setDone(true); }, [done, setDone]);`

#### Q45. Currently, `handleClick` is being called instead of passed as a reference. How do you fix this?

```javascript
<button onClick={this.handleClick()}>Click this</button>
```

- [ ] `<button onClick={this.handleClick.bind(handleClick)}>Click this</button>`
- [ ] `<button onClick={handleClick()}>Click this</button>`
- [x] `<button onClick={this.handleClick}>Click this</button>`
- [ ] `<button onclick={this.handleClick}>Click this</button>`

#### Q46. Which answer best describes a function component?

- [ ] A function component is the same as a class component.
- [x] A function component accepts a single props object and returns a React element.
- [ ] A function component is the only way to create a component.
- [ ] A function component is required to create a React component.

#### Q47. Which library does the `fetch()` function come from?

- [ ] FetchJS
- [ ] ReactDOM
- [x] No library. `fetch()` is supported by most browsers.
- [ ] React

#### Q48. What will happen when this useEffect Hook is executed, assuming name is not already equal to John?

```javascript
useEffect(() => {
  setName('John');
}, [name]);
```

- [ ] It will cause an error immediately.
- [ ] It will execute the code inside the function, but only after waiting to ensure that no other component is accessing the name variable.
- [x] It will update the value of name once and not run again until name is changed from the outside.
- [ ] It will cause an infinite loop.

#### Q49. Which choice will not cause a React component to rerender?

- [ ] if the component calls `this.setState(...)`
- [ ] the value of one of the component's props changes
- [ ] if the component calls `this.forceUpdate()`
- [x] one of the component's siblings rerenders

#### Q50. You have created a new method in a class component called handleClick, but it is not working. Which code is missing?

```javascript
class Button extends React.Component{

  constructor(props) {
    super(props);
    // Missing line
  }

  handleClick() {...}
}
```

- [ ] `this.handleClick.bind(this);`
- [ ] `props.bind(handleClick);`
- [ ] `this.handleClick.bind();`
- [x] `this.handleClick = this.handleClick.bind(this);`

#### Q51. React does not render two sibling elements unless they are wrapped in a fragment. Below is one way to render a fragment. What is the shorthand for this?

```javascript
<React.Fragment>
  <h1>Our Staff</h1>
  <p>Our staff is available 9-5 to answer your questions</p>
</React.Fragment>
```

- [ ] A

```javascript
<...>
  <h1>Our Staff</h1>
  <p>Our staff is available 9-5 to answer your questions</p>
</...>
```

- [ ] B

```javascript
<//>
  <h1>Our Staff</h1>
  <p>Our staff is available 9-5 to answer your questions</p>
<///>
```

- [x] C

```javascript
<>
  <h1>Our Staff</h1>
  <p>Our staff is available 9-5 to answer your questions</p>
</>
```

- [ ] D

```javascript
<Frag>
  <h1>Our Staff</h1>
  <p>Our staff is available 9-5 to answer your questions</p>
</Frag>
```

#### Q52. If you wanted to display the count state value in the component, what do you need to add to the curly braces in the `h1`?

```javascript
class Ticker extends React.component {
  constructor(props) {
    super(props);
    this.state = { count: 0 };
  }
  render() {
    return <h1>{}</h1>;
  }
}
```

- [x] this.state.count
- [ ] count
- [ ] state
- [ ] state.count

#### Q53. Per the following code, when is the Hello component displayed?

```javascript
const greeting = isLoggedIn ? <Hello /> : null;
```

- [ ] never
- [x] when `isLoggedIn` is true
- [ ] when a user logs in
- [ ] when the Hello function is called

#### Q54. In the following code block, what type is orderNumber?

```javascript
ReactDOM.render(<Message orderNumber="16" />, document.getElementById('root'));
```

- [x] string
- [ ] boolean
- [ ] object
- [ ] number

#### Q55. You have added a style property to the `h1` but there is an unexpected token error when it runs. How do you fix this?

```javascript
const element = <h1 style={ backgroundColor: "blue" }>Hi</h1>;
```

- [ ] `const element = <h1 style="backgroundColor: "blue""}>Hi</h1>;`
- [x] `const element = <h1 style={{backgroundColor: "blue"}}>Hi</h1>;`
- [ ] `const element = <h1 style={blue}>Hi</h1>;`
- [ ] `const element = <h1 style="blue">Hi</h1>;`

#### Q56. Which function is used to update state variables in a React class component?

- [ ] `replaceState`
- [ ] `refreshState`
- [ ] `updateState`
- [x] `setState`

#### Q57. Consider the following component. What is the default color for the star?

```javascript
const Star = ({ selected = false }) => <Icon color={selected ? 'red' : 'grey'} />;
```

- [ ] black
- [ ] red
- [x] grey
- [ ] white

#### Q58. What is the difference between the click behaviors of these two buttons(assuming that this.handleClick is bound correctly)

```javascript
  A. <button onClick=this.handleClick>Click Me</button>
  B. <button onClick={event => this.handleClick(event)}>Click Me</button>
```

- [ ] `Button A will not have access to the event object on click of the button`
- [x] `Button A will not fire the handler this.handleClick successfully`
- [ ] `There is no difference`
- [ ] `Button B will not fire the handler this.handleClick successfully`

#### Q59. How would you add to this code, from React Router, to display a component called About?

```javascript
<Route path="/:id" />
```

- [x] A

```javascript
<Route path="/:id">
  {' '}
  <About />
</Route>
```

- [ ] B

```javascript
<Route path="/tid" about={Component} />
```

- [ ] C

```javascript
<Route path="/:id" route={About} />
```

- [ ] D

```javascript
<Route>
  <About path="/:id" />
</Route>
```

#### Q60. Which class-based component is equivalent to this function component?

```javascript
const Greeting = ({ name }) => <h1>Hello {name}!</h1>;
```

- [ ] A

```javascript
class Greeting extends React.Component {
  constructor() {
    return <h1>Hello {this.props.name}!</h1>;
  }
}
```

- [ ] B

```javascript
class Greeting extends React.Component {
  <h1>Hello {this.props.name}!</h1>;
}
```

- [x] C

```javascript
class Greeting extends React.Component {
  render() {
    return <h1>Hello {this.props.name}!</h1>;
  }
}
```

- [ ] D

```javascript
class Greeting extends React.Component {
  render({ name }) {
    return <h1>Hello {name}!</h1>;
  }
}
```

#### Q61. Give the code below, what does the second argument that is sent to the render function describe?

```javascript
ReactDOM.render(
  <h1>Hi<h1>,
    document.getElementById('root')
)
```

- [x] where the React element should be added to the DOM
- [ ] where to call the function
- [ ] where the root component is
- [ ] where to create a new JavaScript file

#### Q62. Why should you use React Router's Link component instead of a basic `<a>` tag in React?

- [ ] The link component allows the user to use the browser's `Back` button.
- [ ] There is no difference--the `Link` component is just another name for the `<a>` tag.
- [ ] The `<a>` tag will cause an error when used in React.
- [x] The `<a>` tag triggers a full page reload, while the `Link` component does not.

#### Q63. What is the first argument, `x`, that is sent to the `createElement` function?

```javascript
React.createElement(x, y, z);
```

- [x] the element that should be created
- [ ] the order in which this element should be placed on the page
- [ ] the properties of the element
- [ ] data that should be displayed in the element

#### Q64. Which class-based lifecycle method would be called at the same time as this effect Hook?

```javascript
useEffect(() => {
  // do things
}, []);
```

- [ ] componentWillUnmount
- [x] componentDidMount
- [ ] render
- [ ] componentDidUpdate

#### Q65. What is the name of this component?

```javascript
class Comp extends React.Component {
  render() {
    return <h1>Look at the time: {time}</h1>;
  }
}
```

- [x] Comp
- [ ] h1
- [ ] React.Component
- [ ] Component

This question might be an updated version of Q37.

#### Q66. When using a portal, what is the first argument?

```javascript
ReactDOM.createPortal(x, y);
```

- [ ] the current state
- [x] the element to render
- [ ] the App component
- [ ] the page

**Explanation:**
From official docs: [Portals](https://reactjs.org/docs/portals.html)

#### Q67. What is `setCount`?

```javascript
const [count, setCount] = useState(0);
```

- [ ] the initial state value
- [ ] a variable
- [ ] a state object
- [x] a function to update the state

**Reference:**
From official docs: [Hooks-State](https://reactjs.org/docs/hooks-state.html#:~:text=If%20we%20want%20to%20update%20the%20current)

#### Q68. What is the use of map function below?

```javascript
const database = [user1:{},user2:{},user3:{}];
database.map((user)=><h1>user.data</h1>);
```

- [ ] gives a map of all the entries in database
- [x] returns a heading tag for every entry in the database containing it's data
- [ ] returns one heading tag for all the entries in database
- [ ] checks which entry in the database is suitable for heading tag

#### Q69. Describe what is happening in this code?

```javascript
const { name: firstName } = person;
```

- [ ] It is creating a new object that contains the same name property as the person object.
- [ ] It is assigning the value of the person object's firstName property to a constant called name.
- [ ] It is retrieving the value of person.name.firstName.
- [x] It is assigning the value of the person object's name property to a constant called firstName.

#### Q70. What is wrong with this code?

```javascript
const MyComponent = ({ names }) => (
  <h1>Hello</h1>
  <p>Hello again</p>
);
```

- [ ] React components cannot be defined using functions.
- [x] React does not allow components to return more than one element.
- [ ] The component needs to use the return keyword.
- [ ] String literals must be surrounded by quotes.

#### Q71. When using a portal, what is the second argument?

```javascript
ReactDOM.createPortal(x, y);
```

- [ ] the App component
- [ ] the page
- [ ] the current state
- [x] the DOM element that exists outside of the parent component

#### Q72. Given this code, what will be printed in the `<h1>` tag?

```javascript
const MyComponent = ({ children }) => (
  <h1>{children.length}</h1>
);
...
<MyComponent>
<p>Hello</p>
<p>Goodbye</p>
</MyComponent>
```

- [ ] It will produce an error saying "cannot read property "length" of undefined."
- [ ] 1
- [ ] undefined
- [x] 2

#### Q73. What is this pattern called?

```javascript
const [count, setCount] = useState(0);
```

- [ ] object destructuring
- [x] array destructuring
- [ ] spread operating
- [ ] code pushing

#### Q74. What is the first file loaded by the browser in a basic React project?

- [ ] src/App.js
- [ ] src/index.js
- [ ] public/manifest.json
- [x] public/index.html

#### Q75. The code below is rendering nothing, and there is an error that says "ReactDOM is not defined." How do you fix this issue?

```javascript
import React from 'react';
import { render } from 'react-dom';

const element = <h1>Hi</h1>;

ReactDOM.render(element, document.getElementById('root'));
```

- [x] `render(element, document.getElementById("root"));`
- [ ] `ReactDOM(element, document.getElementById("root"));`
- [ ] `renderDOM(element, document.getElementById("root"));`
- [ ] `DOM(element, document.getElementById("root"));`

#### Q76. In this component, how do you display whether the user was logged in or not?

```javascript
render() {
  const isLoggedIn = this.state.isLoggedIn;
  return (
    <div>
      The user is:
    </div>
  );
}
```

- [ ] `The user is loggedIn ? logged in : not logged in.`
- [ ] Write a function to check the login status.
- [ ] `The user is {isLoggedIn = "no"}.`
- [x] `The user is {isLoggedIn ? "logged in." : "not logged in"}.`

#### Q77. You are rendering a list with React when this warning appears in the console: "Warning: Each child in a list should have a unique 'key' prop." How do you fix this issue?

- [ ] Pass the name of each item as its key.
- [ ] Add a key prop with the same value to each item the list.
- [ ] Clear the console warnings.
- [x] When iterating over the list items, add a unique property to each list item.

#### Q78. How would you generate the boilerplate code for a new app that you are building to collect underpants?

- [ ] npm create-react-app collect-underpants
- [ ] npx start-app collect-underpants
- [ ] react new collect-underpants
- [x] npx create-react-app collect-underpants

[Source: React Docs](https://reactjs.org/docs/create-a-new-react-app.html#create-react-app)

#### Q79. Add the code that will fire the photon torpedoes when the button is clicked.

```javascript
class StarTrekkin extends React.Component {
  firePhotonTorpedoes(e) {
    console.log('pew pew');
  }
  render() {
    return; // Missing code
  }
}
```

- [ ] `<button onClick={firePhotonTorpedoes()}>Pew Pew</button>`
- [ ] `<button onClick={firePhotonTorpedoes}>Pew Pew</button>`
- [ ] `<button onClick={this.firePhotonTorpedoes()}>Pew Pew</button>`
- [x] `<button onClick={this.firePhotonTorpedoes}>Pew Pew</button>`

[Source: React Docs](https://reactjs.org/docs/handling-events.html)

#### Q80. What is the process of deciding whether an update is necessary?

- [ ] shadow DOM
- [ ] fiber
- [x] reconciliation
- [ ] setting state

#### Q81. React is an open-source project but is maintained by which company?

- [ ] Intuit
- [ ] Twitter
- [x] Facebook
- [ ] Snapchat

#### Q82. What command can you use to generate a React project?

- [ ] react-starter
- [x] create-react-app
- [ ] react-gen
- [ ] react-start

#### Q83. What is the browser extension called that React developers use to debug applications?

- [x] React Developer Tools
- [ ] React Tooling Add-on
- [ ] React Codewatch
- [ ] React Debug

#### Q84. Which tool is not part of Create React App?

- [ ] React
- [x] jQuery
- [ ] webpack
- [ ] ReactDOM

#### Q85. What is the JavaScript syntax extension that is commonly used to create React elements?

- [ ] HTML
- [ ] JavaScriptX
- [x] JSX
- [ ] React JavaScript

#### Q86. How might you check property types without using Flow or TypeScript?

- [ ] Check Manually.
- [ ] Use `prop-helper`.
- [x] use `prop-types`.
- [ ] user `checker-types`.

#### Q87. How do you add an id of heading to the following h1 element?

`let dish = <h1>Mac and Cheese</h1>; `

- [ ] `let dish = <h1 id={heading}>Mac and Cheese</h1>;`
- [x] `let dish = <h1 id="heading">Mac and Cheese</h1>;`
- [ ] `let dish = <h1 id:"heading">Mac and Cheese</h1>;`
- [ ] `let dish = <h1 class="heading">Mac and Cheese</h1>;`

#### Q88. What value of button will allow you to pass the name of the person to be hugged?

```
class Huggable extends React.Component {
  hug(id) {
    console.log("hugging " + id);
  }
  render() {
    let name = "kitten";
    let button = // Missing code
    return button;
  }
}
```

- [ ] `<button onClick={(name) => this.hug(name)}>Hug Button</button>;`
- [ ] `<button onClick={this.hug(e, name)}>Hug Button</button>;`
- [ ] `<button onClick={(e) => hug(name, e)}>Hug Button</button>;`
- [x] `<button onClick={(e) => this.hug(name, e)}>Hug Button</button>;`

**Explanation:**
This question test knowledge of react class components. You need to use `this` in order to call methods declared inside class components.

#### Q89. What syntax do you use to create a component in React?

- [ ] a generator
- [x] a function or a class
- [ ] a service worker
- [ ] a tag

`React Components are like functions that return HTML elements. Components are independent and reusable bits of code. They serve the same purpose as JavaScript functions, but work in isolation and return HTML. Components come in two types, Class components and Function components.` [(Source)](https://reactjs.org/docs/components-and-props.html)

#### Q90. You want to disable a button so that it does not emit any events onClick. Which prop do you use to acomplish this?

- [ ] onBlur
- [ ] onPress
- [ ] defaultValue
- [x] disabled

#### Q91. In this function, which is the best way to describe the Dish component?

```
function Dish() {
  return (
    <>
      <Ingredient />
      <Ingredient />
    </>
  );
}
```

- [ ] child component
- [x] parent component
- [ ] nested component
- [ ] sibling component

#### Q92. When does the componentDidMount function fire?

- [x] right after the component is added to the DOM
- [ ] before the component is added to the DOM
- [ ] right after the component is updated
- [ ] right after an API call

#### Q93. What might you use webpack for?

- [ ] to fetch remote dependencies used by your app
- [x] to split your app into smaller chunks that can be more easily loaded by the browser
- [ ] to format your code so that it is more readable
- [ ] to ensure your app is not vulnerable to code injection

#### Q94. When using the React Developer Tools Chrome extension, what does it mean if the React icon is red?

- [x] You are using the development build of React.
- [ ] You are using the production build of React.
- [ ] You are using webpack.
- [ ] You are using Create React App.

[Reference](https://teamtreehouse.com/community/hey-why-the-logo-of-react-developer-tools-appears-in-red)

#### Q95. How would you modify the constructor to fix this error: "ReferenceError: Must call super constructor in derived class before accessing 'this'..."?

```
class TransIsBeautiful extends React.Component {
  constructor(props){
  // Missing line
  console.log(this) ;
  }
  ...
}
```

- [ ] render(props);
- [x] super(props);
- [ ] super(this);
- [ ] this.super();

#### Q96. Which language can you not use with React?

- [x] Swift.
- [ ] JSX.
- [ ] Javascipt.
- [ ] TypeScript.

#### Q97. This code is part of an app that collects Pokemon. How would you print the list of the ones collected so far?

```javascript
constructor(props) {
    super(props);
    this.state = {
        pokeDex: []
    };
}
```

- [ ] console.log(props.pokeDex);
- [ ] console.log(this.props.pokeDex);
- [ ] console.log(pokeDex);
- [x] console.log(this.state.pokeDex);

[Reference](https://www.digitalocean.com/community/tutorials/how-to-manage-state-on-react-class-components#step-3-setting-state-from-a-static-value)

#### Q98. What would be the result of running this code?

```javascript
function add(x = 1, y = 2) {
  return x + y;
}

add();
```

- [ ] null
- [x] 3
- [ ] 0
- [ ] undefined

![image](https://user-images.githubusercontent.com/62549240/160531605-bf8790d5-5eb9-4291-a9bd-4232f2fd7b6e.png)

#### Q99. Why might you use a React.ref?

- [ ] to refer to another JS file
- [ ] to bind the function
- [ ] to call a function
- [x] to directly access the DOM node

[Reference](https://reactjs.org/docs/refs-and-the-dom.html)

#### Q100. What pattern is being used in this code?

```javascript
const { tree, lake } = nature;
```

- [ ] function defaults
- [ ] array destructuring
- [ ] PRPL pattern
- [x] destructuring assignment

[Reference](https://javascript.info/destructuring-assignment)
## HTML

#### Q1. What is the purpose of the `<track>` tag, and when should it be used?

- [ ] The `<track>` tag is used for specifying subtitles. It is typically applied as a child of the `<audio>` and `<video>` tags.
- [ ] The `<track>` tag is used for specifying subtitles. It is typically applied as a child of the `<video>` tag.
- [ ] The `<track>` tag is used for specifying subtitles, captions, and other types of time-based text. It is typically applied as a child of the `<video>` tag.
- [x] The `<track>` tag is used for specifying subtitles, captions, and other types of time-based text. It is typically applied as a child of the `<audio>` and `<video>` tag.

#### Q2. What are the best examples of void elements?

- [ ] `<link><meta><title>`
- [x] `<br><base><source>`
- [ ] `<input><br><p>`
- [ ] `<area><embed><strong>`

#### Q3. In HTML5, which tag or tags embed a webpage inside of a webpage?

- [ ] `<iframe>, <frame>, and <frameset>`
- [ ] `<frame>`
- [x] `<iframe>`
- [ ] `<frame> and <frameset>`

#### Q4. Where do `<header>` and `<footer>` tags typically occur?

- [ ] as children of `<body>, <article>, <aside>, and <section>` tags
- [x] as children of `<body>, <article>, and <section>` tags
- [ ] as children of `<body>, <article>, <aside>, <nav>, and <section>` tags
- [ ] as children of `<body>, <article>, <table>, and <section>` tags

#### Q5. What is the best way to apply bold styling to text?

- [x] `<strong>`
- [ ] Use CSS.
- [ ] `<bold>`
- [ ] `<b>`

#### Q6. When is the `<link>` tag used?

- [ ] when linking style sheets, JavaScript, and icons for mobile apps
- [x] when linking style sheets, favicons, and preloading assets
- [ ] when linking one webpage to another
- [ ] when linking style sheets, external URLs, and favicons

#### Q7. What should fill the two blanks in the HTML code below?

```html
<address ______ _____>
  <span itemprop="streetAddress">6410 Via Real</span><br />
  <span itemprop="addressLocality">Carpinteria</span>,
  <span itemprop="addressRegion">CA</span>
  <span itemprop="addressCode">93013</span>
</address>
```

- [x] `itemscope` `itemtype="http://schema.org/PostalAddress"`
- [ ] `itemsref="http://schema.org/PostalAddress"` `itemid="address"`
- [ ] `itemscope` `itemref="http://schema.org/PostalAddress"`
- [ ] `itemid="address"` `itemtype="http://schema.org/PostalAddress"`

#### Q8. When should you use the `<aside>` element?

- [x] when the content can be removed without detracting from the page's message
- [ ] for anything you want to move to the side, like a pull quote box, a sidebar, or an image with text wrapping around it
- [ ] for anything in parentheses
- [ ] for anything in a sidebar

#### Q9. With which tags is the `<source>` element associated?

- [ ] `<svg>, <picture>, <audio>, and <video>`
- [x] `<picture>, <audio>, and <video>`
- [ ] It is interchangeable with the `src` attribute, so any element which uses `src` may use `<source>`
- [ ] `<audio> and <video>`

#### Q10. What is NOT a valid attribute for the `<textarea>` element?

- [ ] readonly
- [x] max
- [ ] form
- [ ] spellcheck

#### Q11. What is the best way to code the sample shown?

![Sample text](images/ss-2.png?raw=true)

- [ ] A

```html
<details>
  <summary>Parmesan Deviled Eggs</summary>
  <p>
    These delectable little bites are made with organic eggs, fresh Parmesan, and chopped pine nuts.
  </p>
</details>
```

- [ ] B

```html
<h4>▸ Parmesan Deviled Eggs</h4>
<p>
  These delectable little bites are made with organic eggs, fresh Parmesan, and chopped pine nuts.
</p>
```

- [x] C

```html
<details open>
  <summary>Parmesan Deviled Eggs</summary>
  <p>
    These delectable little bites are made with organic eggs, fresh Parmesan, and chopped pine nuts.
  </p>
</details>
```

- [ ] D

```html
<details>
  <h4>▸ Parmesan Deviled Eggs</h4>
  <p>
    These delectable little bites are made with organic eggs, fresh Parmesan, and chopped pine nuts.
  </p>
</details>
```

#### Q12. What is the purpose of the `<samp>` element?

- [ ] It connects the web browser to a SA-MP server.
- [ ] It identifies enclosed text as a sampler or an example.
- [x] It identifies sample output from a computer program.
- [ ] It uses a simple application messaging protocol to connect the browser to a texting device.

#### Q13. When should you use `<ol>` and `<ul>` elements?

- [x] Use `<ul>` when you want a bulleted list and `<ol>` when you want a numbered list.
- [ ] Use `<ul>` when you have a list of items in which the order of the items matters. Use `<ol>` when you have a list of items that could go in any order.
- [ ] Use `<ol>` when you want a bulleted list and `<ul>` when you want a numbered list.
- [ ] Use `<ol>` when you have a list of items in which the order of the items matters. Use `<ul>` when you have a list of items that could go in any order.

#### Q14. What is the difference between the post and get methods in a form?

- [ ] post is used for sending information to the server. get is used for retrieving form information from the server.
- [ ] get is used for sending information to the server. post is used for retrieving form information from the server.
- [ ] With get, data is included in the form body when send to the server. With post, the data goes through the URL.
- [x] With post, data is included in the form body when send to the server. With get, the data goes through the URL.

#### Q15. What is the difference between the `<div>` and `<span>` tags?

- [x] `<div>` is used where a generic block-level tag is needed, while `<span>` is used where a generic inline tag is needed.
- [ ] `<div>` is used for major divisions on a page, while `<span>` is used to span across columns.
- [ ] `<div>` is the industry-standard default tag, but you could use `<span>` if you prefer.
- [ ] `<div>` is used where a generic inline tag is needed, while `<span>` is used where a generic block-level tag is needed.

#### Q16. What should fill the blank in the HTML code bellow?

```html
<form method="post" action="mailto:info@linkedin.com" ____="text/plain"></form>
```

- [x] enctype
- [ ] media
- [ ] type
- [ ] rel

#### Q17. What is the correct markup for `alt` attribute of an image?

- [ ] A

```html
<img src="cubism.jpg" alt="Version of ""Whistler's Mother"" in cubist style">
```

- [ ] B

```html
<img src="cubism.jpg" alt="Version of "Whistler's Mother" in cubist style">
```

- [x] C

```html
<img src="cubism.jpg" alt='Version of "Whistler\'s Mother" in cubist style'>
```

- [ ] D

```html
<img src="cubism.jpg" alt="Version of \"Whistler's Mother\" in cubist style">
```

#### Q18. In the code below, what is the purpose of the **id** attribute?

```html
<p id="warning">Be careful when installing this product.</p>
```

- [x] It establishes that id is a unique identifier in the document, used for styling CSS, scripting, and linking within a webpage.
- [ ] It establishes that id is a unique identifier in the document, used for styling CSS and with Javascript code.
- [ ] It establishes that id may be used for styling CSS several times per page.
- [ ] It establishes that id is a unique identifier in the website, used for styling CSS, scripting, and linking within a webpage.

#### Q19. What is the best semantic markup for the sentence shown?

```markdown
On July 21, 1969, Neil Armstrong said, "One small step for man, one giant leap for mankind."
```

- [x] A

```markdown
<p>
  On <time datetime="1969-07-21">July 21, 1969</time>, Neil Armstrong said,
  <q cite="https://www.hq.nasa.gov/alsj/a11l/a11.html"
    >One small step for man, one giant leap for mankind.</q
  >
</p>
```

- [ ] B

```markdown
<p>
  On July 21, 1969, Neil Armstrong said,
  <q cite="https://www.hq.nasa.gov/alsj/a11l/a11.html"
    >One small step for man, one giant leap for mankind.</q
  >
</p>
```

- [ ] C

```markdown
<p>
  On July 21, 1969, Neil Armstrong said, <q>One small step for man, one giant leap for mankind.</q>
</p>
```

- [ ] D

```markdown
<p>
  On <time datetime="07-21-1969">July 21, 1969</time>, Neil Armstrong said,
  <q cite="https://www.hq.nasa.gov/alsj/a11l/a11.html"
    >One small step for man, one giant leap for mankind.</q
  >
</p>
```

#### Q20. What should fill the blank in this HTML code?

```html
<a href="https://es.yahoo.com/" hreflang="____" target="_blank">Visita Yahoo</a>
```

- [ ] es
- [ ] es-spanish
- [x] es-es
- [ ] spanish

#### Q21. Review the text in the red box in the image shown. What is the best way to code this in HTML?

![Image of footer](images/ss-3.png?raw=true)

- [ ] ordered list
- [x] unordered list inside a nav element
- [ ] ordered list inside a nav element
- [ ] unordered list

#### Q22. What is the best way to code three choices within a form so that the user can select only one item?

- [ ] A

```markdown
<label for="example">Make a choice:</label>
<datalist id="example">

  <option value="Choice 1"></option>
  <option value="Choice 2"></option>
  <option value="Choice 3"></option>
</datalist>
```

- [ ] B

```markdown
<p>Make a choice:</p>
<input id="choices" name="example" />

<datalist value="choices">
  <option value="Choice 1"></option>
  <option value="Choice 2"></option>
  <option value="Choice 3"></option>
</datalist>
```

- [ ] C

```markdown
<label for="example">Make a choice:</label>
<input list="example" id="choices" name="choices" />

<datalist id="choices">
  <option value="Choice 1">Choice 1</option>
  <option value="Choice 2">Choice 2</option>
  <option value="Choice 3">Choice 3</option>
</datalist>
```

- [x] D

```markdown
<label for="example">Make a choice:</label>
<input list="choices" id="example" name="example" />

<datalist id="choices">
  <option value="Choice 1"></option>
  <option value="Choice 2"></option>
  <option value="Choice 3"></option>
</datalist>
```

#### Q23. How do you confirm that a document is written in HTML5?

- [ ] The server wraps the webpage in an HTML5 wrapper.
- [x] Use the `<!DOCTYPE html>` declaration that starts the document.
- [ ] The browser receives encoding from the server to display the document with HTML5.
- [ ] It is enclosed in a `<html>` tag.

#### Q24. What does the code shown below accomplish?

```html
<picture>
  <source srcset="image1.jpg" media="(min-width: 1000px)" />
  <source srcset="image2.jpg" media="(min-width: 750px)" />
  <img src="image3.jpg" />
</picture>
```

- [x] It displays image1.jpg at 1000px and higher, image2.jpg at 750-999px, and image3.jpg at 749px and lower.
- [ ] It displays image1.jps at 1000px and higher and image2.jpg at 750-999px, image3.jpg is a default in case `<picture>` is not supported.
- [ ] It displays image1.jpg at 1000px and higher and image2.jpg at 750px and higher, image3.jpg is a default in case `<picture>` is not supported.
- [ ] It displays image1.jpg, image2.jpg and image3.jpg at 1000px and higher.

[Source: HTML &lt;picture> Tag](https://www.w3schools.com/tags/tag_picture.asp)

#### Q25. What code will produce this table?

![Table with yellow background](images/ss-4.png?raw=true)

- [ ] A

```markdown
<table>
  <scope cols="2" style="background-color: yellow">
  <tr>
    <th>Col 1</th>
    <th>Col 2</th>
    <th>Col 3</th>
  </tr>
  <tr>
    <td>first</td>
    <td>second</td>
    <td>third</td>
  </tr>
</table>
```

- [x] B

```markdown
<table>
  <colgroup span="2" style="background-color: yellow">
  <tr>
    <th>Col 1</th>
    <th>Col 2</th>
    <th>Col 3</th>
  </tr>
  <tr>
    <td>first</td>
    <td>second</td>
    <td>third</td>
  </tr>
</table>
```

- [ ] C

```markdown
<table>
  <group cols="2" style="background-color: yellow">
  <tr scope="row">
    <th>Col 1</th>
    <th>Col 2</th>
    <th>Col 3</th>
  </tr>
  <tr scope="row">
    <td>first</td>
    <td>second</td>
    <td>third</td>
  </tr>
</table>
```

- [ ] D

```markdown
<table>
  <columns colspan="2" style="background-color: yellow">
  <tr>
    <th>Col 1</th>
    <th>Col 2</th>
    <th>Col 3</th>
  </tr>
  <tr>
    <td>first</td>
    <td>second</td>
    <td>third</td>
  </tr>
</table>
```

#### Q26. What is the `<hr>`tag typically used for?

- [ ] This tag is depreciated and should not be used.
- [x] It designates a topic shift within a section at the paragraph level.
- [ ] It draws a horizontal line.
- [ ] It designates a shift of topic at the section level.

This is a confusing question and there can be an arguments for both the second and the third options being correct.

[MDN](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/hr): The HTML `<hr>` element represents a thematic break between paragraph-level elements. Historically, this has been presented as a horizontal rule or line. While it may still be displayed as a horizontal rule in visual browsers, this element is now defined in semantic terms, rather than presentational terms, so if you wish to draw a horizontal line, you should do so using appropriate CSS.

#### Q27. What should fill the two blanks in the HTML code below?

```markdown
<section itemscope itemtype="http://schema.org/Restaurant">
  <h1 itemprop="name">Nadia's Garden</h1>
  <p itemscope ______ ______>
    <span itemprop="ratingValue">4.5</span> stars - based on
    <span itemprop="reviewCount">120</span> reviews
  </p>
</section>
```

- [ ] `itemprop="aggregateRating" itemref="http://schema.org/AggregateRating"`
- [x] `itemprop="aggregateRating" itemtype="http://schema.org/AggregateRating"`
- [ ] `itemid="aggregateRating" itemtype="http://schema.org/AggregateRating"`
- [ ] `itemid="aggregateRating" itemref="http://schema.org/AggregateRating"`

#### Q28. Which HTML snippet links back to the very top of a webpage?

- [x] A

```markdown
<a id="top"></a>

<!-- placed at the top of the page -->

<a href="#top">back to top</a>
```

- [ ] B

```markdown
<a name="top"></a>

<!-- placed at the top of the page -->

<a href="#top">back to top</a>
```

- [ ] C

```markdown
<a href="#">back to top</a> <a href="#top">back to top</a>
```

- [ ] D

```markdown
<button href="#">back to top</button> <button href="#top">back to top</button>
```

#### Q29. Which three tags where deprecated in HTML4 but returned to HTML5?

- [x] `<rb> <rp> <rt>`
- [ ] `<acronym> <code> <wbr>`
- [ ] `<hgroup> <q> <wbr>`
- [ ] `<b> <i> <u>`

#### Q30. The **\_** tag is used for marking up a short code snippet, while the \_ tag is used for marking up a longer block of code

- [ ] `<kdb>`, `<pre>`
- [ ] `<pre>`, `<code>`
- [ ] `<kdb>`, `<mark>`
- [x] `<code>`, `<pre>`

[Source: MDN Web Docs code](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/code)

[Source: MDN Web Docs pre](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/pre)

#### Q31. What does the `<label>` element do?

- [ ] It labels webpages with important information.
- [ ] It creates an ID for a corresponding input element.
- [ ] It overrides the name attribute's value on a child input element.
- [x] It programmatically associates a text label with an interface element.

#### Q32. To get a link to open in a new window or tab, use the **\_** attribute

- [x] `_blank`
- [ ] `_self`
- [ ] `_new`
- [ ] `_parent`

#### Q33. What is the most semantically accurate way to mark up the sentence shown below? Note: "TLAs" stands for "three-letter acronyms."

**We are fond of our TLAs in web design.**

- [ ] A

```html
<p>We are fond of our <span title="three-letter acronyms">TLAs</span> in web design.</p>
```

- [ ] B

```html
<p>We are fond of our TLAs in web design.</p>
```

- [x] C

```html
<p>we are fond of our <abbr title="three-letter acronyms">TLAs</abbr> in web design.</p>
```

- [ ] D

```html
<p>we are fond of our <acronym title="three-letter acronym">TLAs</acronym> in web design.</p>
```

`<acronym>` has been removed in HTML5 and shouldn't be used anymore. Instead web developers should use the `<abbr>` element.

#### Q34. What is the correctly nested markup for this list?

![Sample list](images/ss-6.png?raw=true)

- [ ] A

```markdown
<ul>
  <li>
    office
    <ol style="circle">
      <li>staple</li>
      <li>paper</li>
    </ol>
  </li>
  <li>
    groceries
    <ol style="circle">
      <li>milk</li>
    </ol>
  </li>
</ul>
```

- [x] B

```markdown
<ul>
  <li>Office Supplies
    <ul>
      <li>Stapler</li>
      <li>Paper clips</li>
    </ul>
  </li>
  <li>Groceries
    <ul>
      <li>Milk</li>
    </ul>
  </li>
</ul>
```

- [ ] C

```markdown
<ul>
  <li>office</li>
  <li>staple</li>
  <li>paper</li>
  <li>groceries</li>
  <li>milk</li>
</ul>
```

#### Q35. What should fill the blank below?

```html
<link href="phone.css" rel="stylesheet" _____="print" />
```

- [ ] title
- [ ] type
- [ ] device
- [x] media

#### Q36. What is the semantically correct way to mark up this layout?

![quote](images/ss-5.png?raw=true)

- [ ] A

```markdown
<p>
  "Making money is what you have to do to sustain a business—being driven to make something of value
  and purpose is much more powerful."
</p>
<p><em>Lynda Weinman</em></p>
```

- [ ] B

```markdown
<blockquote>
  <q
    >"Making money is what you have to do to sustain a business—being driven to make something of
    value and purpose is much more powerful."</q
  >
  <cite><em>Lynda Weinman</em></cite>
</blockquote>
```

- [x] C

```markdown
<blockquote>
  <p>
    "Making money is what you have to do to sustain a business—being driven to make something of
    value and purpose is much more powerful."
  </p>
  <cite>Lynda Weinman</cite>
</blockquote>
```

- [ ] D

```markdown
<section>
  <q
    >"Making money is what you have to do to sustain a business—being driven to make something of
    value and purpose is much more powerful."</q
  >
  <cite>Lynda Weinman</cite>
</section>
```

#### Q37. Which choice uses the correct terminology in describing this markup: `<p>info</p>`?

- [ ] The element opener is `<p>`, the element closer is `</p>`, and the element information is info.
- [ ] The start tag is `<p>`, the end tag is `</p>`, and the enclosed HTML is info.
- [x] The start tag is `<p>`, the end tag is `</p>`, and the element content is info.
- [ ] The start element is `<p>`, the end element is `</p>`, and the tag content is info.

#### Q38. What is the difference between `<input type="submit" value="click me">` and `<button type="submit">Click me</button>`?

- [ ] There is no difference. Both will render a button that submits a form.
- [x] Both will submit a form. However, the `<button>` can have content other than text, like an image or nested HTML elements, while the `<input>` cannot.
- [ ] `<input type="button">` has been deprecated in HTML5. You should use the `<button>` tag instead.
- [ ] Both will submit a form. However, the `<input>` can have content other than text, like an image or nested HTML elements, while the `<button>` cannot.

#### Q39. What is the best semantic way to indicate that text refers to keyboard entry?

- [ ] `<p>Press the <tt>Enter</tt> key to proceed.</p>`
- [x] `<p>Press the <kbd>Enter</kbd> key to proceed.</p>`
- [ ] `<p>Press the <samp>Enter</samp> key to proceed.</p>`
- [ ] `<p>Press the Enter key to proceed.</p>`

#### Q40. What does this code do?

```markdown
<audio controls>
  <source src="sound.mp3" type="audio/mpeg" />
  <source src="sound.ogg" type="audio/ogg" />
  <source src="sound.wav" type="audio/wav" />
</audio>
```

- [x] The browser chooses the first supported format to play with the browser's default controls.
- [ ] The browser chooses the best audio format to play with JavaScript-provided controls.
- [ ] The browser plays each sound file in order automatically. The user has controls to stop playback.
- [ ] The browser chooses the first supported sound file and will loop the sound until the user stops it.

#### Q41. What attribute applies a keyboard shortcut hint to the current element?

- [x] `accesskey`
- [ ] `shortcut`
- [ ] `keyboard`
- [ ] `access`

#### Q42. What is the correct way to code a link that, when clicked, will send an email to `email@example.com` with a subject of "Hello"?

- [ ] `<a href="mailto:email@example.com&subject=Hello">Click me</a>`
- [ ] `<a href="mailto:email@example.com">Hello</a>`
- [x] `<a href="mailto:email@example.com?subject=Hello">Click me</a>`
- [ ] `<a href="mailto:email@example.com?&subject=Hello">Click me</a>`

#### Q43. Which tag is the root element of an HTML document?

- [ ] `<DOCTYPE html>`
- [x] `<html>`
- [ ] `<body>`
- [ ] `<root>`

#### Q44. Which code snippet creates the layout shown, starting at `<table>` and ending at `</table>`?

![Table](images/ss-1.png?raw=true 'table')

- [ ] A

```markdown
<tr>
  <td>Table cell 1</td>
  <td>Table cell 2</td>
</tr>
<tr>
  <td rowspan="2">Table cell 3</td>
</tr>
```

- [ ] B

```markdown
<tr>
  <td>Table cell 1</td>
  <td>Table cell 2</td>
  <td>Table cell 3</td>
</tr>
```

- [x] C

```markdown
<tr>
  <td>Table cell 1</td>
  <td>Table cell 2</td>
</tr>
<tr>
  <td colspan="2">Table cell 3</td>
</tr>
```

- [ ] D

```markdown
<tr>
  <td>Table cell 1</td>
  <td>Table cell 2</td>
</tr>
<tr>
  <td>Table cell 3</td>
</tr>
```

#### Q45. Which choice is NOT a legal value for the **name** attribute within a `<meta>` tag?

- [x] charset
- [ ] viewport
- [ ] generator
- [ ] author

#### Q46. Which form is coded correctly?

- [ ] A

```markdown
<form>
  <legend>Title</legend>
  <fieldset>
    <label for="name">Your name:</label>
    <input type="text" name="name" id="name" />
    <button type="submit">Submit</button>
  </fieldset>
</form>
```

- [ ] B

```markdown
<form>
  <fieldset>
    <legend>Title</legend>
    <p>Your name:</p>
    <input type="text" name="name" id="name" />
    <input type="submit" value="Submit" />
  </fieldset>
</form>
```

- [x] C

```markdown
<form>
  <fieldset>
    <legend>Title</legend>
    <label for="name">Your name:</label>
    <input type="text" name="name" id="name" />
    <button type="submit">Submit</button>
  </fieldset>
</form>
```

- [ ] D

```markdown
<form>
  <legend>Title</legend>
  <label for="name">Your name:</label>
  <input type="text" name="name" id="name" />
  <input type="submit" value="Submit" />
</form>
```

#### Q47. What does the **poster** attribute do in the `<video>` tag?

- [x] It specifies an image that should display while the video downloads and until the video is played.
- [ ] It specifies an image that only displays if there is a problem with the video.
- [ ] It specifies an image that should display until the video is played.
- [ ] It specifies an image that should display while the video downloads.

#### Q48. What does this code do?

```html
<audio controls src="sound.mp3" type="audio/mpeg">When does this text display?</audio>
```

- [ ] The text displays over the audio controls, unless CSS is used to position it elsewhere.
- [ ] The text displays under the audio controls.
- [x] The text displays when the browser cannot play the sound.
- [ ] The text never displays.

#### Q49. What is the primary purpose of the `<canvas>` tag?

- [ ] It allows raster images to be rendered on the webpage.
- [ ] It displays annotated images.
- [x] It allows drawing on a bitmap via JavaScript.
- [ ] It allows vector images to be rendered on the webpage.

#### Q50. Which choice contains three valid block-level elements?</li>

- [ ] `<details> <abbr> <figcaption>`
- [ ] `<canvas> <select> <noscript>`
- [x] `<dt> <table> <pre>`
- [ ] `<kbd> <p> <main>`

#### Q51. In the code below, what is the purpose of the **lang** attribute?

```html
<p lang="en-GB">Welcome to our wonderful website.</p>
```

- [ ] It establishes the language for the website—in this case, English.
- [ ] It establishes the language and dialect for the website—in this case, British English.
- [x] It establishes the language and dialect for the paragraph—in this case, British English.
- [ ] It establishes the language for the paragraph—in this case, English.

#### Q52. Which image formats can be displayed by all web browsers?

- [ ] JPG, GIF, TIF
- [ ] JPG, TIF, BMP
- [ ] TIF, BMP, GIF
- [x] PNG, GIF, JPG

#### Q53. Review the code below. What is the absolute URL for a page called **page.html**?

```html
<base href="http://www.linkedin.com/dir/" />
```

- [x] `http://www.linkedin.com/dir/page.html`
- [ ] `page.html`
- [ ] `http://www.linkedin.com/page.html`
- [ ] `dir/page.html`

#### Q54. What is the correct way to include a stylesheet named **style.css** in the `<head>` of your document?

- [ ] `<style link="style.css">`
- [x] `<link rel="stylesheet" href="style.css">`
- [ ] `<style src="style.css"></style>`
- [ ] `<link style="style.css">`

#### Q55. You want to have single spacing in between some lines, like in a poem or an address. Which approach should you use?

- [ ] Wrap the text in a box that is the right width so everything wraps correctly. Set the box width with CSS.
- [x] Separate lines with a `<p>`, then use CSS to make single spacing.
- [ ] Use the `<pre>` tag to make the line spacing look exactly like you want.
- [ ] Separate the lines with the `<br>` tag.

#### Q56. What does the `<wbr>` tag do?

- [ ] It requires the browser to wrap the current line at that point.
- [ ] It breaks a word into two pieces, using a hyphen to connect the words.
- [ ] It formats a sentence to be easily breakable.
- [x] It presents an opportunity for a break in a very long word, if needed for proper page display.

#### Q57. Review the code below. How do you include subnavigation for Link 2 that includes a link?

```markdown
<nav><ul>
  <li><a href="#">Link 1</a></li>
  <li><a href="#">Link 2</a></li>
  <li><a href="#">Link 3</a></li>
</ul></nav>
```

- [ ] A

```markdown
<nav><ul>
  <li><a href="#">Link 1</a></li>
  <li><a href="#">Link 2</a></li>
    <ul>
      <li><a href="#">Link 2a</a></li>
    </ul>
  <li><a href="#">Link 3</a></li>
</ul></nav>
```

- [x] B

```markdown
<nav><ul>
  <li><a href="#">Link 1</a></li>
  <li><a href="#">Link 2</a>
    <ul>
      <li><a href="#">Link 2a</a></li>
    </ul>
  </li>
  <li><a href="#">Link 3</a></li>
</ul></nav>
```

- [ ] C

```markdown
<ul><nav>
  <li><a href="#">Link 1</a></li>
  <li><a href="#">Link 2</a>
    <ul><nav>
      <li><a href="#">Link 2a</a></li>
    </nav></ul>
  </li>
  <li><a href="#">Link 3</a></li>
</nav></ul>
```

- [ ] D

```markdown
<nav><ul>
  <li><a href="#">Link 1</a></li>
  <li><a href="#">Link 2</a></li>
  <nav><ul>
    <li><a href="#">Link 2a</a></li>
  </ul></nav>
  <li><a href="#">Link 3</a></li>
</ul></nav>
```

#### Q58. What is the correct way to code a comment in HTML?

- [ ] `//this is a comment`
- [ ] `/* this is a comment */`
- [ ] `<! this is a comment ->`
- [x] `<!-- this is a comment -->`

#### Q59. Which statement is **false**?

- [ ] Inline elements can be nested inside inline elements.
- [ ] Block elements can be nested inside block elements.
- [ ] Inline elements can be nested inside block elements.
- [x] Block elements can be nested inside inline elements.

#### Q60. What is the best semantic to use Quotes in HTML?

`Steve Kruz Said: "He will Win"`

- [x] `<q>`
- [ ] `<quote>`
- [ ] `<blockquote>`
- [ ] `<notation>`

[Reference (w3schools)](https://www.w3schools.com/html/html_quotation_elements.asp)

#### Q61. What is the semantic meaning of the `<hr>` tag?

- [ ] It draws a horizontal line.
- [ ] This tag is deprecated and should not be used.
- [ ] It designates a separation of sections within an `<article>`.
- [x] It designates a topic shift within a section at the paragraph level.

#### Q62. How will a video look displayed on a fully loaded webpage if the `<video>` tag is used and the **autoplay** attribute is not set?

- [ ] It will display a random frame from a video, unless the **poster** attribute is set.
- [x] It will display the first frame of the video, unless the **poster** attribute is set.
- [ ] It will display nothing unless the **poster** attribute is set.
- [ ] It will display a black window unless the **poster** attribute is set.

[Reference (w3schools)](https://www.w3schools.com/tags/tryit.asp?filename=tryhtml5_video)

#### Q63. What is the correct way to describe an empty element?

- [ ] It has opening and closing tags but no child content.
- [ ] It display nothing on a website.
- [x] It has no child content and no closing tag.
- [ ] It has child content but no closing tag.

[Reference (MDN Web Docs)](https://developer.mozilla.org/en-US/docs/Glossary/Empty_element)

#### Q64. What is the purpose of async in this code?

`<script async src="myscript.js"></script>`

- [ ] It downloads the script from the server when resources allow.
- [ ] It runs the script after HTML parsing is complete.
- [x] It runs the script when the script is ready.
- [ ] It pauses the parsing of HTML code while the script runs.

#### Q65. What does this code do on a page you are visiting for the first time?

`<audio autoplay loop src="sound.mp3" type="audio/mpeg"></audio>`

- [ ] When the **Play** button is pressed, the browser plays the sound over and over again until the user stops it.
- [ ] The browser plays the sound once automatically in the background. The user has no control over the sound.
- [ ] The browser plays the sound automatically and continuously in the background. The user may stop the sound at any tune.
- [x] It does nothing. Modern browsers require some form of interaction before they let a page autoplay with audio.

References [(MDN) audio](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/audio),
[(MDN) autoplay](https://developer.mozilla.org/en-US/docs/Web/Media/Autoplay_guide)

#### Q66. What is the difference between the `<head>` and `<header>` tags?

- [ ] There is only one `<head>` tag per page, while there may be many `<header>` tags.
- [ ] The `<head>` tag may contain CSS and Javascript links, while the `<header>` tag may contain headings and navigational links.
- [x] all of these answers
- [ ] The `<head>` tag contains meta information, while the `<header>` tag contains navigation, logos, and other page identifying content.

#### Q67. In this code, what is the purpose of defer?

`<script defer src="myscript.js"></script>`

- [ ] It downloads the script from the server when resources allow.
- [x] It runs the script after HTML parsing is complete.
- [ ] It runs the script when the script is ready.
- [ ] It pauses the parsing of HTML code while the script runs.

#### Q68. The code below contains some errors. Which choice corrects all of the errors?

```html
<table>
  <tr>
    Cell 1
  </tr>
  <td>Cell 2</td>
  <caption>
    A table
  </caption>
</table>
```

- [ ] A

```HTML
<caption>A table</caption>
  <table>
    <td>
      <tr>Cell 1</tr>
      <tr>Cell 2</tr>
    </td>
  </table>
```

- [ ] B

```HTML
<caption>A table</caption>
<table>
  <tr>
    <td>Cell 1</td>
    <td>Cell 2</td>
  </tr>
</table>
```

- [x] C

```HTML
<table>
  <caption>A table</caption>
  <tr>
    <td>Cell 1</td>
    <td>Cell 2</td>
  </tr>
</table>
```

- [ ] D

```HTML
<table>
  <tr>
    <td>Cell 1</td>
    <td>Cell 2</td>
  </tr>
  <caption>A table</caption>
</table>
```

#### Q69. Given the file and directory structure shown here, what is the correct element to place in file profit.html to link to info.html?

![Image of footer](images/ss-7.png?raw=true)

- [ ] `<a href="../work/info.html">See Information </a>`
- [x] `<a href="../info.html">See Information </a>`
- [ ] `<a href="../../info.html">See Information </a>`
- [ ] `<a href="info.html">See Information </a>`

#### Q70. When should you use the `<article>` element?

- [ ] For blog posts and other social media items
- [ ] For the main content area of your website
- [x] When the content stands alone as a unit, is suitable for syndication, or is reusable
- [ ] To associate comments with a blog post

[Reference (MDN)](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/article)

#### Q71. Which list comprises three empty elements?

- [ ] A

```HTML
<area>
<embed>
<strong>
```

- [ ] B

```HTML
<input>
<br>
<p>
```

- [ ] C

```HTML
<link>
<meta>
<title>
```

- [x] D

```HTML
<wbr>
<base>
<source>
```

#### Q72. Which snippet of HTML, when clicked, makes a phone call on a mobile device?

- [x] `<a href="tel:802-555-1212">Call me</a>`
- [ ] `<a href="phone">802-555-1212</a>`
- [ ] `<a href="tel">802-555-1212</a>`
- [ ] `<a href="phone:802-555-1212">Call me</a>`

#### Q73. What is the purpose of the `class` attribute?

- [ ] Classes allow CSS to select specific elements on the page. You may list as many class names within the class attribute as you wish,
      separated by spaces.
- [ ] Classes allow CSS and JavaScript to select specific elements on the page. You may list only one class name per class attribute.
- [ ] Classes allow CSS to select specific elements on the page. You may list only one class name per class attribute.
- [x] Classes allow CSS and JavaScript to select specific elements on the page. You may list as many class names within the class attribute
      as you wish, separated by spaces.

[Reference (MDN)](https://developer.mozilla.org/en-US/docs/Web/HTML/Global_attributes/class)

#### Q74. Which choice is not a legal type attribute for the `<input>` tag?

- [ ] `<input type="color">`
- [ ] `<input type="tel">`
- [ ] `<input type="week">`
- [x] `<input type="num">`

[Reference (MDN)](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/Input)

#### Q75. What is the most semantic way to mark up this sentence so that "happy talk must die" is rendered as an inline quote?

As Steve Krug once said, happy talk must die.

- [ ] `<p>`As Steve Krug once said, `<b>`happy talk must die.`</b>` `</p>`
- [ ] `<p>`As Steve Krug once said, `<i>`happy talk must die.`</i>` `</p>`
- [ ] `<p>`As Steve Krug once said, `<blockquote>`happy talk must die.`</blockquote>` `</p>`
- [x] `<p>`As Steve Krug once said, `<q>`happy talk must die.`</q>` `</p>`

[Source: W3Schools](https://www.w3schools.com/tags/tag_q.asp)

**`<q>` tag**
`Most browsers will display q tags as inline elements with quotes`

#### Q76. What is the most semantically accurate way to make up a main navigation bar, displayed in a horizontal direction?

- [ ] A

```markdown
<p>
  <a href="index.html">Home</a>
  <a href="about.html">About</a>
  <a href="contact.html">Contact</a>
</p>
```

- [ ] B

```markdown
<nav>
  <a href="index.html">Home</a>
  <a href="about.html">About</a>
  <a href="contact.html">Contact</a>
</nav>
```

- [ ] C

```markdown
 <nav>
    <ol>
      <li><a href="index.html">Home</a></li>
      <li><a href="about.html">About</a></li>
      <li><a href="contact.html">Contact</a></li>
     </ol>
  </nav>
```

- [x] D

```markdown
 <nav>
   <ul>
     <li><a href="index.html">Home</a></li>
     <li><a href="about.html">About</a></li>
     <li><a href="contact.html">Contact</a></li>
    </ul>
  </nav>
```

#### Q77. Which choice is the best way to mark up this layout?

![Image of footer](images/ss-8.png?raw=true)

- [x] A

```markdown
<h4>Mailing Address</h4>
<address>
  6410 Via Real <br>
  Carpinteria, CA 93013<br>
  <a href="mailto:info@linkedin.com">info@linkedin.com</a>
</address>
```

- [ ] B

```markdown
<h4><strong>Mailing Address</h4>
<address><em>
  6410 Via Real <br>
  Carpinteria, CA 93013<br>
  <a href="mailto:info@linkedin.com">info@linkedin.com</a>
</em></address>
```

- [ ] C

```markdown
<h4>Mailing Address</h4>
<p><em>
  6410 Via Real <br>
  Carpinteria, CA 93013<br>
  <a href="mailto:info@linkedin.com">info@linkedin.com</a>
</em></p>
```

- [ ] D

```markdown
<p><strong>Mailing Address</strong></p>
<p><em>
  6410 Via Real <br>
  Carpinteria, CA 93013<br>
  <a href="mailto:info@linkedin.com">info@linkedin.com</a>
</em></p>
```

[Source: W3Schools](https://www.w3schools.com/tags/tag_address.asp)

`The <address> tag defines the contact information for the author/owner of a document or an article. The contact information can be an email address, URL, physical address, phone number, social media handle, etc. The text in the <address> element usually renders in italic, and browsers will always add a line break before and after the <address> element.`

#### Q78. What is the primary purpose of HTML?

- [x] HTML structures the webpage, identifying its elements such as paragraphs, headings, and lists.
- [ ] HTML structures and provides a rudimentary look to webpages.
- [ ] HTML is responsible for the structure, styling, and interactivity of webpages.
- [ ] HTML is responsible for the structure and styling of webpages.

#### Q79. What is the correct way to describe an empty element, such as a line break tag?

- [ ] It displays nothing on a website.
- [ ] It has opening and closing tags but no child content.
- [ ] It has child content but no closing tag.
- [x] It has no child content and no closing tag.

#### Q80. For the HTML code below, when will "Sample Text" display to the browser?

```markdown
<noscript>Sample Text</noscript>
```

- [ ] when there is no JavaScript used on this webpage
- [x] when JavaScript is not supported by the browser or if JavaScript is disabled in the browser
- [ ] when JavaScript is disabled in the web browser
- [ ] when JavaScript is not supported by the web browser

[Reference (MDN)](https://www.w3schools.com/tags/tag_noscript.asp)

#### Q81. How will this code render by default in most web browsers?

```markdown
<details>
  <h4>Mixed Berry Tart.</h4>
  <p>Raspberries, blueberries, and strawberries on top of a creamy filling served in a crispy tart.</p>
</details>
```

- [ ] A
      ![A](images/Q84-1.jpg)
- [x] B
      ![B](images/Q84-2.jpg)
- [ ] C
      ![C](images/Q84-3.jpg)
- [ ] D
      ![D](images/Q84-4.jpg)

#### Q82. In this code, what is _target_?

- [x] an attribute
- [ ] a tag
- [ ] content
- [ ] an element

#### Q83. What is the difference between the `<svg>` and `<canvas>`?

- [x] `<svg>` produces vector graphics, while `<canvas>` produces raster graphics.
- [ ] `<svg>` integrates with JavaScript, while `<canvas>` does not.
- [ ] `<svg>` produces raster graphics, while `<canvas>` produces vector graphics.
- [ ] `<svg>` cannot be used as a background image, while `<canvas>` can be used as a background

#### Q84. What is the difference between the _readonly_ and _disabled_ attributes for the `<textarea>` element?

- [x] _readonly_ allows clicking in the `<textarea>` element. _disabled_ prevents all interaction with the control.
- [ ] _readonly_ is invalid attribute for `<textarea>`, while _disabled_ is a valid attribute.
- [ ] _disabled_ allows clicking in the `<textarea>` element. _readonly_ prevents all interaction with the control.
- [ ] _disabled_ is invalid attribute for `<textarea>`, while _readonly_ is a valid attribute.

[Source: readonly](https://www.w3schools.com/tags/att_readonly.asp)

[Source: disabled](https://www.w3schools.com/tags/att_disabled.asp)

#### Q85. In this code, what is _target_?

`<a target="_blank">...</a>`

- [x] an attribute
- [ ] a tag
- [ ] content
- [ ] an element

#### Q86. What is the correct way to add a submit URL to a `button` element?

- [ ] A

```HTML
<button submit="http://example.com/process">
  Process data
</button>
```

- [ ] B

```HTML
<button action="http://example.com/process">
  Process data
</button>
```

- [x] C

```HTML
<button formaction="http://example.com/process">
  Process data
</button>
```

- [ ] D

```HTML
<button method="http://example.com/process">
  Process data
</button>
```

`formaction — The URL that processes the information submitted by the button. Overrides the action attribute of the button's form owner. Does nothing if there is no form owner.` [Source](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/button#attr-formaction)

#### Q87. Which is the best markup to produce this text?

`x<y&z>w`

- [ ] `<p>x<y&z>w</p>`
- [x] `<p>x\<y&z\>w</p>`
- [ ] `<p>x<<y&&z>>w`
- [ ] `<p>x<y&z>w</p>`

`This question has an issue, however this answer will count as correct`

`It's too strange question because all of that methods doesn't work. The good method is &amp, &lt, &gt using.`

#### Q88. What is wrong with this code snippet?

```HTML
<label>Address:</label>
<input type="text" name="address" id="address-input" />
```

- [ ] The `<label>` and `<input>` should be nested inside of a `<fieldset>` element.
- [ ] **"address"** is not a valid value for the attribute **name** on an `<input>` element.
- [ ] The `<label>` element is missing an **id** set to "address-input".
- [x] The `<label>` element is missing a **for** attribute set to "address-input".

#### Q89. What is the default method for form submission?

- [x] GET
- [ ] POST
- [ ] PUT
- [ ] SUBMIT

#### Q90. Which is the most semantically correct markup for a side comment in small print?

- [x] `<p>` Get 10% discount `<small>`not valid in France`</small></p>`
- [ ] `<p>` Get 10% discount `<!--not valid in France--> </p>`
- [ ] `<p>` Get 10% discount `<comment>`not valid in France`</comment></p>`
- [ ] `<p>` Get 10% discount `<aside>`not valid in France`</aside></p>`

#### Q91. Which choice will produce the spanish word <i>canción</i>?

- [ ] `<p lang="es">canción</p>`
- [x] `<p lang="es">canci&oacuten</p>`
- [ ] `<p lang="es">cancio'n</p>`
- [ ] `<p lang="es">canci'on</p>`

#### Q92. What is the purpose of `<caption>`?

- [ ] `<caption>` provides captions for `<audio>`,`<video>`,`<img>`, and `<table>`.
- [x] `<caption>` provides captions to `<table>`.
- [ ] `<caption>` provides captions for `<audio>`, `<video>`, and `<table>`.
- [ ] `<caption>` provides captions for `<img>`, `<audio>`, and `<video>`.

#### Q93. The value attribute is associated with which set of tags ?

- [x] A

```HTML
<li>
<input>
<option>
```

- [ ] B

```HTML
<input>
<option>
<textarea>
```

- [ ] C

```HTML
<button>
<input>
<form>
```

- [ ] D

```HTML
<input>
<label>
<meter>
```

#### Q94. What is wrong with this code?

`<img src="https://source.unsplash.com/random">`

- [ ] `<img>` should be paired with a `<caption>` tag.
- [x] The `<img>` element is missing an alt attribute.
- [ ] `<img>` is not a valid HTML element. Instead, use `<image src="..."/>`.
- [ ] `<img>` should be nested within a `<figure>` tag.

#### Q95. Which choice is the most semantically correct markup for specifying the first definition of a term?

- [ ] `<p>`The `<dl>`focal length`</dl>` of a lens gives the distance from the lens to the image sensor.`</p>`
- [x] `<p>`The `<dfn>`focal length`<dfn>` of a lens gives the distance from the lens to the image sensor.`</p>`
- [ ] `<p>`The `<dt>`focal length`</dt>` of a lens gives the distance from the lens to the image sensor.`</p>`
- [ ] `<p>`The `<dd>`focal length`</dd>` of a lens gives the distance from the lens to the image sensor.`</p>`

`**Definition element => The <dfn> HTML element is used to indicate the term being defined within the context of a definition phrase or sentence. `<br>`**Description Term element => The <dt> HTML element specifies a term in a description or definition list, and as such must be used inside a <dl> element.`<br>` **Description Details element =>The <dd> HTML element provides the description, definition, or value for the preceding term (<dt>) in a description list (<dl>).`

[Source](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/dfn)

#### Q96. Which choice is the best way to code three choices within a form so that the user can select multiple items?

- [ ] <input type="radio" name="example"> Choice 1 <br/>
      <input type="radio" name="example"> Choice 2 <br/>
      <input type="radio" name="example"> Choice 3

- [x] <input type="checkbox" name="example"> Choice 1 <br/>
      <input type="checkbox" name="example"> Choice 2 <br/>
      <input type="checkbox" name="example"> Choice 3

- [ ] <label><input type="checkbox" name="example"> Choice 1</label><br/>
      <label><input type="checkbox" name="example"> Choice 2</label><br/>
      <label><input type="checkbox" name="example"> Choice 3</label>

- [ ] <label><input type="radio" name="example"> Choice 1</label><br/>
      <label><input type="radio" name="example"> Choice 2</label><br/>
      <label><input type="radio" name="example"> Choice 3</label>

`<input> elements of type checkbox are rendered by default as boxes that are checked (ticked) when activated, like you might see in an official government paper form. The exact appearance depends upon the operating system configuration under which the browser is running. Generally this is a square but it may have rounded corners.`

[Source](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/input/checkbox)

#### Q97. How would you mark up a piece of ASCII art (an emoticon) in an accessible way?

- [x] `<pre role="emoticon" aria-label="ASCII emoticon of a shrug">¯\_(ツ)_/¯</pre>`
- [ ] `<pre role="img" aria-label="ASCII emoticon of a shrug">¯\_(ツ)_/¯</pre>`
- [ ] `<dfn title="ASCII emoticon of a shrug">¯\_(ツ)_/¯</dfn>`
- [ ] `<label for="art">ASCII emoticon of a shrug</label><pre role="img" id="art">¯\_(ツ)_/¯</pre>`

#### Q98. Which example is a standard way in HTML5 for adding author metadata to a page?

- [ ] `<metadata name="author" content="Author Name">`
- [ ] `<meta name="author">Author Name</meta>`
- [ ] `<meta name="creator" content="Author Name">`
- [x] `<meta name="author" content="Author Name">`

#### Q99. Given the following requirements, select the correct `input` configuration: An `input` that allows the user to select from a range of integer values between 0 and 100 (inclusive) in increments of 5.

- [ ] `<input type="range" min="0" max="100" by="5" />`
- [x] `<input type="range" min="0" max="100" step="5" />`
- [ ] `<input type="number" min="0" max="100" step="5" />`
- [ ] `<input type="number" min="0" max="100" by="5" />`

`<input> elements of type range let the user specify a numeric value which must be no less than a given value, and no more than another given value. The step attribute is a number that specifies the granularity that the value must adhere to.`

[Source](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/Input/range)

#### Q100. Which choice is valid markup for a `<head>` element?

- [ ] `<head class="Page Section Information" id="head"><title>Page Title</title></head>`
- [ ] `<head><title>Page Title</title> <img src="favicon.icon" alt=""></head>`
- [x] `<head><title>Page Title</title> <data value="email">email@example.com</data></head>`
- [ ] `<head><title>Page Title</title><address>email@example.com</address></head>`

`The <head> HTML element contains machine-readable information (metadata) about the document, like its title.The <data> tag is used to add a machine-readable translation of a given content.`
[Source 1](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/head)/
[Source 2](https://www.w3schools.com/tags/tag_data.asp)

#### Q101. You need to add comments to the company blog. What is the most semantic markup for a list of comments?

- [x] A

```HTML
<aside>
  <h3>Comments</h3>
  <article> First comment.</article>
  <article> Second comment.</article>
</aside>
```

- [ ] B

```HTML
<div aria="dpub-comments">
  <h3>Comments</h3>
  <div aria="dpub-comment"> First comment.</div>
  <div aria="dpub-comment"> Second comment.</div>
</div>
```

- [ ] C

```HTML
<aside>
  <h3>Comments</h3>
  <aside> First comment.</aside>
  <aside> Second comment.</aside>
</aside>
```

- [ ] D

```HTML
<div typeof="comments">
  <h3>Comments</h3>
  <div typeof="comment"> First comment.</div>
  <div typeof="comment"> Second comment.</div>
</div>
```

`The <article> HTML element represents a self-contained composition in a document, page, application, or site, which is intended to be independently distributable or reusable (e.g., in syndication). Example:a user-submitted comment.`
[Source](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/article)

#### Q102. To make something editable by the user, you need to set the **\_** attribute to **\_**.

- [ ] `access`; allow
- [ ] `designMode`; true
- [x] `contenteditable`; true
- [ ] `contenteditable`; yes

`The contenteditable global attribute is an enumerated attribute indicating if the element should be editable by the user. If so, the browser modifies its widget to allow editing. The attribute must take one of the following values: true or an empty string, which indicates that the element is editable; false, which indicates that the element is not editable.`
[Source](https://developer.mozilla.org/en-US/docs/Web/HTML/Global_attributes/contenteditable)

#### Q103. Which choice is the standard way to include a value in a form without making it visible to or editable by the user?

- [ ] `<input type="invisible" name="important" value="information">`
- [ ] `<input type="text" style="display: none;" name="important" value="information">`
- [x] `<input type="hidden" name="important" value="information">`
- [ ] `<input type="text" hidden name="important" value="information">`

`<input> elements of type hidden let web developers include data that cannot be seen or modified by users when a form is submitted. For example, the ID of the content that is currently being ordered or edited, or a unique security token. Hidden inputs are completely invisible in the rendered page, and there is no way to make it visible in the page's content.` [Source](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/input/hidden)

#### Q104. What is the semantic way to add an identifying title to a table?

- [ ] `<table><label>Heading</label>...</table>`
- [ ] `<table><title>Heading</title>...</table>`
- [ ] `<table><legend>Heading</legend>...</table>`
- [x] `<table><caption>Heading</caption>...</table>`

`The <caption> HTML element specifies the caption (or title) of a table.` [Source](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/caption)

#### Q105. Which image file referenced in this `img` element's `srcset` attribute should a browser on a small mobile phone load?

```html
<img
  srcset="medium.jpg 320w, large.jpg 1280w"
  src="small.jpg"
  alt="Our favorite image"
  sizes="(min-width: 1200px) 640px, 100vw"
/>
```

- [ ] small.jpg
- [ ] medium.jpg
- [ ] none of them
- [x] large.jpg

`The browser will: 1. Look at its device width. 2. Work out which media condition in the sizes list is the first one to be true. 3. Look at the slot size given to that media query. 4. Load the image referenced in the srcset list that has the same size as the slot or, if there isn't one, the first image that is bigger than the chosen slot size.` [Source](https://developer.mozilla.org/en-US/docs/Learn/HTML/Multimedia_and_embedding/Responsive_images)

#### Q106. Which description is coded correctly?

- [x] A

```HTML
<dl>
  <dt>Server</dt>
  <dd>Software used to serve webpages, like Apache.</dd>
  <dd> Hardware used to provide data to other computers.</dd>
  <!-- Other terms and descriptions -->
</dl>
```

- [ ] B

```HTML
<dt>
  <dl>Server</dl>
  <dd>Software used to serve webpages, like Apache.</dd>
  <dd> Hardware used to provide data to other computers.</dd>
  <!-- Other terms and descriptions -->
</dt>
```

- [ ] C

```HTML
<dl>
  <dt>Server</dt>
  <dd>Software used to serve webpages, like Apache.</dd>
  <dt> Hardware used to provide data to other computers.</dt>
  <!-- Other terms and descriptions -->
</dl>
```

- [ ] D

```HTML
<dl>
  <dd>Server</dd>
  <dt>Software used to serve webpages, like Apache.</dt>
  <dt> Hardware used to provide data to other computers.</dt>
  <!-- Other terms and descriptions -->
</dl>
```

[Source 1](https://html.spec.whatwg.org/multipage/grouping-content.html#the-dl-element)
[Source 2](https://www.w3schools.com/tags/tag_dl.asp)

#### Q107. What is wrong with this code?

```HTML
<ul>
  <h2>Espresso Drinks</h2>
  <li>Espresso</li>
  <li>Latte</li>
  <li>Cappuccino</li>
  <li>Mocha</li>
</ul>
```

- [ ] Nothing is wrong.
- [x] `<ul>` cannot contain a heading element as a direct child.
- [ ] An `<h1>` should be used here instead of an `<h2>` tag.
- [ ] Only `<ol>` allows direct descendants to contain elements other than an `<li>`, so use an `<ol>` here instead.

`ul content model only accepts "Zero or more li and script-supporting elements".` [Source](https://html.spec.whatwg.org/multipage/grouping-content.html#the-ul-element)

#### Q108. A designer gave you CSS code that should run only when the device rendering the page is in dark mode. How would you embed that code?

- [ ] `<style media="light-mode: false">/* CSS code */</style>`
- [ ] `<style media="color-mode: dark">/* CSS code */</style>`
- [x] `<style media="prefers-color-scheme: dark">/* CSS code */</style>`
- [ ] `<style media="color-scheme: dark">/* CSS code */</style>`

#### Q109. How would you mark up a header for a table row?

- [x] A

```HTML
<table>
  <thead scope="row"><th row="1">Header</th></thead>
  <tr>
    <td>10</td>
    <td>18</td>
  </tr>
</table>
```

- [ ] B

```HTML
<table>
  <tr>
  <th scope="row">Header</th>
    <td>10</td>
    <td>18</td>
  </tr>
</table>
```

- [ ] C

```HTML
<table>
  <tr>
    <thead scope="row">Header</thead>
    <td>10</td>
    <td>18</td>
  </tr>
</table>
```

- [ ] D

```HTML
<table>
  <tr>
    <th>Header</th>
    <td>10</td>
    <td>18</td>
  </tr>
</table>
```

#### Q110. What is the best semantic markup for this sentence? On July 21, 1969, Neil Armstrong said, "That's one small step for man, one giant leap for mankind.

- [x] A

```HTML
  <p>On <time datetime="1969-07-21">July 21, 1969</time>, Neil Armstrong said, <q cite="https://www.hq.nasa.gov/alsj/a11/a11.step.html">That's one small step for man, one giant leap for mankind.</q></p>
```

- [ ] B

```HTML
<p>On <time datetime="07-21-1969">July 21, 1969</time>, Neil Armstrong said, <q cite="https://www.hq.nasa.gov/alsj/a11/a11.step.html">That's one small step for man, one giant leap for mankind.</q></p>
```

- [ ] C

```HTML
<p>On July 21, 1969, Neil Armstrong said, <q cite="https://www.hq.nasa.gov/alsj/a11/a11.step.html">"That's one small step for man, one giant leap for mankind."</q></p>
```

- [ ] D

```HTML
<p>On July 21, 1969, Neil Armstrong said, <q>"That's one small step for man, one giant leap for mankind."</q></p>
```

#### Q111. What is the root element of an HTML document.

- [x] `<html>`
- [ ] `<body>`
- [ ] `<root>`
- [ ] `<!DOCTYPE html>`

`
The <html> tag is the root element of an HTML document, which means that it contains all the contents and tags of the HTML document within it.

The html element represents the root of a document.
`
[Source](https://www.interviewbit.com/html-mcq/)
[Source](https://www.w3.org/TR/2010/WD-html-markup-20100624/html.html)
## CSS

#### Q1. In the following example, which selector has the highest specificity ranking for selecting the anchor link element?

```css
ul li a
a
.example a
div a
```

- [x] `.example a`
- [ ] `div a`
- [ ] `a`
- [ ] `ul li a`

#### Q2. Using an attribute selector, how would you select an `<a>` element with a "title" attribute?

- [x] `a[title]{...}`
- [ ] `a > title {...}`
- [ ] `a.title {...}`
- [ ] `a=title {...}`

#### Q3. CSS grid and flexbox are now becoming a more popular way to create page layouts. However, floats are still commonly used, especially when working with an older code base, or if you need to support older browser version. What are two valid techniques used to clear floats?

- [ ] Use the "clearfix hack" on the floated element and add a float to the parent element.
- [ ] Use the overflow property on the floated element or the "clearfix hack" on either the floated or parent element.
- [ ] Use the "clearfix hack" on the floated element or the overflow property on the parent element.
- [x] Use the "clearfix hack" on the parent element or use the overflow property with a value other than "visible."

#### Q4. What element(s) do the following selectors match to?

```css
1) .nav {
  ...;
}
2) nav {
  ...;
}
3) #nav {
  ...;
}
```

- [ ]
  ```markdown
  1. An element with an ID of "nav"
  2. A nav element
  3. An element with a class of "nav"
  ```
- [ ]
  ```markdown
      They all target the same nav element.
  ```
- [x]
  ```markdown
  1. An element with an class of "nav"
  2. A nav element
  3. An element with a id of "nav"
  ```
- [ ]
  ```markdown
  1. An element with an class of "nav"
  2. A nav element
  3. An div with a id of "nav"
  ```

#### Q5. When adding transparency styles, what is the difference between using the opacity property versus the background property with an `rgba()` value?

- [ ] Opacity specifies the level of transparency of the child elements. Background with an `rgba()` value applies transparency to the background color only.
- [ ] Opacity applies transparency to the background color only. Background with an `rgba()` value specifies the level of transparency of an element, as a whole, including its content.
- [x] Opacity specifies the level of transparency of an element, including its content. Background with an `rgba()` value applies transparency to the background color only.
- [ ] Opacity applies transparency to the parent and child elements. Background with an `rgba()` value specifies the level of transparency of the parent element only.

#### Q6. What is true of block and inline elements? (_Alternative_: Which statement about block and inline elements is true?)

- [ ] By default, block elements are the same height and width as the content container between their tags; inline elements span the entire width of its container.
- [x] By default, block elements span the entire width of its container; inline elements are the same height and width as the content contained between their tags.
- [ ] A `<nav>` element is an example of an inline element. `<header>` is an example of a block element.
- [ ] A `<span>` is an example of a block element. `<div>` is an example of an inline element.

#### Q7. CSS grid introduced a new length unit, fr, to create flexible grid tracks. Referring to the code sample below, what will the widths of the three columns be?

```css
.grid {
  display: grid;
  width: 500px;
  grid-template-columns: 50px 1fr 2fr;
}
```

- [ ] The first column will have a width of 50px. The second column will be 50px wide and the third column will be 100px wide.
- [x] The first column will have a width of 50px. The second column will be 150px wide and the third column will be 300px wide.
- [ ] The first column will have a width of 50px. The second column will be 300px wide and the third column will be 150px wide.
- [ ] The first column will have a width of 50px. The second column will be 500px wide and the third column will be 1000px wide.

#### Q8. What is the line-height property primarily used for?

- [x] to control the height of the space between two lines of content
- [ ] to control the height of the space between heading elements
- [ ] to control the height of the character size
- [ ] to control the width of the space between characters

#### Q9. Three of these choices are true about class selectors. Which is NOT true?

- [ ] Multiple classes can be used within the same element.
- [ ] The same class can be used multiple times per page.
- [ ] Class selectors with a leading period
- [x] Classes can be used multiple times per page but not within the same element.

#### Q10. There are many properties that can be used to align elements and create page layouts such as float, position, flexbox and grid. Of these four properties, which one should be used to align a global navigation bar which stays fixed at the top of the page?

- [x] position
- [ ] flexbox
- [ ] grid
- [ ] float

#### Q11. In the shorthand example below, which individual background properties are represented?

```css
background: blue url(image.jpg) no-repeat scroll 0px 0px;
```

- [x]
  ```css
  background-color: blue;
  background-image: url(image.jpg);
  background-repeat: no-repeat;
  background-attachment: scroll;
  background-position: 0px 0px;
  ```
- [ ]
  ```css
  background-color: blue;
  background-img: url(image.jpg);
  background-position: no-repeat;
  background-scroll: scroll;
  background-size: 0px 0px;
  ```
- [ ]
  ```css
  background-color: blue;
  background-src: url(image.jpg);
  background-repeat: no-repeat;
  background-wrap: scroll;
  background-position: 0px 0px;
  ```
- [ ]
  ```css
  background-color: blue;
  background-src: url(image.jpg);
  background-repeat: no-repeat;
  background-scroll: scroll;
  background-position: 0px 0px;
  ```

#### Q12. In the following example, according to cascading and specificity rules, what color will the link be?

```css
.example {
  color: yellow;
}
ul li a {
  color: blue;
}
ul a {
  color: green;
}
a {
  color: red;
}
```

```html
<ul>
  <li><a href="#" class="example">link</a></li>
  <li>list item</li>
  <li>list item</li>
</ul>
```

- [ ] green
- [x] yellow
- [ ] blue
- [ ] red

#### Q13. When elements overlap, they are ordered on the z-axis (i.e., which element covers another). The z-index property can be used to specify the z-order of overlapping elements. Which set of statements about the z-index property are true?

- [x] Larger z-index values appear on top of elements with a lower z-index value. Negative and positive numbers can be used. z-index can only be used on positioned elements.
- [ ] Smaller z-index values appear on top of elements with a larger z-index value. Negative and positive numbers can be used. z-index must also be used with positioned elements.
- [ ] Larger z-index values appear on top of elements with a lower z-index value. Only positive numbers can be used. z-index must also be used with positioned elements.
- [ ] Smaller z-index values appear on top of elements with a larger z-index value. Negative and positive numbers can be used. z-index can be used with or without positioned elements.

#### Q14. What is the difference between the following line-height settings?

```css
line-height: 20px;
line-height: 2;
```

- [x] The value of 20px will set the line-height to 20px. The value of 2 will set the line-height to twice the size of the corresponding font-size value.
- [ ] The value of 20px will set the line-height to 20px. The value of 2 is not valid.
- [ ] The value of 20px will set the line-height to 20px. The value of 2 will default to a value of 2px.
- [ ] The value of 20px will set the line-height to 20px. The value of 2 will set the line-height to 20% of the corresponding font-size value.

#### Q15. In the following example, what color will paragraph one and paragraph two be? (_Alternative_: In this example, what color will paragraphs one and two be?)

```html
<section>
  <p>paragraph one</p>
</section>

<p>paragraph two</p>
```

```css
section p {
  color: red;
}
section + p {
  color: blue;
}
```

- [ ] Paragraph one will be blue, paragraph two will be red.
- [ ] Both paragraphs will be blue.
- [x] Paragraphs one will be red, paragraph two will be blue.
- [ ] Both paragraphs will be red.

#### Q16. What are three valid ways of adding CSS to an HTML page?

- [ ]
  ```markdown
  1. External; CSS is written in a separate file.
  2. Inline; CSS is added to the <head> of the HTML page.
  3. Internal; CSS is included within the HTML tags.
  ```
- [ ]
  ```markdown
  1. External; CSS is written in a separate file and is linked within the <header> element of the HTML file.
  2. Inline; CSS is added to the HTML tag.
  3. Internal; CSS is included within the <header> element of the HTML file.
  ```
- [ ]
  ```markdown
  1. External; CSS is written in a separate file and is linked within the <head> element of the HTML file.
  2. Internal; CSS is included within the <header> element of the HTML file.
  3. Inline; CSS is added to the HTML tag.
  ```
- [x]
  ```markdown
  1. External; CSS is written in a separate file and is linked within the <head> element of the HTML file.
  2. Inline; CSS is added to the HTML tag.
  3. Internal; CSS is included within the <head> element of the HTML file.
  ```

#### Q17. Which of the following is true of the SVG image format? (_Alternative_: Which statement about the SVG image format is true?)

- [ ] CSS can be applied to SVGs but JavaScript cannot be.
- [ ] SVGs work best for creating 3D graphics.
- [x] SVGs can be created as a vector graphic or coded using SVG specific elements such as &#x3C;svg&#x3E;, &#x3C;line&#x3E;, and &#x3C;ellipse&#x3E;.
- [ ] SVGs are a HAML-based markup language for creating vector graphics.

#### Q18. In the example below, when will the color pink be applied to the anchor element?

```css
a:active {
  color: pink;
}
```

- [ ] The color of the link will display as pink after its been clicked or if the mouse is hovering over the link.
- [ ] The color of the link will display as pink on mouse hover.
- [x] The color of the link will display as pink while the link is being clicked but before the mouse click is released.
- [ ] The color of the link will display as pink before it has been clicked.

#### Q19. To change the color of an SVG using CSS, which property is used?

- [ ] Use background-fill to set the color inside the object and stroke or border to set the color of the border.
- [ ] The color cannot be changed with CSS.
- [ ] Use fill or background to set the color inside the object and stroke to set the color of the border.
- [x] Use fill to set the color inside the object and stroke to set the color of the border.

#### Q20. When using position: fixed, what will the element always be positioned relative to?

- [ ] the closest element with position: relative
- [x] the viewport
- [ ] the parent element
- [ ] the wrapper element

#### Q21. By default, a background image will repeat \_

- [ ] only if the background-repeat property is set to repeat
- [x] indefinitely, vertically, and horizontally
- [ ] indefinitely on the horizontal axis only
- [ ] once, on the x and y axis

#### Q22. When using media queries, media types are used to target a device category. Which choice lists current valid media types?

- [ ] print, screen, aural
- [ ] print, screen, television
- [x] print, screen, speech
- [ ] print, speech, device

#### Q23. How would you make the first letter of every paragraph on the page red?

- [x] p::first-letter { color: red; }
- [ ] p:first-letter { color: red; }
- [ ] first-letter::p { color: red; }
- [ ] first-letter:p { color: red; }

#### Q24. In this example, what is the selector, property, and value?

```css
p {
  color: #000000;
}
```

- [ ]
  ```markdown
  "p" is the selector
  "#000000" is the property
  "color" is the value
  ```
- [x]
  ```markdown
  "p" is the selector
  "color" is the property
  "#000000" is the value
  ```
- [ ]
  ```markdown
  "color" is the selector
  "#000000" is the property
  "#p" is the value
  ```
- [ ]
  ```markdown
  "color" is the selector
  "p" is the property
  "#000000" is the value
  ```

#### Q25. What is the rem unit based on?

- [ ] The rem unit is relative to the font-size of the p element.
- [ ] You have to set the value for the rem unit by writing a declaration such as rem { font-size: 1 Spx; }
- [ ] The rem unit is relative to the font-size of the containing (parent) element.
- [x] The rem unit is relative to the font-size of the root element of the page.

#### Q26. Which choice would give a block element rounded corners?

- [ ] `corner-radius: 10px;`
- [ ] `border-corner: 10px;`
- [ ] `corner-curve: 10px;`
- [x] `border-radius: 10px;`

[Official doc:](https://www.w3schools.com/css/css3_borders.asp)

#### Q27. In the following media query example, what conditions are being targeted?

```css
@media (min-width: 1024px), screen and (orientation: landscape) { … }
```

- [x] The rule will apply to a device that has either a width of 1024px or wider, or is a screen device in landscape mode.
- [ ] The rule will apply to a device that has a width of 1024px or narrower and is a screen device in landscape mode.
- [ ] The rule will apply to a device that has a width of 1024px or wider and is a screen device in landscape mode.
- [ ] The rule will apply to a device that has a width of 1024px or narrower, or is a screen device in landscape mode.

#### Q28. CSS transform properties are used to change the shape and position of the selected objects. The transform-origin property specifies the location of the element's transformation origin. By default, what is the location of the origin?

- [x] the top left corner of the element
- [ ] the center of the element
- [ ] the top right corner of the element
- [ ] the bottom left of the element

#### Q29. Which of the following is not a valid color value? (_Alternative:_ Which choice is not a valid color value?)

- [ ] `color: #000`
- [ ] `color: rgb(0,0,0)`
- [ ] `color: #000000`
- [x] `color: 000000`

#### Q30. What is the vertical gap between the two elements below?

```html
<div style="margin-bottom: 2rem;">Div 1</div>
<div style="margin-top: 2rem;">Div 2</div>
```

- [x] 2rem
- [ ] 32px
- [ ] 64px
- [ ] 4rem

[Reference MDN Webdocs](https://developer.mozilla.org/en-US/docs/Web/CSS/CSS_Box_Model/Mastering_margin_collapsing)

#### Q31. When using the Flexbox method, what property and value is used to display flex items in a column?

- [x] flex-flow: column; or flex-direction: column
- [ ] flex-flow: column;
- [ ] flex-column: auto;
- [ ] flex-direction: column;

#### Q32. Which type of declaration will take precedence?

- [ ] any declarations in user-agent stylesheets
- [x] important declarations in user stylesheets
- [ ] normal declarations in author stylesheets
- [ ] important declarations in author stylesheets

#### Q33. The flex-direction property is used to specify the direction that flex items are displayed. What are the values used to specify the direction of the items in the following examples?

![quote](https://raw.githubusercontent.com/ram-sah/LinkedIn-Assessments/master/CSS/images/rm-1.png)

- [x]
  - Example 1: `flex-direction: row;`
  - Example 2: `flex-direction: row-reverse;`
  - Example 3: `flex-direction: column;`
  - Example 4: `flex-direction: column-reverse;`
- [ ]
  - Example 1: `flex-direction: row-reverse;`
  - Example 2: `flex-direction: row;`
  - Example 3: `flex-direction: column-reverse;`
  - Example 4: `flex-direction: column;`
- [ ]
  - Example 1: `flex-direction: row;`
  - Example 2: `flex-direction: row-reverse;`
  - Example 3: `flex-direction: column;`
  - Example 4: `flex-direction: reverse-column;`
- [ ]
  - Example 1: `flex-direction: column;`
  - Example 2: `flex-direction: column-reverse;`
  - Example 3: `flex-direction: row;`
  - Example 4: `flex-direction: row-reverse;`

Note: Examples seem to be missing.

#### Q34. There are two sibling combinators that can be used to select elements contained within the same parent element; the general sibling combinator (~) and the adjacent sibling combinator (+). Referring to example below, which elements will the styles be applied to?

```css
h2 ~ p {
  color: blue;
}
h2 + p {
  background: beige;
}
```

```html
<section>
  <p>paragraph 1</p>
  <h2>Heading</h2>
  <p>paragraph 2</p>
  <p>paragraph 3</p>
</section>
```

- [ ] Paragraphs 2 and 3 will be blue. The h2 and paragraph 2 will have a beige background.
- [x] Paragraphs 2, and 3 will be blue, and paragraph 2 will have a beige background.
- [ ] Paragraph 2 will be blue. Paragraphs 2 and 3 will have a beige background.

#### Q35. When using flexbox, the "justify-content" property can be used to distribute the space between the flex items along the main axis. Which value should be used to evenly distribute the flex items within the container shown below?

![quote](https://raw.githubusercontent.com/ram-sah/LinkedIn-Assessments/master/CSS/images/rm-2.png)

- [x] justify-content: space-around;
- [ ] justify-content: center;
- [ ] justify-content: auto;
- [ ] justify-content: space-between;

#### Q36. There are many advantages to using icon fonts. What is one of those advantages?

- [ ] Icon fonts increase accessibility.
- [ ] Icon fonts can be used to replace custom fonts.
- [x] Icon fonts can be styled with typography related properties such as font-size and color.
- [ ] Icon fonts are also web safe fonts.

#### Q37. What is the difference between `display:none` and `visibility:hidden`?

- [ ] Both will hide the element on the page, but display:none has greater browser support. visibility:hidden is a new property and does not have the best browser support
- [ ] display:none hides the elements but maintains the space it previously occupied. visibility:hidden will hide the element from view and remove it from the normal flow of the document
- [x] display:none hides the element from view and removes it from the normal flow of the document. visibility:hidden will hide the element but maintains the space it previously occupied.
- [ ] There is no difference; both will hide the element on the page

#### Q38. What selector and property would you use to scale an element to be 50% smaller on hover?

- [ ] element:hover {scale: 0.5;}
- [x] element:hover {transform: scale(0.5);}
- [ ] element:hover {scale: 50%;}
- [ ] element:hover {transform: scale(50%);}

#### Q39. Which statement regarding icon fonts is true?

- [ ] Icon fonts can be inserted only using JavaScript.
- [ ] Icon fonts are inserted as inline images.
- [ ] Icon fonts require browser extensions.
- [x] Icon fonts can be styled with typography-related properties such as font-size and color.

#### Q40. The values for the font-weight property can be keywords or numbers. For each numbered value below, what is the associated keyword?

```css
font-weight: 400;
font-weight: 700;
```

- [ ] bold; normal
- [x] normal; bold
- [ ] light; normal
- [ ] normal; bolder

#### Q41. If the width of the container is 500 pixels, what would the width of the three columns be in this layout?

`.grid { display: grid; grid-template-columns: 50px 1fr 2fr; }`

- [x] 50px, 150px, 300px
- [ ] 50px, 200px, 300px
- [ ] 50px, 100px, 200px
- [ ] 50px, 50px, 100px

Note: an alternative for Q7.

#### Q42. Using the :nth-child pseudo class, what would be the most efficient way to style every third item in a list, no matter how many items are present, starting with item 2?

- [ ]
  ```css
  li:nth-child(3 + 2n) {
    margin: 0 5 px;
  }
  ```
- [x]
  ```css
  li:nth-child(3n + 2) {
    margin: 0 5 px;
  }
  ```
- [ ]
  ```css
  li:nth-child(2),
  li:nth-child(5),
  li:nth-child(8) {
    margin: 0 5 px;
  }
  ```
- [ ]
  ```css
  li:nth-child(2n + 3) {
    margin: 0 5 px;
  }
  ```

#### Q43. Which selector would select only internal links within the current page?

- [ ] `a[href="#"] {...}`
- [ ] `a[href~="#"]`
- [x] `a[href^="#"]`
- [ ] `a[href="#"]`

#### Q44. What is not true about class selectors?

- [x] Only one class value can be assigned to an element.
- [ ] An element can have multiple class value.
- [ ] Class selectors are marked with a leading period.
- [ ] More than one element can have the same class value.

#### Q45. What is the difference between the margin and padding properties?

- [ ] Margin adds space around and inside of an element; padding adds space only inside of an element.
- [x] Margin adds space around an element; padding adds space inside of an element.
- [ ] Margin adds a line around an element, padding adds space inside of an element.
- [ ] Margin adds space inside of an element, padding adds space around an element.

#### Q46. What is not a valid way of declaring a padding value of 10 pixels on the top and bottom, and 0 pixels on the left and right?

- [x] padding: 10px 10px 0px 0px;
- [ ] padding: 10px 0px;
- [ ] padding: 10px 0;
- [ ] padding: 10px 0px 10px 0px;

#### Q47. Is there an error in this code? If so, find the best description of the problem

```css
@font-face {
  font-family: 'Avenir', sans-serif;
  src: url('avenir.woff2') format('woff2'), url('avenir.woff') format('woff');
}
```

- [ ] The font file formats are not supported in modern browsers.
- [ ] The src attribute requires a comma between the URL and format values.
- [ ] There are no errors in the example.
- [x] The sans-serif inclusion is problematic.

#### Q48. Which style places an element at a fixed location within its container?

- [x] position: absolute;
- [ ] display: flex;
- [ ] display: block;
- [ ] float: left;

#### Q49. The calc() CSS function is often used for calculating relative values. In the example below, what is the specified margin-left value?

```css
.example {
  margin-left: calc(5% + 5px);
}
```

- [x] The left margin value is equal to 5% of its parents element's width plus 5px
- [ ] The left margin value is equal to 5% of the viewport width plus 5px
- [ ] The left margin value is equal to 5% of the closest positioned element's width plus 5px
- [ ] The left margin value is equal to 5% of the selected element's width (.example) plus 5px

#### Q50. What is the CSS selector for an `<a>` tag containing the title attribute?

- [x] `a[title]`
- [ ] `a > title`
- [ ] `a=title`
- [ ] `a.title`

Note: an alternative for Q2.

#### Q51. Which code would you use to absolutely position an element of the logo class?

- [x] `.logo { position: absolute; left: 100px; top: 150px; }`
- [ ] `.logo { position: absolute; margin-left: 100px; margin-top: 150px; }`
- [ ] `.logo { position: absolute; padding-left: 100px; padding-top: 150px; }`
- [ ] `.logo { position: absolute; left-padding: 100px; top-padding: 150px; }`

#### Q52. In this example, what color will Paragraph 1 be?

```css
p:first-of-type {
  color: red;
}
p {
  color: blue;
}
.container {
  color: yellow;
}
p:first-child {
  color: green;
}
```

```html
<div class="container">
  <h1>Heading</h1>
  <p>Paragraph1</p>
  <p>Paragraph2</p>
</div>
```

- [ ] blue
- [ ] green
- [x] red
- [ ] yellow

#### Q53. What is the `::placeholder pseudo-element` used for?

- [x] It is used to format the appearance of placeholder text within a form control.
- [ ] It specifies the default input text for a form control.
- [ ] It writes text content into a hyperlink tooltip.
- [ ] It writes text content into any page element.

#### Q54. Which statement is true of the single colon (`:`) or double colon (`::`) notations for pseudo-elements-for example, `::before` and `:before`?

- [ ] All browsers support single and double colons for new and older pseudo-elements. So you can use either but it is convention to use single colons for consistency.
- [ ] In CSS3, the double colon notation (`::`) was introduced to create a consistency between pseudo-elements from pseudo-classes. For newer browsers, use the double colon notation. For IE8 and below, using single colon notation (`:`).
- [ ] Only the new CSS3 pseudo-elements require the double colon notation while the CSS2 pseudo-elements do not.
- [x] In CSS3, the double colon notation (`::`) was introduced to differentiate pseudo-elements from pseudo-classes. However, modern browsers support both formats. Older browsers such as IE8 and below do not.

#### Q55. Which choice is not valid value for the font-style property?

- [ ] normal
- [ ] italic
- [x] none
- [ ] oblique

#### Q56. When would you use the @font-face method?

- [ ] to set the font size of the text
- [x] to load custom fonts into stylesheet
- [ ] to change the name of the font declared in the font-family
- [ ] to set the color of the text

#### Q57. When elements within a container overlap, the z-index property can be used to indicate how those items are stacked on top of each other. Which set of statements is true?

- [x]
  ```markdown
  1. Larger z-index values appear on top elements with a lower z-index value.
  2. Negative and positive number can be used.
  3. z-index can be used only on positioned elements.
  ```
- [ ]
  ```markdown
  1. Smaller z-index values appear on top of elements with a larger z-index value.
  2. Negative and positive numbers can be used.
  3. z-index can be used with or without positioned elements.
  ```
- [ ]
  ```markdown
  1. Smaller z-index values appear on top of elements with a larger z-index value.
  2. Negative and positive number can be used.
  3. z-index must also be used with positioned elements.
  ```
- [ ]
  ```markdown
  1. Larger z-index values appear on top of elements with a lower z-index value.
  2. Only positive number can be used.
  3. z-index must also be used with positioned elements.
  ```

Note: an alternative for Q13.

#### Q58. You have a large image that needs to fit into a 400 x 200 pixel area. What should you resize the image to if your users are using Retina displays?

- [ ] 2000 x 1400 pixels
- [ ] 200 x 100 pixels
- [x] 800 x 400 pixels
- [ ] 400 x 200 pixels

#### Q59. In Chrome's Developer Tools view, where are the default styles listed?

- [x] under the User Agent Stylesheet section on the right
- [ ] in the third panel under the Layout tab
- [ ] under the HTML view on the left
- [ ] in the middle panel

#### Q60. While HTML controls document structure, CSS controls `___`.

- [ ] semantic meaning
- [ ] content meaning
- [ ] document structure
- [x] content appearance

#### Q61. What is the recommended name you should give the folder that holds your project's images?

- [x] images
- [ ] #images
- [ ] Images
- [ ] my images

#### Q62. What is an advantage of using inline CSS?

- [ ] It is easier to manage.
- [x] It is easier to add multiple styles through it.
- [ ] It can be used to quickly test local CSS overrides.
- [ ] It reduces conflict with other CSS definition methods.

#### Q63. Which W3C status code represents a CSS specification that is fully implemented by modern browsers?

- [ ] Proposed Recommendation
- [ ] Working Draft
- [x] Recommendation
- [ ] Candidate Recommendation

#### Q64. Are any of the following declarations invalid?

```css
color: red; /* declaration A */
font-size: 1em; /* declaration B */
padding: 10px 0; /* declaration C */
```

- [ ] Declaration A is invalid.
- [ ] Declaration B is invalid.
- [ ] Declaration C is invalid.
- [x] All declarations are valid.

#### Q65. Which CSS will cause your links to have a solid blue background that changes to semitransparent on hover?

- [x]
  ```css
  a:link {
    background: #0000ff;
  }
  a:hover {
    background: rgba(0, 0, 255, 0.5);
  }
  ```
- [ ]
  ```css
  a {
    color: blue;
  }
  a:hover {
    background: white;
  }
  ```
- [ ]
  ```css
  a:link {
    background: blue;
  }
  a:hover {
    color: rgba(0, 0, 255, 0.5);
  }
  ```
- [ ]
  ```css
  a:hover {
    background: rgba(blue, 50%);
  }
  a:link {
    background: rgba(blue);
  }
  ```

#### Q66. Which CSS rule takes precedence over the others listed?

- [ ] `div.sidebar {}`
- [ ] `* {}`
- [x] `div#sidebar2 p {}`
- [ ] `.sidebar p {}`

#### Q67. The body of your page includes some HTML sections. How will it look with the following CSS applied?

```css
body {
  background: #ffffff; /* white */
}
section {
  background: #0000ff; /* blue */
  height: 200px;
}
```

- [x] blue sections on a white background
- [ ] Yellow sections on a blue background
- [ ] Green sections on a white background
- [ ] blue sections on a red background

#### Q68. Which CSS keyword can you use to override standard source order and specificity rules?

- [ ] `!elevate!`
- [ ] `*prime`
- [ ] `override`
- [x] `!important`

#### Q69. You can use the `___` pseudo-class to set a different color on a link if it was clicked on.

- [x] `a:visited`
- [ ] `a:hover`
- [ ] `a:link`
- [ ] `a:focus`

#### Q70. Which color will look the brightest on your screen, assuming the background is white?

- [ ] `background-color: #aaa;`
- [ ] `background-color: #999999;`
- [ ] `background-color: rgba(170,170,170,0.5);`
- [x] `background-color: rgba(170,170,170,0.2);`

#### Q71. Which CSS selector can you use to select all elements on your page associated with the two classes header and clear?

- [ ] `."header clear" {}`
- [ ] `header#clear {}`
- [x] `.header.clear {}`
- [ ] `.header clear {}`

#### Q72. A universal selector is specified using a(n) `___`.

- [ ] "h1" string
- [ ] "a" character
- [ ] "p" character
- [x] "\*" character

#### Q73. In the following CSS code, `'h1'` is the `___`, while `'color'` is the `___`.

```css
h1 {
  color: red;
}
```

- [ ] property; declaration
- [ ] declaration; rule
- [ ] "p" character
- [x] selector; property

#### Q74. What is an alternate way to define the following CSS rule?

```css
font-weight: bold;
```

- [ ] font-weight: 400;
- [ ] font-weight: medium;
- [x] font-weight: 700;
- [ ] font-weight: Black;

#### Q75. You want your styling to be based on a font stack consisting of three fonts. Where should the generic font for your font family be specified?

- [ ] It should be the first one on the list.
- [ ] Generic fonts are discouraged from this list.
- [x] It should be the last one on the list.
- [ ] It should be the second one on the list.

#### Q76. What is one disadvantage of using a web font service?

- [ ] It requires you to host font files on your own server.
- [ ] It uses more of your site's bandwidth.
- [ ] It offers a narrow selection of custom fonts.
- [x] It is not always a free service.

#### Q77. How do you add Google fonts to your project?

- [x] by using an HTML link element referring to a Google-provided CSS
- [ ] by embedding the font file directly into the project's master JavaScript
- [ ] by using a Google-specific CSS syntax that directly links to the desired font file
- [ ] by using a standard font-face CSS definition sourcing a font file on Google's servers

#### Q78. Using the following HTML and CSS example, what will equivalent pixel value be for .em and .rem elements?

```css
html {
  font-size: 10px;
}
body {
  font-size: 2rem;
}
.rem {
  font-size: 1.5rem;
}
.em {
  font-size: 2em;
}
```

```html
<body>
  <p class="rem"></p>
  <p class="em"></p>
</body>
```

- [ ] The .rem will be equivalent to 25px; the .em value will be 20px.
- [ ] The .rem will be equivalent to 15px; the .em value will be 20px.
- [x] The .rem will be equivalent to 15px; the .em value will be 40px.
- [ ] The .rem will be equivalent to 20px; the .em value will be 40px.

#### Q79. What property is used to adjust the space between text characters?

- [ ] `font-style`
- [ ] `text-transform`
- [ ] `font-variant`
- [x] `letter-spacing`

#### Q80. What is the correct syntax for changing the cursor from an arrow to a pointing hand when it interacts with a named element?

- [x] `.element {cursor: pointer;}`
- [ ] `.element {cursor: hand;}`
- [ ] `.element {cursor: move-hand;}`
- [ ] `.element {cursor: pointer-hand;}`

#### Q81. What is the effect of this style?

```css
background-position: 10% 50%;
```

- [x] The background image is placed 10% from the left and 50% from the top of its container
- [ ] The background image is placed 10% from the bottom and 50% from the left of its container
- [ ] The background image is placed 10% from the right and 50% from the bottom of its container
- [ ] The background image is placed 10% from the top and 50% from the left of its container

#### Q82. How will the grid items display?

```css
grid-template-columns: 2fr 1fr;
```

- [ ] The first column is twice the height of the second column and will be as wide as the content
- [ ] The first column is half the size of the container and the second column will absorb the remaining space
- [x] The first column is twice as wide as the second column and will fit proportionally within the grid container
- [ ] The first column is twice the width and height of the second column, and will fit proportionally within the grid container

#### Q83. Which style rule would make the image 50% smaller during a hover?

```html
<img id="photo" alt="" src="..." />
```

- [ ] img#photo:hover {scale: 0.5;}
- [x] img#photo:hover {transform: scale(0.5);}
- [ ] img#photo {hover-scale: 0.5;}
- [ ] img#photo:hover {size: smaller;}

#### Q84. Which CSS properties can you use to create a rounded corner on just the top-left and top-right corners of an element?

```css
A. border-radius: 10px 10px 0 0;
B. border-top-left-radius: 10px; and border-top-right-radius: 10px;
C. border-radius: 10px 0;
D. border-top-radius: 10px;
```

- [ ] A and C
- [ ] C and D
- [ ] B and C
- [x] A and B

#### Q85. Review the HTML example below. Then choose the list of selectors that select the \<p>, from lowest to highest specificity.

```html
<section>
  <p class="example">...</p>
</section>
```

- [ ]
  ```css
  1. section \* {
    ...;
  }
  2. [class*='example'] {
    ...;
  }
  3. p.example {
    ...;
  }
  4. section p {
    ...;
  }
  ```
- [ ]
  ```css
  1. p {
    ...;
  }
  2. p.example {
    ...;
  }
  3. section p {
    ...;
  }
  4. [class*='example'] {
    ...;
  }
  ```
- [ ]
  ```css
  1. p.example {
    ...;
  }
  2. section p {
    ...;
  }
  3. [class*='example'] {
    ...;
  }
  4. section \* {
    ...;
  }
  ```
- [x]
  ```css
  1. p {
    ...;
  }
  2. section p {
    ...;
  }
  3. [class*='example'] {
    ...;
  }
  4. p.example {
    ...;
  }
  ```

#### Q86. Which property is used to create a drop shadow effect on an HTML element?

- [ ] element-shadow
- [ ] outer-shadow
- [ ] dropbox-shadow
- [x] box-shadow

#### Q87. What is the correct selector for targeting all text inputs that are not disabled?

- [x] `input[type="text"]:not([disabled]) {...}`
- [ ] `input[type="text"]:not("disabled") {...}`
- [ ] `input[type*="text"]:not([disabled="disabled"]) {...}`
- [ ] `input[type="text"]:not([type="disabled"]) {...}`

`input[type="text"]` selects all the input with type text, and `:not([disabled])` selects all the elements not having the attribute "disabled". Combining both only selects all the input elements with type attribte as "text" and not having "disabled" attribute.`

[Reference link attribute-selector](https://www.w3schools.com/css/css_attribute_selectors.asp)

[Reference link-:not()](https://developer.mozilla.org/en-US/docs/Web/CSS/:not)

#### Q88. How can you create a semi-transparent background color?

- [ ] `background-color: hsl(0, 0, 0, 0.5);`
- [ ] `background-color: rgbx(0, 0, 0, 0.5);`
- [x] `background-color: rgba(0, 0, 0, 0.5);`
- [ ] `background-color: rgba(0, 0, 0, 1);`

`rgba` is a funtion in css. rgba stands for red, green, blue and alpha. The value of alpha can be between 0 and 1 both inclusive with 0 being fully transparent and 1 being fully opaque.

[Reference link-rgba](https://www.w3schools.com/cssref/func_rgba.asp)

#### Q89. Using this HTML markup, how would you select only the headings contained within the `<header>` element?

```html
<header>
  <hl>Heading 1</h1>
  <h2>Heading 2</h2>
</header>
<h2>Heading 2</h2>
```

- [x] `header h1, header h2 {...}`
- [ ] `header h1 + header h2 {...}`
- [ ] `header h1, h2 {...}`
- [ ] `h1, h2 {...}`

#### Q90. Suppose you want to have a list of items (.item) displayed in a row and in reverse order using flexbox. What is the error in the CSS below?

```css
.container {
  display: flex;
}
.item {
  border: 1px solid red;
  flex-direction: row-reverse;
}
```

- [ ] The value for flex-direction should be reverse-row.
- [ ] The .container element should have a property of flex: display.
- [x] The flex-direction property should be declared in the container.
- [ ] The display value should be flex-inline to display the items in a row.

#### Q91. Which choice is not a valid transition?

- [x] `transition: margin 1000ms ease-in-out;`
- [ ] `transition: color 1.3s ease-in;`
- [ ] `transition: position 400ms linear;`
- [ ] `transition: opacity 1s ease-in;`

#### Q92. In this example, what color will the paragraphs be and why?

```css
article p {
  color: blue;
}
article > p {
  color: green;
}
```

```html
<article>
  <p>Paragraph 1</p>

  <aside>
    <p>Paragraph 2</p>
  </aside>
</article>
```

- [ ] Paragraph 1 will be blue. Paragraph 2 will be green.
- [ ] Both paragraphs will be green.
- [x] Paragraph 1 will be green. Paragraph 2 will be blue.
- [ ] Both paragraphs will be blue.

#### Q93. Review the declaration of border style shown below. What is the corresponding longhand syntax?

```css
border: 1px solid red;
```

- [ ]
  ```css
  border-size: 1px;
  border-style: solid;
  border-color: red;
  ```
- [ ]
  ```css
  border-size: 1px;
  border-type: solid;
  border-color: red;
  ```
- [x]
  ```css
  border-width: 1px;
  border-style: solid;
  border-color: red;
  ```
- [ ]
  ```css
  border-width: 1px;
  border-line: solid;
  border-color: red;
  ```

#### Q94. Pseudo-classes are used to `_`.

- [x] style the state of the selected element
- [ ] insert presentational content
- [ ] style a specific part of the selected element
- [ ] style the elements using class selectors

#### Q95. In this example, what styles will be applied to which elements?

```css
section {
  color: gray;
}
```

```html
<section>
  <p>paragraph</p>
  <a href="#">link</a>
</section>
```

- [ ] The paragraph and link will be gray.
- [ ] The background color of the section element will be gray.
- [ ] The paragraph will be gray. The link will be the browser default, black.
- [x] Only the paragraph will be gray.

#### Q96. Which answer is an example of a type selector (also sometimes referred to as an element selector)?

- [ ] `.header {...}`
- [x] `header {...}`
- [ ] `#header {...}`
- [ ] `header > h1 {...}`

#### Q97. What is the correct order for listing different link states in a website so those states display correctly on the page?

- [ ]
  ```css
  a
  a:hover
  ```
- [ ]
  ```css
  :link
  :visited
  :hover
  :active
  :focus
  ```
- [ ]
  ```css
  :active
  :focus
  :hover
  :link
  :visited
  ```
- [x]
  ```css
  :link
  :visited
  :focus
  :hover
  :active
  ```

#### Q98. Which selector is used to select the paragraph element that is a direct descendent of section?

- [ ] `section * p`
- [ ] `section + p`
- [ ] `section ~ p`
- [x] `section > p`

[Child combinator](https://developer.mozilla.org/en-US/docs/Web/CSS/Child_combinator)

#### Q99. For this code, what is the font color of the hypertext link?

```css
ul {
  --color: red;
}
p {
  color: var(--color);
}
a {
  color: var(--color, orange);
}
```

```html
<p>Paragraph</p>
<ul>
  <li>
    <a href="#">list item a link </a>
  </li>
  <li>list item</li>
</ul>
```

- [x] red
- [ ] orange
- [ ] blue
- [ ] black

[Reference](https://www.sitepoint.com/pseudo-classes-the-basics/)

#### Q100. Which statement is not true?

- [ ] Specificity determines which CSS rule is applied by the browsers.
- [x] When two selectors apply to the same element, the one with lower specificity wins.
- [ ] The last rule defined overrides all previous rules and even conflicting rules.
- [ ] Rules with more specific selectors have greater specificity.

[Reference](https://www.smashingmagazine.com/2007/07/css-specificity-things-you-should-know/)

#### Q101. What is the output of the margin value when used within this context, assuming that its containing element is larger than 800px?

```css
.example {
  width: 800px;
  margin: 0 auto;
}
```

- [ ] The example element will have 0 margin space around the whole element. The auto value will center align the element horizontally and vertically within its container.

- [ ] The example element will have 0 margin space on the left and right. It will be sized automatically on the top and bottom, which will center align the element within its container.

- [x] The example element will have 0 margin space on the top and bottom. The margin will be sized automatically on the left and right, which may center align the element within its container.

- [ ] The margin value is invalid because its missing a unit measurement after the 0.

[Source: SOW](https://stackoverflow.com/questions/3170772/what-does-auto-do-in-margin-0-auto)

#### Q102. There are currently four viewport-percentage lengths that can be used to define the value relative to the viewport size: vw, vh, vmin, and vmax. If the current viewport size has a width of 800px and a height of 600px, what will these values be equivalent to in pixels?

```css
10vw = ?px
10vh = ?px
10vmin = ?px
10vmax = ?px
```

- [x] 10vw = 80px
      10vh = 60px
      10vmin = 60px
      10vmax = 80px

- [ ] 10vw = 60px
      10vh = 80px
      10vmin = 80px
      10vmax = 60px

- [ ] 10vw = 8px
      10vh = 6px
      10vmin = 6px
      10vmax = 8px

- [ ] 10vw = 6px
      10vh = 8px
      10vmin = 8px
      10vmax = 6px

#### Q103. Which element(s) will be blue?

```css
h2 ~ p {
  color: blue;
}
```

```html
<section>
  <p>P1</p>
  <h2>H2</h2>
  <p>P3</p>
  <p>P4</p>
</section>
```

- [ ] P3P3
- [ ] P1P1
- [ ] P1, P3, and P4P1, P3, and P4
- [x] P3 and P4

#### Q104. Referring to the HTML markup and CSS example below, which element(s) will be targeted?

```css
p:first-of-type:first-letter {
  color: red;
}
```

```html
<body>
  <p>Paragraph 1.</p>
  <p>Paragraph 2.</p>

  <article>
    <h1>Heading</h1>
    <p>Paragraph 3.</p>
    <p>paragraph 4.</p>
  </article>

  <section>
    <p>Paragraph 5.</p>
    <p>Paragraph 6.</p>
  </section>
</body>
```

- [ ] The first letter in all paragraphs will be red.
- [ ] Only the first letter in paragraphs 1 and 5 will be red.
- [x] The first letter in paragraphs 1, 3, and 5 will be red.
- [ ] Only the first letter in paragraph 1 will be red.Only

#### Q105. Which five style features are associated with the box model?

- [x] margin, padding, border, width, height
- [ ] width, height, z-index, overflow, font size
- [ ] margin, padding, font size, line height, border
- [ ] font size, line height, letter spacing, width, height

#### Q106. Which choice will not set all links that include domain.com to pink?

- [ ] A

```css
a[href$='domain.com'] {
  color: pink;
}
```

- [x] B

```css
a[href='*domain.com'] {
  color: pink;
}
```

- [ ] C

```css
a[href*='domain.com'] {
  color: rgb(255, 155, 155);
}
```

- [ ] D

```css
a[href*='domain.com'] {
  color: pink;
}
```

[Reference](https://www.smashingmagazine.com/2007/07/css-specificity-things-you-should-know/)

#### Q107. Which property and value pair could be used to apply a linear gradient effect?

- [x] `css background: linear-gradient(#648880, #293f50);`
- [ ] `css background-image: linear(#648880, #293f50);`
- [ ] `css background: gradient(linear, #648880, #293f50);`
- [ ] `css background-color: linear-gradient(#648880, #293f50);`

#### Q108. You want to add a background circle behind an icon. Which style declaration is correct?

- [ ] A

```css
.glyphicon-bgcircle {
  circle-radius: 50%;
  margins: 50px;
  background-color: #fdadc6;
  color: rgba(255, 255, 255, 1);
  font-size: 24px;
}
```

- [ ] B

```css
glyphicon-bgcircle {
  border-circle: 50%;
  padding: 50px;
  background-color: #fdadc6;
  color: rgba(255, 255, 255, 1);
  font-size: 24px;
}
```

- [x] C

```css
.glyphicon-bgcircle {
  border-radius: 50%;
  padding: 50px;
  background-color: #fdadc6;
  color: rgba(255, 255, 255, 1);
  font-size: 24px;
}
```

- [ ] D

```css
.glyphicon-bgcircle {
  radius-rounded: 50%;
  margins: auto;
  background-color: #fdadc6;
  color: rgba(255, 255, 255, 1);
  font-size: 24px;
}
```

#### Q109. When using a font stack to declare the font family, in what order should the values appear?

- [x] The first value is the first choice, followed by alternative options, ordered by preference. The last option should be a generic font.
- [ ] The first value is the first choice. The order of the alternative options does not matter. It depends on what is available on the user's computer.
- [ ] The first value is the first choice, and must be followed by at least one alternative option before adding the generic font.
- [ ] The first value is the first choice, followed by a maximum of three alternatives.

#### Q110. Which items are valid values for the font-size property?

```css
A. font-size: xsmall
B. font-size: 50%
C. font-size: 1em
D. font-size: 20px
```

- [ ] C, D
- [x] B, C, D
- [ ] A, C
- [ ] A, B, C, D

#### Q111. In this image, the blue box and sample text are both contained within the same parent element. The blue box is floated on the left margin of the container. Why is it not contained with the container?

![Sample text](https://raw.githubusercontent.com/ram-sah/LinkedIn-Assessments/master/CSS/images/rm-3.png)

- [ ] Floating the blue box increased its height.
- [ ] Floating the blue box on the left also moves it down.
- [ ] Floating the blue box actually shifts it to the right and down.
- [x] Floating the blue box took it out of document flow and the container is sized only to the sample text.

#### Q112. Given this code, which CSS declaration of .overlay will span the entire width and height of its container?

```css
<style>
.container {
  position: relative;
  height: 200px;
  width: 200px;
  border: 1px solid black;
}
</style>
<div class="container"><div class="overlay"></div></div>
```

- [ ] A

```css
.overlay {
  position: static;
  top: 200px;
  bottom: 200px;
  right: 200px;
  left: 200px;
  background-color: rgba(0, 0, 0, 0.5);
}
```

- [ ] B

```css
.overlay {
  position: absolute;
  top: 200px;
  bottom: 200px;
  right: 200px;
  left: 200px;
  background-color: rgba(0, 0, 0, 0.5);
}
```

- [ ] C

```css
.overlay {
  position: static;
  top: 0;
  bottom: 0;
  right: 0;
  left: 0;
  background-color: rgba(0, 0, 0, 0.5);
}
```

- [x] D

```css
.overlay {
  position: absolute;
  top: 0;
  bottom: 0;
  right: 0;
  left: 0;
  background-color: rgba(0, 0, 0, 0.5);
}
```

#### Q113. Which missing line of code would place the text on top of the image?

```js
<div class="container">
  <img src="grumpy-cat.gif" />
  <p>The z-index property is cool!</p>
</div>
```

```css
img {
  position: absolute;
  left: 0px;
  top: 0px;
  // Missing line
}
```

- [ ] `z-index: 1;`
- [x] `z-index: -1;`
- [ ] `z-index: 0;`
- [ ] `z-index: true;`

#### Q114. To make the font size of an element one size smaller than the font size of the element's container, which style property would you apply?

- [ ] `font-size: reduce;`
- [ ] `font-size: 8px;`
- [ ] `font-size: -1em;`
- [x] `font-size: smaller;`

#### Q115. Given this markup, which selector would result in the text being highlighted in yellow?

```js
<span class="highlight">#BLM</span>
```

- [ ] A

```css
.highlight {
  background-color: yellow;
}
```

- [ ] B

```css
#highlight {
  background-color: yellow;
}
```

- [x] C

```css
.highlight {
  color: yellow;
}
```

- [ ] D

```css
#highlight {
  color: yellow;
}
```

#### Q116. To prevent a background image from tiling in any direction, which style property would you apply?

- [x] A

```css
background-repeat: no-repeat;
```

- [ ] B

```css
background-repeat: fixed;
```

- [ ] C

```css
background-repeat: none;
```

- [ ] D

```css
background-tile: none;
```

#### Q117. To rotate an object 30 degrees counterclockwise, which style property would you apply?

- [x] `transform: rotate(-30deg);`
- [ ] `transform: rotate(30deg);`
- [ ] `rotate: 30deg;`
- [ ] `spin: 30deg;`

[Reference](<https://developer.mozilla.org/en-US/docs/Web/CSS/transform-function/rotate()>)

#### Q118. Which style rule would you apply to set the background image to display the contents of the wood.png file?

- [ ] `background-image: file('wood.png');`
- [x] `background-image: url('wood.png');`
- [ ] `background-image: wood.png;`
- [ ] `image: wood.png`

#### Q119. What style rule would set the font color of only paragraph two to blue?

```js
<section><p>paragraph one</p></section><p>paragraph two</p>
```

- [ ] A

```css
section > p {
  color: blue;
}
```

- [ ] B

```css
p {
  color: blue;
}
```

- [x] C

```css
section + p {
  color: blue;
}
```

- [ ] D

```css
p + section {
  color: blue;
}
```

[Reference](https://www.w3schools.com/cssref/sel_element_pluss.asp)

#### Q120. You want to move an element up 100px. Which CSS property would you use?

- [ ] `transform: translateX(-100px)`
- [x] `transform: translateY(-100px)`
- [ ] `transform: translateY(100px)`
- [ ] `transform: translateX(100px)`

#### Q121. Which style will horizontally center the inner &lt;div&gt; within the outer &lt;div&gt;?

```js
<div id="outer">
  <div id="inner">Center Me!</div>
</div>
```

- [ ] A

```css
#inner {
  width: 50%;
}

#outer {
  width: 100%;
}
```

- [ ] B

```css
#inner {
  left: 0;
  right: 0;
  position: center;
}
```

- [ ] C

```css
#inner {
  text-align: center;
}
```

- [x] D

```css
#inner {
  width: 50%;
  margin: 0 auto;
}
```

#### Q122. Which corner will the puppy be in when these CSS rules are applied?

```css
.pen {
  height: 100px;
  width: 100px;
  border: 2px dashed brown;
  position: relative;
}

#puppy {
  position: absolute;
  right: 80px;
  bottom: 0px;
}
```

```html
<div class="pen">
  <span id="puppy">🐶</span>
</div>
```

- [ ] top-right corner
- [ ] bottom-right corner
- [ ] top-left corner
- [x] bottom-left corner

#### Q123. Which choice uses the correct syntax for adding a hover pseudo class to <a> element ?

- [x] `a:hover {...}`
- [ ] `a :hover {...}`
- [ ] `a.hover {...}`
- [ ] `a hover {...}`

[Reference](https://stackoverflow.com/questions/1935820/set-ahover-based-on-class)

#### Q124. Which missing code will give "Cellar Door" a shadow?

```css
  <style>
    #cellar-door {
      box-shadow: 3px 5px 10px #000;
    }
    .text-shadow {
      text-shadow: 3px 5px 10px #000;
    }
  </style>

  <h1 _____> Cellar Door</h1>
```

- [x] `class="text-shadow"`
- [ ] `id="cellar-door"`
- [ ] `id="text-shadow"`
- [ ] `class="cellar-door"`

[Reference](https://www.w3schools.com/html/html_classes.asp)

#### Q125. Which choice is a valid example of a comment in CSS?

- [ ] -- This line has been cancelled.
- [x] /* This line has been cancelled. */
- [ ] // This line has been cancelled.
- [ ] # This line has been cancelled.

[Reference](https://www.w3schools.com/css/css_comments.asp)

#### Q126. Which element(s) will be displayed in blue text?

```css
    h2 ~ p {
      color: blue;
    }
  <section>
    <p>P1</p>
    <h2>H2</h2>
    <p>P3</p>
    <p>P4</p>
  </section>
```

- [ ] P3
- [ ] P1, P3 and P4
- [x] P3 and P4
- [ ] P1

[Reference](https://www.w3docs.com/snippets/css/what-does-the-css-tilde-selector-mean.html)
## JavaScript

#### Q1. Which operator returns true if the two compared values are not equal?

- [ ] `<>`
- [ ] `~`
- [ ] `==!`
- [x] `!==`

[Reference Javascript Comparison Operators](https://www.w3schools.com/js/js_operators.asp)

#### Q2. How is a forEach statement different from a for statement?

- [ ] Only a for statement uses a callback function.
- [x] A for statement is generic, but a forEach statement can be used only with an array.
- [ ] Only a forEach statement lets you specify your own iterator.
- [ ] A forEach statement is generic, but a for statement can be used only with an array.

[Reference Differences between forEach and for loop](https://www.geeksforgeeks.org/difference-between-foreach-and-for-loop-in-javascript/)

#### Q3. Review the code below. Which statement calls the addTax function and passes 50 as an argument? How would you use this function to find out how much tax should be paid on \$50?

```js
function addTax(total) {
  return total * 1.05;
}
```

- [ ] `addTax = 50;`
- [ ] `return addTax 50;`
- [x] `addTax(50);`
- [ ] `addTax 50;`

[Reference functions in javascript](https://www.w3schools.com/js/js_functions.asp)

#### Q4. Which statement is the correct way to create a variable called rate and assign it the value 100?

- [x] `let rate = 100;`
- [ ] `let 100 = rate;`
- [ ] `100 = let rate;`
- [ ] `rate = 100;`

[Reference Javascript Assignment operators](https://www.w3schools.com/js/js_operators.asp)

#### Q5. Which statement creates a new object using the Person constructor? Which statement creates a new Person object called "student"?

- [x] `var student = new Person();`
- [ ] `var student = construct Person;`
- [ ] `var student = Person();`
- [ ] `var student = construct Person();`

[Reference](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Classes)

#### Q6. When would the final statement in the code shown be logged to the console? When would 'results shown' be logged to the console?

```js
let modal = document.querySelector('#result');
setTimeout(function () {
  modal.classList.remove('hidden');
}, 10000);
console.log('Results shown');
```

- [ ] after 10 second
- [ ] after results are received from the HTTP request
- [ ] after 10000 seconds
- [x] immediately

[Reference Javascript is synchronous and single threaded](https://stackoverflow.com/a/2035662/15067394)

#### Q7. Which snippet could you add to this code to print "food" to the console?

```javascript
class Animal {
  static belly = [];
  eat() {
    Animal.belly.push('food');
  }
}
let a = new Animal();
a.eat();
console.log(/* Snippet Here */); //Prints food
```

- [ ] `a.prototype.belly[0]`
- [ ] `Object.getPrototype0f (a).belly[0]`
- [x] `Animal.belly[0]`
- [ ] `a.belly[0]`

[Reference Javascript Class static Keyword](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Classes/static)

#### Q8. You've written the code shown to log a set of consecutive values, but it instead results in the value 5, 5, 5, and 5 being logged to the console. Which revised version of the code would result in the value 1, 2, 3 and 4 being logged?

```javascript
for (var i = 1; i <= 4; i++) {
  setTimeout(function () {
    console.log(i);
  }, i * 10000);
}
```

- [ ]

```javascript
for (var i = 1; i <= 4; i++) {
  (function (i) {
    setTimeout(function () {
      console.log(j);
    }, j * 1000);
  })(j);
}
```

- [ ]

```javascript
while (var i=1; i<=4; i++) {
  setTimeout(function() {
    console.log(i);
    }, i*1000);
}
```

- [x]

```javascript
for (var i = 1; i <= 4; i++) {
  (function (j) {
    setTimeout(function () {
      console.log(j);
    }, j * 1000);
  })(i);
}
```

- [ ]

```javascript
for (var j = 1; j <= 4; j++) {
  setTimeout(function () {
    console.log(j);
  }, j * 1000);
}
```

1. [Reference setTimeout](https://developer.mozilla.org/en-US/docs/Web/API/setTimeout)
2. [Reference immediately invoked anonymous functions](https://www.javascripttutorial.net/javascript-anonymous-functions/)

#### Q9. How does a function create a closure?

- [ ] It reloads the document whenever the value changes.
- [x] It returns a reference to a variable in its parent scope.
- [ ] It completes execution without returning.
- [ ] It copies a local variable to the global scope.

[Reference](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Closures)

#### Q10. Which statement creates a new function called discountPrice?

- [x]

```js
let discountPrice = function (price) {
  return price * 0.85;
};
```

- [ ]

```js
let discountPrice(price) {
  return price * 0.85;
};
```

- [ ]

```js
let function = discountPrice(price) {
  return price * 0.85;
};
```

- [ ]

```js
discountPrice = function (price) {
  return price * 0.85;
};
```

[Reference defining javascript functions](https://www.w3schools.com/js/js_functions.asp)

#### Q11. What is the result in the console of running the code shown?

```js
var Storm = function () {};
Storm.prototype.precip = 'rain';
var WinterStorm = function () {};
WinterStorm.prototype = new Storm();
WinterStorm.prototype.precip = 'snow';
var bob = new WinterStorm();
console.log(bob.precip);
```

- [ ] Storm()
- [ ] undefined
- [ ] 'rain'
- [x] 'snow'

[Reference prototype chain](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Inheritance_and_the_prototype_chain)

#### Q12. You need to match a time value such as 12:00:32. Which of the following regular expressions would work for your code?

- [ ] `/[0-9]{2,}:[0-9]{2,}:[0-9]{2,}/`
- [x] `/\d\d:\d\d:\d\d/`
- [ ] `/[0-9]+:[0-9]+:[0-9]+/`
- [ ] `/ : : /`

NOTE: The first three are all partially correct and will match digits, but the **second option is the most correct** because it will **only** match **2 digit** time values (12:00:32). The first option would have worked if the repetitions range looked like `[0-9]{2}`, however because of the **comma** `[0-9]{2,}` it will select 2 **or more** digits (120:000:321). The third option will any range of time digits, single _and_ multiple (meaning `1:2:3` will also match).

**More resources:**

1. [Repeating characters](https://regexone.com/lesson/repeating_characters)
2. [Kleene operators](https://regexone.com/lesson/kleene_operators)

#### Q13. What is the result in the console of running this code?

```js
'use strict';
function logThis() {
  this.desc = 'logger';
  console.log(this);
}
new logThis();
```

- [ ] `undefined`
- [ ] `window`
- [x] `{desc: "logger"}`
- [ ] `function`

[Reference javascript classes](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Classes)

#### Q14. How would you reference the text 'avenue' in the code shown?

```js
let roadTypes = ['street', 'road', 'avenue', 'circle'];
```

- [ ] roadTypes.2
- [ ] roadTypes\[3\]
- [ ] roadTypes.3
- [x] roadTypes\[2\]

[Reference accessing javascript arrays](https://www.w3schools.com/js/js_arrays.asp)

#### Q15. What is the result of running this statement?

```javascript
console.log(typeof 42);
```

- [ ] `'float'`
- [ ] `'value'`
- [x] `'number'`
- [ ] `'integer'`

[Reference javascript data types](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Data_structures)

#### Q16. Which property references the DOM object that dispatched an event?

- [ ] `self`
- [ ] `object`
- [x] `target`
- [ ] `source`

[Reference DOM events](https://www.w3schools.com/jsref/dom_obj_event.asp)

#### Q17. You're adding error handling to the code shown. Which code would you include within the if statement to specify an error message?

```js
function addNumbers(x, y) {
  if (isNaN(x) || isNaN(y)) {
  }
}
```

- [ ] `exception('One or both parameters are not numbers')`
- [ ] `catch('One or both parameters are not numbers')`
- [ ] `error('One or both parameters are not numbers')`
- [x] `throw('One or both parameters are not numbers')`

[Reference javascript throw](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Statements/throw)

#### Q18. Which method converts JSON data to a JavaScript object?

- [ ] `JSON.fromString();`
- [x] `JSON.parse()`
- [ ] `JSON.toObject()`
- [ ] `JSON.stringify()`

[Reference convert json to javascript object](https://www.w3schools.com/js/js_json_parse.asp)

#### Q19. When would you use a conditional statement?

- [ ] When you want to reuse a set of statements multiple times.
- [x] When you want your code to choose between multiple options.
- [ ] When you want to group data together.
- [ ] When you want to loop through a group of statement.

[Reference javascript conditionals](https://www.javascript.com/learn/conditionals)

#### Q20. What would be the result in the console of running this code?

```js
for (var i = 0; i < 5; i++) {
  console.log(i);
}
```

- [ ] 1 2 3 4 5
- [ ] 1 2 3 4
- [x] 0 1 2 3 4
- [ ] 0 1 2 3 4 5

[Reference javascript for loops](https://www.w3schools.com/js/js_loop_for.asp)

#### Q21. Which Object method returns an iterable that can be used to iterate over the properties of an object?

- [ ] `Object.get()`
- [ ] `Object.loop()`
- [ ] `Object.each()`
- [x] `Object.keys()`

[Reference javascript object static methods](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Object#static_methods)

#### Q22. What will be logged to the console?

```js
var a = ['dog', 'cat', 'hen'];
a[100] = 'fox';
console.log(a.length);
```

- [x] 101
- [ ] 3
- [ ] 4
- [ ] 100

#### Q23. What is one difference between collections created with Map and collections created with Object?

- [ ] You can iterate over values in a Map in their insertion order.
- [x] You can count the records in a Map with a single method call.
- [ ] Keys in Maps can be strings.
- [ ] You can access values in a Map without iterating over the whole collection.

**Explanation:** `Map.prototype.size returns the number of elements in a Map, whereas Object does not have a built-in method to return its size.`
[Reference map methods javascript](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Map)

#### Q24. What is the value of dessert.type after executing this code?

```js
const dessert = { type: 'pie' };
dessert.type = 'pudding';
```

- [ ] pie
- [ ] The code will throw an error.
- [x] pudding
- [ ] undefined

[Reference working with js objects](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide/Working_with_Objects)

#### Q25. 0 && hi

- [ ] ReferenceError
- [ ] True
- [x] 0
- [ ] false

[Reference boolean logic](https://ntgard.medium.com/https-medium-com-ntgard-boolean-logic-in-javascript-part-1-3371af974f19)

#### Q26. Which of the following operators can be used to do a short-circuit evaluation?

- [ ] `\++`
- [ ] `\--`
- [ ] `\==`
- [x] `\|\|`

[Reference short circuit javascript](https://codeburst.io/javascript-what-is-short-circuit-evaluation-ff22b2f5608c)

#### Q27. Which statement sets the Person constructor as the parent of the Student constructor in the prototype chain?

- [ ] `Student.parent = Person;`
- [x] `Student.prototype = new Person();`
- [ ] `Student.prototype = Person;`
- [ ] `Student.prototype = Person();`

[Reference prototype object js](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Inheritance_and_the_prototype_chain)

#### Q28. Why would you include a "use strict" statement in a JavaScript file?

- [ ] to tell parsers to interpret your JavaScript syntax loosely
- [x] to tell parsers to enforce all JavaScript syntax rules when processing your code
- [ ] to instruct the browser to automatically fix any errors it finds in the code
- [ ] to enable ES6 features in your code

[Reference what is use strict in js](https://www.w3schools.com/js/js_strict.asp)

#### Q29. Which Variable-defining keyword allows its variable to be accessed (as undefined) before the line that defines it?

- [ ] all of them
- [ ] `const`
- [x] `var`
- [ ] `let`

[Reference var vs let vs const in js](https://www.freecodecamp.org/news/var-let-and-const-whats-the-difference/)

#### Q30. Which of the following values is not a Boolean false?

- [ ] `Boolean(0)`
- [ ] `Boolean("")`
- [ ] `Boolean(NaN)`
- [x] `Boolean("false")`

[Reference boolean of a string](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Boolean)

#### Q31. Which of the following is not a keyword in JavaScript?

- [ ] `this`
- [ ] `catch`
- [ ] `function`
- [x] `array`

[Reference js reserved words](https://www.w3schools.com/js/js_reserved.asp)

#### Q32. Which variable is an implicit parameter for every function in JavaScript?

- [x] Arguments
- [ ] args
- [ ] argsArray
- [ ] argumentsList

[Reference implicit js parameters for functions](https://www.codeproject.com/Tips/1221966/JavaScript-Functions-Implicit-Parameters)

#### Q33. For the following class, how do you get the value of 42 from an instance of X?

```js
class X {
  get Y() {
    return 42;
  }
}
var x = new X();
```

- [ ] `x.get('Y')`
- [x] `x.Y`
- [ ] `x.Y()`
- [ ] `x.get().Y`

[Reference getters](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Functions/get)

#### Q34. What is the result of running this code?

```js
sum(10, 20);
diff(10, 20);
function sum(x, y) {
  return x + y;
}

let diff = function (x, y) {
  return x - y;
};
```

- [ ] 30, ReferenceError, 30, -10
- [x] 30, ReferenceError
- [ ] 30, -10
- [ ] ReferenceError, -10

[Reference accessing before initialization](https://stackoverflow.com/questions/56318460/cannot-access-variable-name-before-initialization)

#### Q35. Why is it usually better to work with Objects instead of Arrays to store a collection of records?

- [ ] Objects are more efficient in terms of storage.
- [ ] Adding a record to an object is significantly faster than pushing a record into an array.
- [x] Most operations involve looking up a record, and objects can do that better than arrays.
- [ ] Working with objects makes the code more readable.

**Explanation:** Records in an object can be retrieved using their key which can be any given value (e.g. an employee ID, a city name, etc), whereas to retrieve a record from an array we need to know its index.
[Reference efficiency of lookups](https://stackoverflow.com/questions/17295056/array-vs-object-efficiency-in-javascript)

#### Q36. Which statement is true about the "async" attribute for the HTML script tag?

- [ ] It can be used for both internal and external JavaScript code.
- [ ] It can be used only for internal JavaScript code.
- [ ] It can be used only for internal or external JavaScript code that exports a promise.
- [x] It can be used only for external JavaScript code.

[Reference async attribute for html](https://www.w3schools.com/tags/att_script_async.asp)

#### Q37. How do you import the lodash library making it top-level Api available as the "\_" variable?

- [x] `import _ from 'lodash';`
- [ ] `import 'lodash' as _;`
- [ ] `import '_' from 'lodash;`
- [ ] `import lodash as _ from 'lodash';`

[Reference how to import library in js](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Statements/import)

#### Q38. What does the following expression evaluate to?

```js
[] == [];
```

- [ ] True
- [ ] undefined
- [ ] []
- [x] False

[Reference arrays in js are objects](https://stackoverflow.com/questions/30820611/why-doesnt-equality-check-work-with-arrays)

#### Q39. What type of function can have its execution suspended and then resumed at a later point?

- [x] Generator function
- [ ] Arrow function
- [ ] Async/ Await function
- [ ] Promise function

[Reference what are generators in nodejs](https://www.guru99.com/node-js-generators-compare-callbacks.html#:~:text=Generators%20are%20function%20executions%20that,resumed%20at%20a%20later%20point.)

#### Q40. What will this code print?

```js
var v = 1;
var f1 = function () {
  console.log(v);
};

var f2 = function () {
  var v = 2;
  f1();
};

f2();
```

- [ ] 2
- [x] 1
- [ ] Nothing - this code will throw an error.
- [ ] undefined

[Reference closures in js \/ nested functions](https://javascript.info/closure)

#### Q41. Which statement is true about Functional Programming?

- [ ] Every object in the program has to be a function.
- [ ] Code is grouped with the state it modifies.
- [ ] Date fields and methods are kept in units.
- [x] Side effects are not allowed.

[Reference functional programming](https://medium.com/javascript-scene/master-the-javascript-interview-what-is-functional-programming-7f218c68b3a0)

#### Q42. Your code is producing the error: TypeError: Cannot read property 'reduce' of undefined. What does that mean?

- [x] You are calling a method named reduce on an object that's declared but has no value.
- [ ] You are calling a method named reduce on an object that does not exist.
- [ ] You are calling a method named reduce on an empty array.
- [ ] You are calling a method named reduce on an object that's has a null value.

**Explanation**: `You cannot invoke reduce on undefined object... It will throw (yourObject is not Defined...)`

#### Q43. How many prototype objects are in the chain for the following array?

`let arr = [];`

- [ ] 3
- [x] 2
- [ ] 0
- [ ] 1

[Reference array prototype](https://www.w3schools.com/jsref/jsref_prototype_array.asp)

#### Q44. Which choice is _not_ a unary operator?

- [ ] `typeof`
- [ ] `delete`
- [x] `instanceof`
- [ ] `void`

[Reference js unary operators](https://www.digitalocean.com/community/tutorials/javascript-unary-operators-simple-and-useful#:~:text=A%20unary%20operation%20is%20an,therefore%20their%20functionality%20is%20guaranteed.)

#### Q45. What type of scope does the end variable have in the code shown?

```javascript
var start = 1;
if (start === 1) {
  let end = 2;
}
```

- [ ] conditional
- [x] block
- [ ] global
- [ ] function

[Reference block vs function scope](https://josephcardillo.medium.com/the-difference-between-function-and-block-scope-in-javascript-4296b2322abe)

#### Q46. What will the value of y be in this code:

```js
const x = 6 % 2;
const y = x ? 'One' : 'Two';
```

- [ ] One
- [ ] undefined
- [ ] TRUE
- [x] Two

[Reference ternary operator js](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Operators/Conditional_Operator)

#### Q47. Which keyword is used to create an error?

- [x] `throw`
- [ ] `exception`
- [ ] `catch`
- [ ] `error`

[Reference throwing errors in js](<https://www.w3schools.com/jsref/jsref_throw.asp#:~:text=The%20throw%20statement%20throws%20(generates,to%20create%20a%20custom%20error.)>)

#### Q48. What's one difference between the async and defer attributes of the HTML script tag?

- [ ] The defer attribute can work synchronously.
- [ ] The defer attribute works only with generators.
- [ ] The defer attribute works only with promises.
- [x] The defer attribute will asynchronously load the scripts in order.

[Reference async vs defer](https://www.digitalocean.com/community/tutorials/html-defer-async#:~:text=%3E-,Async%20vs%20Defer,order%20as%20they%20are%20called.)

#### Q49. The following program has a problem. What is it?

```js
var a;
var b = (a = 3) ? true : false;
```

- [x] The condition in the ternary is using the assignment operator.
- [ ] You can't define a variable without initializing it.
- [ ] You can't use a ternary in the right-hand side of an assignment operator.
- [ ] The code is using the deprecated var keyword.

[Reference ternary operator js](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Operators/Conditional_Operator)

#### Q50. Which statement references the DOM node created by the code shown?

```html
<p class="pull">lorem ipsum</p>
```

- [ ] `Document.querySelector('class.pull')`
- [x] `document.querySelector('.pull');`
- [ ] `Document.querySelector('pull')`
- [ ] `Document.querySelector('#pull')`

[Reference query selector](https://developer.mozilla.org/en-US/docs/Web/API/Document/querySelector)

#### Q51. What value does this code return?

```js
let answer = true;
if (answer === false) {
  return 0;
} else {
  return 10;
}
```

- [x] 10
- [ ] true
- [ ] false
- [ ] 0

[Reference javascript conditionals](https://www.javascript.com/learn/conditionals)

#### Q52. What is the result in the console of running the code shown?

```js
var start = 1;
function setEnd() {
  var end = 10;
}
setEnd();
console.log(end);
```

- [ ] 10
- [ ] 0
- [x] ReferenceError
- [ ] undefined

[Reference](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Closures)

#### Q53. What will this code log in the console?

```js
function sayHello() {
  console.log('hello');
}

console.log(sayHello.prototype);
```

- [ ] undefined
- [ ] "hello"
- [x] an object with a constructor property
- [ ] an error message

[Reference prototypes](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Inheritance_and_the_prototype_chain)

#### Q54. Which collection object allows unique value to be inserted only once?

- [ ] Object
- [x] Set
- [ ] Array
- [ ] Map

[Reference javascript sets](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Set)

#### Q55. What two values will this code print?

```js
function printA() {
  console.log(answer);
  var answer = 1;
}
printA();
printA();
```

- [ ] `1` then `1`
- [ ] `1` then `undefined`
- [x] `undefined` then `undefined`
- [ ] `undefined` then `1`

[Reference](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Closures)

#### Q56. How does the `forEach()` method differ from a `for` statement?

- [ ] forEach allows you to specify your own iterator, whereas for does not.
- [ ] forEach can be used only with strings, whereas for can be used with additional data types.
- [x] forEach can be used only with an array, whereas for can be used with additional data types.
- [ ] for loops can be nested; whereas forEach loops cannot.

[Reference Differences between forEach and for loop](https://www.geeksforgeeks.org/difference-between-foreach-and-for-loop-in-javascript/)

#### Q57. Which choice is an incorrect way to define an arrow function that returns an empty object?

- [ ] => `({})`
- [x] => `{}`
- [ ] => `{ return {};}`
- [ ] => `(({}))`

[Reference arrow functions](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Functions/Arrow_functions)

#### Q58. Why might you choose to make your code asynchronous?

- [x] to start tasks that might take some time without blocking subsequent tasks from executing immediately
- [ ] to ensure that tasks further down in your code are not initiated until earlier tasks have completed
- [ ] to make your code faster
- [ ] to ensure that the call stack maintains a LIFO (Last in, First Out) structure

**EXPLANATION:** "to ensure that tasks further down in your code are not initiated until earlier tasks have completed" you use the normal (synchronous) flow where each command is executed sequentially. Asynchronous code allows you to break this sequence: start a long running function (AJAX call to an external service) and continue running the rest of the code in parallel.

#### Q59. Which expression evaluates to true?

- [ ] `[3] == [3]`
- [x] `3 == '3'`
- [ ] `3 != '3'`
- [ ] `3 === '3'`

[Reference booleans](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Boolean)

#### Q60. Which of these is a valid variable name?

- [ ] 5thItem
- [x] firstName
- [ ] grand total
- [ ] function

[Reference coding conventions](https://www.w3schools.com/js/js_conventions.asp)

#### Q61. Which method cancels event default behavior?

- [ ] `cancel()`
- [ ] `stop()`
- [x] `preventDefault()`
- [ ] `prevent()`

[Reference javascript events](https://developer.mozilla.org/en-US/docs/Web/API/Event/preventDefault)

#### Q62. Which method do you use to attach one DOM node to another?

- [ ] `attachNode()`
- [ ] `getNode()`
- [ ] `querySelector()`
- [x] `appendChild()`

[Reference Node interface](https://developer.mozilla.org/en-US/docs/Web/API/Node/appendChild)

#### Q63. Which statement is used to skip iteration of the loop?

- [ ] `break`
- [ ] `pass`
- [ ] `skip`
- [x] `continue`

[Reference break vs continue](https://www.w3schools.com/js/js_break.asp)

#### Q64. Which choice is valid example for an arrow function?

- [x] `(a,b) => c`
- [ ] `a, b => {return c;}`
- [ ] `a, b => c`
- [ ] `{ a, b } => c`

[Reference arrow functions](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Functions/Arrow_functions)

#### Q65. Which concept is defined as a template that can be used to generate different objects that share some shape and/or behavior?

- [x] class
- [ ] generator function
- [ ] map
- [ ] proxy

[Reference javascript classes](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Classes)

#### Q66. How do you add a comment to JavaScript code?

- [ ] `! This is a comment`
- [ ] `# This is a comment`
- [ ] `\\ This is a comment`
- [x] `// This is a comment`

[Reference comments in javascript](https://www.w3schools.com/js/js_comments.asp)

#### Q67. If you attempt to call a value as a function but the value is not a function, what kind of error would you get?

- [x] TypeError
- [ ] SystemError
- [ ] SyntaxError
- [ ] LogicError

[Reference javascript errors](https://developer.mozilla.org/en-US/docs/web/javascript/reference/global_objects/error)

#### Q68. Which method is called automatically when an object is initialized?

- [ ] create()
- [ ] new()
- [x] constructor()
- [ ] init()

[Reference javascript constructors](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Classes/constructor)

#### Q69. What is the result of running the statement shown?

```javascript
let a = 5;
console.log(++a);
```

- [ ] 4
- [ ] 10
- [x] 6
- [ ] 5

[Reference ++x vs x++](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Operators/Increment)

#### Q70. You've written the event listener shown below for a form button, but each time you click the button, the page reloads. Which statement would stop this from happening?

```javascript
button.addEventListener(
  'click',
  function (e) {
    button.className = 'clicked';
  },
  false,
);
```

- [ ] `e.blockReload();`
- [ ] `button.preventDefault();`
- [ ] `button.blockReload();`
- [x] `e.preventDefault();`

[Reference events in javascript](https://developer.mozilla.org/en-US/docs/Web/API/Event/preventDefault)

#### Q71. Which statement represents the starting code converted to an IIFE?

- [ ] `function() { console.log('lorem ipsum'); }()();`
- [ ] `function() { console.log('lorem ipsum'); }();`
- [x] `(function() { console.log('lorem ipsum'); })();`

[Reference what is an Immediately Invoked Function Expression](https://javascript.plainenglish.io/https-medium-com-javascript-in-plain-english-stop-feeling-iffy-about-using-an-iife-7b0292aba174)

#### Q72. Which statement selects all img elements in the DOM tree?

- [ ] `Document.querySelector('img')`
- [ ] `Document.querySelectorAll('<img>')`
- [x] `Document.querySelectorAll('img')`
- [ ] `Document.querySelector('<img>')`

[Reference query selector](https://developer.mozilla.org/en-US/docs/Web/API/Document/querySelector)

#### Q73. Why would you choose an asynchronous structure for your code?

- [ ] To use ES6 syntax
- [x] To start tasks that might take some time without blocking subsequent tasks from executing immediately
- [ ] To ensure that parsers enforce all JavaScript syntax rules when processing your code
- [ ] To ensure that tasks further down in your code aren't initiated until earlier tasks have completed

[Reference async function](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Statements/async_function)

#### Q74. What is the HTTP verb to request the contents of an existing resource?

- [ ] DELETE
- [x] GET
- [ ] PATCH
- [ ] POST

[Reference http methods](https://developer.mozilla.org/en-US/docs/Web/HTTP/Methods)

#### Q75. Which event is fired on a text field within a form when a user tabs to it, or clicks or touches it?

- [x] focus
- [ ] blur
- [ ] hover
- [ ] enter

[Reference javascript events](https://developer.mozilla.org/en-US/docs/Web/Events)

#### Q76. What is the result in the console of running this code?

```javascript
function logThis() {
  console.log(this);
}
logThis();
```

- [ ] function
- [ ] undefined
- [ ] Function.prototype
- [x] window

[Reference what is the javascript window](https://www.w3schools.com/js/js_window.asp)

#### Q77. Which class-based component is equivalent to this function component?

```javascript
const Greeting = ({ name }) => <h1>Hello {name}!</h1>;
```

- [x] `class Greeting extends React.Component { render() { return <h1>Hello {this.props.name}!</h1>; } }`
- [ ] `class Greeting extends React.Component { constructor() { return <h1>Hello {this.props.name}!</h1>; } }`
- [ ] `class Greeting extends React.Component { <h>Hello {this.props.name}!</h>; } }`
- [ ] `class Greeting extends React.Component { render({ name }) { return <h1>Hello {name}!</h1>; } }`

#### Q78. Which class-based lifecycle method would be called at the same time as this effect Hook?

```javascript
useEffect(() => {
  // do things
}, []);
```

- [ ] componentWillUnmount
- [ ] componentDidUpdate
- [ ] render
- [x] componentDidMount

[Reference react lifecycle methods](https://reactjs.org/docs/react-component.html)

#### Q79. What is the output of this code?

```javascript
var obj;
console.log(obj);
```

- [ ] `ReferenceError: obj is not defined`
- [ ] `{}`
- [x] `undefined`
- [ ] `null`

[Reference working with objects](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide/Working_with_Objects)

#### Q80. How would you use the TaxCalculator to determine the amount of tax on \$50?

```javascript
class TaxCalculator {
  static calculate(total) {
    return total * 0.05;
  }
}
```

- [ ] calculate(50);
- [ ] new TaxCalculator().calculate(\$50);
- [x] TaxCalculator.calculate(50);
- [ ] new TaxCalculator().calculate(50);

[Reference functions in javascript](https://www.w3schools.com/js/js_functions.asp)

#### Q81. What is wrong with this code?

```js
const foo = {
  bar() {
    console.log('Hello, world!');
  },
  name: 'Albert',
  age: 26,
};
```

- [ ] The function bar needs to be defined as a key/value pair.
- [ ] Trailing commas are not allowed in JavaScript.
- [ ] Functions cannot be declared as properties of objects.
- [x] Nothing, there are no errors.

1. [Reference functions in javascript](https://www.w3schools.com/js/js_functions.asp)
2. [Reference working with objects](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide/Working_with_Objects)

#### Q82. What will be logged to the console?

```js
console.log('I');
setTimeout(() => {
  console.log('love');
}, 0);
console.log('Javascript!');
```

- [x]

```plaintext
I
Javascript!
love
```

- [ ]

```plaintext
love
I
Javascript!
```

- [] The output may change with each execution of code and cannot be determined.

- [ ]

```
I
love
Javascript!
```

**Reference**
https://developer.mozilla.org/en-US/docs/Web/API/setTimeout#reasons_for_delays_longer_than_specified especially see the 'late timeouts' section.

#### Q83. What will this code log to the console?

```js
const foo = [1, 2, 3];
const [n] = foo;
console.log(n);
```

- [x] 1
- [ ] undefined
- [ ] NaN
- [ ] Nothing--this is not proper JavaScript syntax and will throw an error.

[Reference array deconstruction](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Operators/Destructuring_assignment)

#### Q84. How do you remove the property name from this object?

```js
const foo = {
  name: 'Albert',
};
```

- [ ] delete name from foo;
- [x] delete foo.name;
- [ ] del foo.name;
- [ ] remove foo.name;

[Reference working with objects](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide/Working_with_Objects)

#### Q85. What is the difference between the `map()` and the `forEach()` methods on the Array prototype?

- [ ] There is no difference.
- [ ] The `forEach()` method returns a single output value, whereas the `map()` method performs operation on each value in the array.
- [x] The map() methods returns a new array with a transformation applied on each item in the original array, whereas the `forEach()` method iterates through an array with no return value.
- [ ] The `forEach()` methods returns a new array with a transformation applied on each item in the original array, whereas the `map()` method iterates through an array with no return value.

1. [Reference map](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Map)
2. [Reference Differences between forEach and for loop](https://www.geeksforgeeks.org/difference-between-foreach-and-for-loop-in-javascript/)

#### Q86. Which concept does this code illustrate?

```js
function makeAdder(x) {
  return function (y) {
    return x + y;
  };
}

var addFive = makeAdder(5);
console.log(addFive(3));
```

- [ ] overloading
- [ ] closure
- [x] currying
- [ ] overriding

[Reference currying](https://javascript.info/currying-partials)

#### Q87. Which tag pair is used in HTML to embed JavaScript?

- [x] `<script></script>`
- [ ] `<js></js>`
- [ ] `<javascript></javascript>`
- [ ] `<code></code>`

[Reference add js to html file](https://www.w3schools.com/tags/tag_script.asp)

#### Q88. If your app receives data from a third-party API, which HTTP response header must the server specify to allow exceptions to the same-origin policy?

- [ ] Security-Mode
- [x] Access-Control-Allow-Origin
- [ ] Different-Origin
- [ ] Same-Origin

[Reference Cross-Origin Resource Sharing](https://developer.mozilla.org/en-US/docs/Web/HTTP/CORS)

#### Q89. What will be logged to the console??

```js
'use strict';
function logThis() {
  this.desc = 'logger';
  console.log(this);
}
new logThis();
```

- [ ] window
- [ ] undefined
- [ ] function
- [x] {desc: "logger"}

[Reference strict in javascript classes](https://www.w3schools.com/js/js_strict.asp)

#### Q90. What will this code print?

```js
let rainForests = ['Amazon', 'Borneo', 'Cerrado', 'Congo'];
rainForests.splice(0, 2);
console.log(rainForests);
```

- [ ] `["Amazon","Borneo","Cerrado","Congo"]`
- [x] `["Cerrado", "Congo"]`
- [ ] `["Congo"]`
- [ ] `["Amazon","Borneo"]`

[Reference array methods](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array)

#### Q91. Which missing line would allow you to create five variables(one,two,three,four,five) that correspond to their numerical values (1,2,3,4,5)?

```js
const numbers = [1, 2, 3, 4, 5];
//MISSING LINE
```

- [x] `const [one,two,three,four,five]=numbers`
- [ ] `const {one,two,three,four,five}=numbers`
- [ ] `const [one,two,three,four,five]=[numbers]`
- [ ] `const {one,two,three,four,five}={numbers}`

[Reference array destructuring](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Operators/Destructuring_assignment)

#### Q92. What will this code print?

```js
const obj = {
  a: 1,
  b: 2,
  c: 3,
};

const obj2 = {
  ...obj,
  a: 0,
};

console.log(obj2.a, obj2.b);
```

- [ ] Nothing, it will throw an error
- [x] 0 2
- [ ] undefined 2
- [ ] undefined 2

[Reference spread syntax es6](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Operators/Spread_syntax)

#### Q93. Which line could you add to this code to print "jaguar" to the console?

```js
let animals = ['jaguar', 'eagle'];
//Missing Line
console.log(animals.pop()); //Prints jaguar
```

- [ ] `animals.filter(e => e === "jaguar");`
- [ ] `animals.reverse();`
- [ ] `animals.shift();`
- [x] `animals.pop();`

[Reference Javascript Array Reverse](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array/reverse)

#### Q94. What line is missing from this code?

```js
//Missing Line
for (var i = 0; i < vowels.length; i++) {
  console.log(vowels[i]);
  //Each letter printed on a separate line as follows;
  //a
  //e
  //i
  //o
  //u
}
```

- [ ] `let vowels = "aeiou".toArray();`
- [ ] `let vowels = Array.of("aeiou");`
- [ ] `let vowels = {"a", "e", "i", "o", "u"};`
- [x] `let vowels = "aeiou";`

[Reference working with arrays](https://www.w3schools.com/js/js_arrays.asp)

#### Q95. What will be logged to the console?

```js
const x = 6 % 2;
const y = x ? 'One' : 'Two';
console.log(y);
```

- [ ] undefined
- [ ] One
- [ ] true
- [x] Two

[Reference ternary operator js](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Operators/Conditional_Operator)

#### Q96. How would you access the word It from this multidimensional array?

`let matrix = [["You","Can"],["Do","It"],["!","!","!"]];`

- [ ] `matrix[1[2]]`
- [x] `matrix[1][1]`
- [ ] `matrix[1,2]`
- [ ] `matrix[1][2]`

#### Q97. What does this code do?

```js
const animals = ['Rabbit', 'Dog', 'Cat'];
animals.unshift('Lizard');
```

- [x] It adds "Lizard" to the start of the animals array.
- [ ] It adds "Lizard" to the end of the animals array.
- [ ] It replaces "Rabbit" with "Lizard" in the animals array.
- [ ] It replaces "Cat" with "Lizard" in the animals array.

[Reference working with arrays](https://www.w3schools.com/js/js_arrays.asp)

#### Q98. What is the output of this code?

```js
let x = 6 + 3 + '3';
console.log(x);
```

- [x] 93
- [ ] 12
- [ ] 66
- [ ] 633

[Reference type coercion](https://www.freecodecamp.org/news/js-type-coercion-explained-27ba3d9a2839/)

#### Q99. Which statement can take a single expression as input and then look through a number of choices until one that matches that value is found?

- [ ] else
- [ ] when
- [ ] if
- [x] switch

[Reference switch](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Statements/switch)

#### Q100. Which statement prints "roar" to the console?

```js
var sound = 'grunt';
var bear = { sound: 'roar' };
function roar() {
  console.log(this.sound);
}
```

- [ ] `bear.bind(roar);`
- [ ] `roar.bind(bear);`
- [x] `roar.apply(bear);`
- [ ] `bear[roar]();`

1. [Reference Apply](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Function/apply)
2. [Reference this](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Operators/this)
3. [Reference bind](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_objects/Function/bind)

#### Q101. Which choice is a valid example of an arrow function, assuming c is defined in the outer scope?

- [ ] `a, b => { return c; }`
- [ ] `a, b => c`
- [ ] `{ a, b } => c`
- [x] `(a,b) => c`

[Reference arrow functions](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Functions/Arrow_functions)

#### Q102. Which statement correctly imports this code from some-file.js?

```js
//some-file.js
export const printMe = (str) => console.log(str);
```

- [ ] `import printMe from './some-file';`
- [x] `import { printMe } from './some-file';`
- [ ] `import default as printMe from './some-file';`
- [ ] `const printMe = import './some-file';`

[Reference importing libraries in javascript](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Statements/import)

#### Q103. What will be the output of this code?

```js
const arr1 = [2, 4, 6];
const arr2 = [3, 5, 7];

console.log([...arr1, ...arr2]);
```

- [ ] `[2, 3, 4, 5, 6, 7]`
- [ ] `[3,5,7,2,4,6]`
- [ ] `[3, 5, 7, 2, 4, 6]`
- [ ] `[[2, 4, 6], [3, 5, 7]]`
- [x] `[2, 4, 6, 3, 5, 7]`

[Reference spread syntax](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Operators/Spread_syntax)

#### Q104. Which method call is chained to handle a successful response returned by `fetch()`?

- [ ] `done()`
- [x] `then()`
- [ ] `finally()`
- [ ] `catch()`

[Reference fetch](https://developer.mozilla.org/en-US/docs/Web/API/Fetch_API/Using_Fetch)

#### Q105. Which choice is not an array method?

- [ ] `array.slice()`
- [ ] `array.shift()`
- [ ] `array.push()`
- [x] `array.replace()`

[Reference working with arrays](https://www.w3schools.com/js/js_arrays.asp)

#### Q106. Which JavaScript loop ensures that at least a singular iteration will happen?

- [x] do…while
- [ ] forEach
- [ ] while
- [ ] for

[Reference loops in js](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Statements/do...while)

#### Q107. What will be logged to the console?

```javascript
console.log(typeof 'blueberry');
```

- [x] `string`
- [ ] `array`
- [ ] `Boolean`
- [ ] `object`

[Reference what is typeof](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Operators/typeof)

#### Q108. What is the output that is printed when the div containing the text "Click Here" is clicked?

```html
//HTML Markup
<div id="A">
  <div id="B">
    <div id="C">Click Here</div>
  </div>
</div>
```

```javascript
//JavaScript
document.querySelectorAll('div').forEach((e) => {
  e.onclick = (e) => console.log(e.currentTarget.id);
});
```

- [x] C B A
- [ ] A
- [ ] C
- [ ] A B C

1. [Reference query selector](https://developer.mozilla.org/en-US/docs/Web/API/Document/querySelector)
2. [Reference events](https://developer.mozilla.org/en-US/docs/Web/Events)

#### Q109. What will this code log to the console?

```js
const myNumbers = [1, 2, 3, 4, 5, 6, 7];
const myFunction = (arr) => {
  return arr.map((x) => x + 3).filter((x) => x < 7);
};
console.log(myFunction(myNumbers));
```

- [ ] [4,5,6,7,8,9,10]
- [ ] [4,5,6,7]
- [ ] [1,2,3,4,5,6]
- [x] [4,5,6]

[Reference functions in javascript](https://www.w3schools.com/js/js_functions.asp)

#### Q110. What does this code print to the console?

```js
let rainForestAcres = 10;
let animals = 0;

while (rainForestAcres < 13 || animals <= 2) {
  rainForestAcres++;
  animals += 2;
}

console.log(animals);
```

- [ ] 2
- [ ] 4
- [x] 6
- [ ] 8

[Reference MDN JavaScript Looping code](https://developer.mozilla.org/en-US/docs/Learn/JavaScript/Building_blocks/Looping_code)

#### Q111. Which snippet could you add to this code to print "YOU GOT THIS" to the console?

```js
let cipherText = [...'YZOGUT QGMORTZ MTRHTILS'];
let plainText = '';

/* Missing Snippet */

console.log(plainText); //Prints YOU GOT THIS
```

- [ ]

```js
for (let key of cipherText.keys()) {
  plainText += key % 2 === 0 ? key : ' ';
}
```

- [ ]

```js
for (let [index, value] of cipherText.entries()) {
  plainText += index % 2 !== 0 ? value : '';
}
```

- [x]

```js
for (let [index, value] of cipherText.entries()) {
  plainText += index % 2 === 0 ? value : '';
}
```

- [ ]

```js
for (let value of cipherText) {
  plainText += value;
}
```

1. [Reference MDN JavaScript Destructuring](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Operators/Destructuring_assignment)
2. [Reference MDN JavaScript Array entries](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array/entries)
3. [Reference MDN JavaScript Remainder/Modulo](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Operators/Remainder)

#### Q112. Which Pokemon will be logged to the console?

```js
var pokedex = ['Snorlax', 'Jigglypuff', 'Charmander', 'Squirtle'];
pokedex.pop();
console.log(pokedex.pop());
```

- [x] Charmander
- [ ] Jigglypuff
- [ ] Snorlax
- [ ] Squirtle

**Explanation**: The pop() method removes the last element from an array and returns that element. This method changes the length of the array.

[Reference Array.pop](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array/pop)

#### Q113. Which statement can be used to select the element from the DOM containing the text "The LinkedIn Learning library has great JavaScript courses" from this markup?

```html
<h1 class="content">LinkedIn Learning</h1>
<div class="content">
  <span class="content">The LinkedIn Learning library has great JavaScript courses!</span>
</div>
```

- [ ] document.querySelector("div.content")
- [x] document.querySelector("span.content")
- [ ] document.querySelector(".content")
- [ ] document.querySelector("div.span")

#### Q114. Which value is not falsey?

- [x] `[]`
- [ ] `undefined`
- [ ] `0`
- [ ] `null`

[Reference Falsy](https://developer.mozilla.org/en-US/docs/Glossary/Falsy)

#### Q115. What line of code causes this code segment to throw an error?

```js
const lion = 1;
let tiger = 2;
var bear;

++lion;
bear += lion + tiger;
tiger++;
```

- [x] `line 5, because lion cannot be reassigned a value`
- [ ] `line 6, because the += operator cannot be used with the undefined variable bear`
- [ ] `line 5, because the prefix (++) operator does not exist in JavaScript`
- [ ] `line 3, because the variable bear is left undefined`

1. [Reference const in js](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Statements/const)
2. [Reference TypeError: invalid assignment to const "x"](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Errors/Invalid_const_assignment)

#### Q116. What will be the value of `result` after running this code?

```js
const person = { name: 'Dave', age: 40, hairColor: 'blue' };
const result = Object.keys(person).map((x) => x.toUpperCase());
```

- [ ] It will throw a TypeError.
- [ ] `["Name", "Age", "HairColor"]`
- [ ] `["DAVE", 40, "BLUE"]`
- [x] `["NAME", "AGE", "HAIRCOLOR"]`

1. [Reference Object.keys()](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Object/keys)
2. [Reference Array.prototype.map()](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array/map)
3. [Reference String.prototype.toUpperCase()](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String/toUpperCase)

#### Q117. Which snippet could you insert to this code to print "swim" to the console?

```js
let animals = ["eagle", "osprey", "salmon"];
let key = animal => animal === "salmon";

if(/* Insert Snippet Here */){
  console.log("swim");
}
```

- [ ] `animals.every(key)`
- [ ] `animals.some(key).length === 1`
- [ ] `animals.filter(key) === true`
- [x] `animals.some(key)`

[Reference Array.prototype.some](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array/some)

#### Q118. What is the output of this code?

```js
class RainForest {
  static minimumRainFall = 60;
}

let congo = new RainForest();
RainForest.minimumRainFall = 80;
console.log(congo.minimumRainFall);
```

- [x] `undefined`
- [ ] `None of these answers, as static is not a feature in Javascript.`
- [ ] `60`
- [ ] `80`

[Reference Classes static](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Classes/static)

#### Q119. How can you attempt to access the property `a.b` on `obj` without throwing an error if a is undefined?

```js
let obj = {};
```

- [ ] `obj?.a.b`
- [x] `obj.a?.b`
- [ ] `obj[a][b]`
- [ ] `obj.?a.?b`

[Reference Optional chaining (?.)](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Operators/Optional_chaining)

#### Q120. What happens when you run this code?

```js
if (true) {
  var x = 5;
  const y = 6;
  let z = 7;
}
console.log(x + y + z);
```

- [ ] It will throw a `ReferenceError` about `x`.
- [ ] It will print `18`.
- [ ] It will print `undefined`.
- [x] It will throw a `ReferenceError` about `y`.

[Reference let statement](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Statements/let)

#### Q121. What does this code print to the console?

```js
const x = [1, 2];
const y = [5, 7];
const z = [...x, ...y];
console.log(z);
```

- [x] `[1,2,5,7]`
- [ ] `[[1, 2], [5, 7]]`
- [ ] `[2,7]`
- [ ] `[2,1,7,5]`

[Reference spread syntax (...)](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Operators/Spread_syntax)

#### Q122. Given this code, which statement will evaluate to false?

```js
const a = { x: 1 };
const b = { x: 1 };
```

- [ ] `a['x'] === b['x']`
- [ ] `a != b`
- [x] `a === b`
- [ ] `a.x === b.x`

[Reference](http://adripofjavascript.com/blog/drips/object-equality-in-javascript.html)

#### Q123. What will this code log to the console?

```js
console.log(typeof 41.1);
```

- [ ] `Nothing. It resuults in a ReferenceError.`
- [ ] `decimal`
- [ ] `float`
- [x] `number`

[Reference](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Operators/typeof#basic_usage)

#### Q124. What is the output of this code?

```js
let scores = [];
scores.push(1, 2);
scores.pop();
scores.push(3, 4);
scores.pop();
score = scores.reduce((a, b) => a + b);
console.log(score);
```

- [ ] `3`
- [x] `4`
- [ ] `6`
- [ ] `7`

1. [Reference](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array/push)
2. [Reference](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array/pop)
3. [Reference](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array/Reduce)

#### Q125. What does this code print to the console?

```js
let bear = {
  sound: 'roar',
  roar() {
    console.log(this.sound);
  },
};

bear.sound = 'grunt';
let bearSound = bear.roar;
bearSound();
```

- [ ] `Nothing is printed to the console.`
- [ ] `grunt`
- [x] `undefined`
- [ ] `roar`

[Reference](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide/Working_with_Objects)

#### Q126. What is the output of this code?

```js
var cat = { name: 'Athena' };

function swap(feline) {
  feline.name = 'Wild';
  feline = { name: 'Tabby' };
}

swap(cat);
console.log(cat.name);
```

- [ ] undefined
- [x] Wild
- [ ] Tabby
- [ ] Athena

#### Q127. What will this code output to the log?

```js
var thing;
let func = (str = 'no arg') => {
  console.log(str);
};
func(thing);
func(null);
```

- [ ] null no arg
- [ ] no arg no arg
- [ ] null null
- [x] no arg null

#### Q128. What will this code print to the console?

```js
const myFunc = () => {
  const a = 2;
  return () => console.log('a is ' + a);
};
const a = 1;
const test = myFunc();
test();
```

- [ ] a is 1
- [ ] a is undefined
- [ ] It won't print anything.
- [x] a is 2

#### Q129. What will this code print to the console?

```js
const myFunc = (num1, num2 = 2, num3 = 2) => {
  return num1 + num2 + num3;
};
let values = [1, 5];
const test = myFunc(2, ...values);
console.log(test);
```

- [x] 8
- [ ] 6
- [ ] 2
- [ ] 12

#### Q130. Which code would you use to access the Irish flag?

```js
var flagsJSON =
  '{ "countries" : [' +
  '{ "country":"Ireland" , "flag":"🇮🇪" },' +
  '{ "country":"Serbia" , "flag":"🇷🇸" },' +
  '{ "country":"Peru" , "flag":"🇵🇪" } ]}';

var flagDatabase = JSON.parse(flagsJSON);
```

- [ ] flagDatabase.countries[1].flag
- [x] flagDatabase.countries[0].flag
- [ ] flagDatabase[1].flag
- [ ] flagsJSON.countries[0].flag
## jQuery

#### Q1. What is the difference between these two snippets?

```js
$('button').on('click', function () {
  alert('you clicked the button!');
});
$('button').click(function () {
  alert('you clicked the button!');
});
```

- [ ] Only the second one will work; jQuery does not have a function called `.on`.
- [ ] The second snippet will not function.
- [x] Nothing `.click(function)` is shorter way to write `.on('click', function)`.
- [ ] The first snippet will execute for every button on the page, the second will only apply to the first button.

#### Q2. What does the following line of code do?

`jQuery('p')`

- [ ] Loads a paragraph tag from a remote server using AJAX
- [ ] Aliases jQuery to a variable p
- [x] Selects all paragraphs on the page
- [ ] Creates a new paragraph tag and inserts it into the body tag

#### Q3. Given the following HTML, how could we use one line to hide or show the button?

```html
<button class="btn btn-primary" type="submit">Continue to checkout</button>
```

- [x] `$('.btn-primary').toggle();`
- [ ] `$('.btn-primary').showHide();`
- [ ] `$('.btn-primary').not(':visible').show();`
- [ ] `$('.btn-primary').css({ display: 'block'});`

#### Q4. Working with AJAX, we may run into situations where a piece of code should not be run until after multiple AJAX calls have completed successfully. Say we need to call two external services for JSON data (a list of students, and a list of classes). And only after retrieving those data will we perform some manipulations on a page. What is the preferred way for dealing with this scenario?

`https://example.com/json-api/students`  
`https://example.com/json-api/classes`

- [ ] A

```js
$.get(
  ['https://example.com/json-api/students', 'https://example.com/json-api/classes'],
  function (studentRequest, classRequest) {
    // the rest of the code goes here
  },
);
```

- [ ] B

```js
$.when(
  $.get('https://example.com/json-api/students'),
  $.get('https://example.com/json-api/classes'),
).done(function (studentRequest, classRequest) {
  // the rest of the code goes here
});
```

- [ ] C

```js
$.bind(
  $.get('https://example.com/json-api/students'),
  $.get('https://example.com/json-api/classes'),
).done(function (studentRequest, classRequest) {
  // the rest of the code goes here
});
```

- [x] D

```js
$.ajax('https://example.com/json-api/students', {
  success: function (studentRequest) {
    $.ajax('https://example.com/json-api/classes', {
      success: function (classRequest) {
        // the rest of the code goes here
      },
    });
  },
});
```

#### Q5. Given the snippet of HTML below, what is the difference between the two lines that follow it?

```html
<ul>
  <li>Item 1</li>
  <li>Item 2</li>
  <li>Item 3</li>
  <li>Item 4</li>
</ul>
```

```js
$('ul').find('li').get(2);
$('ul').find('li').eq(2);
```

- [x] .get() retrieves a DOM element, and can't be chained, eq() retrieves a jQuery object, and can be chained.
- [ ] .get() retrieves a jQuery object, and can't be chained, eq() retrieves a DOM element, and can be chained.
- [ ] .get() retrieves a jQuery object, and is zero-indexed, eq() retrieves a DOM element, and is 1-indexed.
- [ ] .get() retrieves a DOM element, and is zero-indexed, eq() retrieves a jQuery object, and is 1-indexed.

#### Q6. Suppose we want to have a ball created from an HTML element (id=ball) move down and to the right from its original location when clicked, and move back into its original place when finished. Given a starting point of this, which of these snippets would accomplish that goal?

```js
$('#ball').click(function () {
  // Our code goes here
});
```

- [x] A

```js
$(this).animate(
  { top: '+=100', left: '+=100' },
  {
    duration: 600,
    complete: function () {
      $(this).animate({ top: '-=100', left: '-=100' }, 600);
    },
  },
);
```

- [ ] B

```js
$(this).animate({ top: '-=100', left: '-=100' }, 600, function () {
  $(this).animate({ top: '+=100', left: '+=100' }, 600);
});
```

- [ ] C

```js
$(this).animate(
  { top: '=100', left: '=100' },
  {
    duration: 600,
    complete: function () {
      $(this).animate({ top: 0, left: 0 }, 600);
    },
  },
);
```

- [ ] D

```js
$(this).animate({ top: '100', left: '100' }, 600, function () {
  $(this).animate({ top: 0, left: 0 }, 600);
});
```

#### Q7. Given the following CSS and HTML codes below, how could you apply the success class to the feedback div?

```css
.success {
  color: green;
  background: #ddffdd;
}
```

```html
<div class="feedback">Thank you for answering this survey.</div>
```

- [ ] `$('.feedback').hasClass('.success');`
- [ ] `$.css('.feedback', '.success')`;
- [x] `$('.feedback').addClass('success');`
- [ ] `$('.feedback').css('.success');`

#### Q8. The following page snippet includes a couple of messages in a list, and a code snippet that retrieves a few hundred messages from an API endpoint using AJAX. How can you add these new items to the .message-area--list element in the most performant way?

```html
<div class="message-area">
  <ul class="message-area--list">
    <li>Existing message 1</li>
    <li>Existing message 2</li>
  </ul>
</div>

$.get('//example.com/api/v1/message').done(function (data) { var tonsOfItems = data.messages; // add
all these messages to a large page });
```

- [ ] A

```js
tonsOfItems.map(function (item) {
  $('.message-area--list').append('<li>' + item + '</li>');
});
```

- [x] B

```js
var tonsOfListItems = tonsOfItems.map(function (item) {
  return '<li>' + item + '</li>';
});
$('.message-area--list').append(tonsOfListItems.join(''));
```

- [ ] C

```js
CSS.$messageList = $('.message-area--list');
$.each(tonsOfItems, function (idx, item) {
  $('<li>' + item + '</li>').appendTo($messageList);
});
```

- [ ] D

```js
$.each(tonsOfItems, function (idx, item) {
  $('.message-area--list').append('<li>' + item + '</li>');
});
```

#### Q9. What is jQuery?

- [ ] jQuery is a bridge between Java and Javascript that makes native apps easier to write.
- [ ] jQuery is a plugin for JavaScript that makes database queries easier to write.
- [x] jQuery is a collection of JavaScript functions that makes finding and manipulating elements on a page, AJAX, and other things easier.
- [ ] jQuery is a Chrome extension that allows users to create their own extensions with just a few lines of JavaScript.

#### Q10. We want to create a new jQuery plugin called linkUpdater that can be chained onto other jQuery selector like a normal plugin. It should update all the links in the referenced collection so they open in new windows or tabs. Below is the first cut. What is one problem with this plugin?

```js
'user strict';
($.linkUpdater = function () {
  this.find('a').attr('target', '_blank');
})(jQuery);
```

- [ ] this needs to be wrapped, like `$(this)`, in order to be chained in a plugin.
- [ ] jQuery plugins can't be safely authored in strict mode.
- [ ] In order to be used by other code, plugins need to be added to the global namespace, not wrapped in a function expression.
- [x] Our plugin should extend jQuery.fn, not jQuery itself.

#### Q11. Generally speaking, when used on a web page, how should jQuery be installed, and why?

- [x] Just before the closing body tag, because we want to avoid blocking other resources from loading, and we use the ready method to make sure our code fires after the DOM is ready
- [ ] Using the highest version number possible because only jQuery 3 and up are compatible with Internet Explorer 7
- [ ] In the head tag because we want jQuery available as soon as possible
- [ ] From a CDN because we want to be able to use jQuery online or offline

#### Q12. Given the following HTML, how could we make this button disappear from the page using jQuery?

```html
<button class="btn btn-primary" type="submit">Continue to checkout</button>
```

- [x] `$('.btn-primary').hide();`
- [ ] `$('.btn-primary:visible').not();`
- [ ] `$('.btn-primary').visibility(false);`
- [ ] `$('.btn-primary').show(false);`

#### Q13. What is the difference between `$('header').html()` and `$('header').text()`?

- [x] `$('header').html()` returns the inner HTML of the header. `$('header').text()` returns only the text
- [ ] `$('header').html()` returns only the HTML tags used, without the text. `$('header').text()` returns only the text
- [ ] `$('header').html()` strips all HTML from the header. `$('header').text()` always returns an empty string.
- [ ] `$('header').html()` returns all headers in an HTML document. `$('header').text()` the first line of a text file.

#### Q14. When writing jQuery plugins, we often provide default options that may be overridden by the end user. What jQuery function is most useful for this purpose?

- [x] \$.extend
- [ ] \$.clone
- [ ] \$.fn.extend
- [ ] \$.merge

#### Q15. There are times when you might want to programmatically trigger an event, instead of simply reacting to user input directly. Given this markup, Which choice will NOT cause a click event to the select box when the button is clicked?

```html
<article>
  <div>Here's a button you can click: <button class="btn">Click Me</button></div>
  <form>
    <p>Further down the page, there's a select box.</p>
    <select>
      <option value="1">One</option>
      <option value="2">One</option>
      <option value="3">One</option>
      <option value="4">One</option>
    </select>
  </form>
</article>
```

- [x] `$('button').on('click.myApp', (function() { $('input[type=select]').trigger('click'); });`
- [ ] `$('button').on('click', (function() { $('input[type=select]').click()); });`
- [ ] `$('button').trigger(function() { $('input[type=select]').click(); });`
- [ ] `$('button').click(function() { $('input[type=select]').click(); });`

#### Q16. You have an absolutely positioned element inside a relatively positioned parent element, and you want to animate that element within its parent element. What jQuery function is most useful for finding the initial coordinates of the `.animate-me`?

```html
<style>
  .parent {
    position: relative;
    top: 3em;
    width: 50%;
    min-height: 50vh;
    margin: 0 auto;
  }

  .animate-me {
    position: absolute;
    top: 40px;
    right: 30px;
  }
</style>

<div class="parent">
  <div class="animate-me">This box will move!</div>
</div>
```

- [x] `$('.animate-me').offset();`
- [ ] `$('.animate-me').each();`
- [ ] `$('.animate-me').position();`
- [ ] `$('.animate-me').offsetParent();`

#### Q17. You want to work with AJAX using a Promise-like interface instead of nested callback functions. What jQuery API should you use?

- [ ] `jQuery.sub`
- [ ] `jQuery.ajaxTransport`
- [x] `jQuery.Deferred`
- [ ] `jQuery.proxy`

#### Q18. What is tricky about jQuery's nth- filters (:nth-child, :nth-of-type, etc.) relative to other filters?

- [x] Referring to lists of items, they are 1-indexed (like CSS), not 0-indexed (like JavaScript).
- [ ] They don't return the jQuery object, and cannot be chained.
- [ ] They can return the wrong items if the DOM was recently manipulated.
- [ ] They are not part of CSS, so they don't get the performance benefits of passing through the `document.querySelectorAll`.

#### Q19. jQuery's AJAX functions return objects that implement the Promise API. As a result, you can chain promises and avoid nested callbacks. What does that look like?

- [x] A

```js
$.get('hhttp://httpbin.org/delay/2')
  .then(function (response) {
    // Data from first GET is here as 'response'
    return $.get('http://httpbin.org/delay/2');
  })
  .then(function (response) {
    // Data from second GET is here as 'response'
  });
```

- [ ] B

```js
$.get('hhttp://httpbin.org/delay/2')
  .catch(function (response) {
    // Data from first GET is here as 'response'
    return $.get('http://httpbin.org/delay/2');
  })
  .done(function (response) {
    // Data from second GET is here as 'response'
  });
```

- [ ] C

```js
$.get('hhttp://httpbin.org/delay/2', function (response1) {
  // Data from first GET is here as 'response1'

  $.get('http://httpbin.org/delay/2', function (response2) {
    // Data from second GET is here as 'response2'
  });
});
```

- [ ] D

```js
$.get('hhttp://httpbin.org/delay/2')
  .then(function (response) {
    // Data from first GET is here as 'response'
    return response;
  })
  .get('http://httpbin.org/delay/2', function (response) {
    // Data from second GET is here as 'response'
  });
```

#### Q20. You want to have a ball that is created from an HTML element (id=ball) move down and to the right of its original location when clicked, and move back to its original place when finished. What snippet, added to the code below, would do this?

```js
$('#ball').click(function () {
  // Our code goes here
});
```

- [ ] A

```js
$(this).animate(
  {
    top: '-=100',
    left: '-=100',
  },
  600,
  function () {
    $(this).animate(
      {
        top: '+=100',
        left: '+=100',
      },
      600,
    );
  },
);
```

- [x] B

```js
$(this).animate(
  {
    top: '+=100',
    left: '+=100',
  },
  {
    duration: 600,
    complete: function () {
      $(this).animate(
        {
          top: '-=100',
          left: '-=100',
        },
        600,
      );
    },
  },
);
```

- [ ] C

```js
$(this).animate(
  {
    top: 100,
    left: 100,
  },
  600,
  function () {
    $(this).animate(
      {
        top: 0,
        left: 0,
      },
      600,
    );
  },
);
```

- [ ] D

```js
$(this).animate(
  {
    top: 100,
    left: 100,
  },
  {
    duration: 600,
    complete: function () {
      $(this).animate(
        {
          top: 0,
          left: 0,
        },
        600,
      );
    },
  },
);
```

#### Q21. The way `.wrap()` works is sometimes misunderstood. Given the DOM and jQuery snippets below, what does the modified DOM snippet look like?

```html
<div id="container">
  <div class="item">Here's an item</div>
</div>
```

```js
$('#container').wrap('<div class="wrapper"></div>').css('border', '2px solid red');
```

- [ ] A

```html
<div class="wrapper" style="border: 2px solid red;">
  <div id="container">
    <div class="item">Here's an item</div>
  </div>
</div>
```

- [x] B

```html
<div class="wrapper">
  <div id="container" style="border: 2px solid red;">
    <div class="item">Here's an item</div>
  </div>
</div>
```

- [ ] C

```html
<div id="container" style="border: 2px solid red;">
  <div class="wrapper">
    <div class="item">Here's an item</div>
  </div>
</div>
```

- [ ] D

```html
<div id="container">
  <div class="wrapper" style="border: 2px solid red;">
    <div class="item">Here's an item</div>
  </div>
</div>
```

#### Q22. How can you select the following blockquote AND the list in a single call to jQuery() without chaining?

```html
<div class="quotes">
  <blockquote data-favorite="false">A quote</blockquote>
  <blockquote data-favorite="true">A favorite quote</blockquote>
  <blockquote data-favorite="false">A quote</blockquote>
  <blockquote data-favorite="false">A quote</blockquote>
</div>

<ul class="menu-first">
  <li>Item 1</li>
  <li>Item 2</li>
  <li>Item 3</li>
  <li>Item 4</li>
</ul>
```

- [ ] `$('.quotes + .menu-first')`
- [ ] `$('.quotes .menu-first')`
- [x] `$('.quotes, .menu-first')`
- [ ] `$('.quotes' + '.menu-first')`

#### Q23. Effects like show, hide, fadIn, and fadeOut can be called with no arguments, but can also take arguments for how long they should last. Which is NOT a duration argument supported by these functions?

- [ ] "fast"
- [x] "extreme"
- [ ] 2000
- [ ] "slow"

#### Q24. Though jQuery offers visual effects, it is considered a best practice to use CSS to set up different states triggered by classes, where it makes sense. What's the easiest way to enable and disable a class bounce on an element with the ID dialog?

- [ ] `$('#dialog').classToggle('bounce')`
- [ ] `$('#dialog.bounce').removeClass().addClass()`
- [ ] `$('#dialog').addOrRemoveClass('bounce')`
- [x] `$('#dialog').toggleClass('bounce')`

#### Q25. What is the main difference between selectors and filters?

- [ ] Selectors are used to refine the content that filters have been applied to.
- [x] Selectors are used to find and select content in a page. Filters are used to refine the results of selectors.
- [ ] Filters are used to remove content from the page. Selectors are used to add content to the page
- [ ] There is no real difference. They are both used to build up lists of page content.

#### Q26. You want to create a custom right-click menu. How might you start the code?

- [ ] `$('#canvas').on('click.right', function(){ console.log('Handled a right-click') });`
- [ ] `$('#canvas').on('contextual', function(){ console.log('Handled a right-click') });`
- [x] `$('#canvas').on('contextmenu', function(){ console.log('Handled a right-click') });`
- [ ] `$('#canvas').on('rightclick', function(){ console.log('Handled a right-click') });`

#### Q27. What is the correct way to check how many paragraphs exist on a page using jQuery?

- [ ] `$('p').count()`
- [x] `$('p').length`
- [ ] `$('*').find('p')`
- [ ] `$('p').length()`

#### Q28. As with many areas of JavaScript, keeping track of the meaning of **this** is important and sometimes tricky. What does **this** mean at each of the two points in this custom plugin snippet?

```js
$.fn.customPlugin = function () {
  // Point 1

  return this.each(function () {
    // Point 2
  });
};
$(document).customPlugin();
```

- [ ] At Point 1, `this` means a jQuery object. At Point 2, it means a DOM element.
- [ ] In this case, they mean the same thing: a jQuery object.
- [ ] In this case, they mean the same thing: a DOM element.
- [x] At Point 1, `this` means a DOM element. At Point 2, it means a jQuery object.

#### Q29. How can you make the first list item bold and the next item oblique, in a single statement chain?

```html
<ul class="menu-first">
  <li>Item 1</li>
  <li>Item 2</li>
  <li>Item 3</li>
  <li>Item 4</li>
</ul>
```

- [ ] A

```js
$('.menu-first > li').eq(0).css('font-weight', 'bold').eq(1).css('font-style', 'oblique');
```

- [ ] B

```js
$('.menu-first > li').first().css('font-weight', 'bold').after().css('font-style', 'oblique');
```

- [ ] C

```js
$('.menu-first > li').first().css('font-weight', 'bold').second().css('font-style', 'oblique');
```

- [x] D

```js
$('.menu-first > li').eq(0).css('font-weight', 'bold').next().css('font-style', 'oblique');
```

#### Q30. Which CSS selectors can you NOT use in jQuery?

- [ ] You cannot use multiple class selectors such as `.class1.class2`.
- [ ] You cannot use pseudo-classes such as `:not` or `:last-of-type`.
- [ ] You cannot use IDs and classes together, such as `#element.class`.
- [x] None. All CSS selectors are compatible in jQuery.

#### Q31. Starting with some DOM elements in the nested structure below, you assign listeners for the same event to a child element and one of the parents using the JavaScript that follows. You want to ensure that when `.leaf` is clicked, only its event handler will be fired, instead of the click bubbling up and also firing the parent's click handler. What do you need to add to its handler function?

```html
<ul class="items" id="main-menu">
  <li>
    Item 1
    <ul>
      <li class="leaf">Sub Item 1</li>
      <li>Sub Item 2</li>
    </ul>
  </li>
</ul>
```

```js
$('.leaf').click(function (event) {
  console.log('Sub Item 1 got a click');
});
$('#main-menu').click(function (event) {
  console.log('Main menu got a click');
});
```

- [ ] `event.capture();`
- [x] `event.stopPropagation();`
- [ ] `event.preventDefault();`
- [ ] `event.stop();`

#### Q32. Using event delegation, you can listen for events on a lot of different items without having to attach separate listeners to each one. But there are times when you may want to check the type of item receiving the event before doing anything, such as checking if an image was clicked versus a text field. Given the starter code below, which choice shows what jQuery provides to help with that process?

```html
<div id="sidebar">
  <img src="fancy-button.png" alt="Pick Me" />
  <input type="text" placeholder="Fill in something" />
</div>
```

```js
$('#sidebar').click(function (evt) {
  var $target = $(evt.target);

  // What goes here?
});
```

- [ ] `$($target.get(0) + ':image')`
- [ ] `$('img').is($target)`
- [ ] `$target.filter('img')`
- [x] `$target.is('img')`

#### Q33. There are many ways to create elements that can be added to the page. Which answer is NOT one of those ways, assuming you have the following on the page?

```html
<div id="elements"></div>
```

- [ ] A

```js
$('#elements').append($('<p class="appended">As an HTML string</p>'));
```

- [ ] B

```js
var p = document.createElement('p');
var text = document.createTextNode('As a DOM element');
p.appendChild(text);
$('#elements').append(p);
```

- [x] C

```js
$('#elements').append(<p class="appended">As a JSX object</p>);
```

- [ ] D

```js
$('#elements').append(
  $('<p>', {
    class: 'appended',
    text: 'As an attribute object',
  }),
);
```

#### Q34. The `.addClass()` and `.removeClass()` methods can accept functions as arguments. What does this function do?

```js
$('#menu').addClass(function () {
  return $('body').attr('class');
});
```

- [ ] It adds the first class found on the body element to the #menu element.
- [ ] It adds all classes found on the #menu element to the body tag.
- [ ] It replaces any classes on the #menu element with all classes from the body tag.
- [x] It adds all classes found on the body element to the #menu element.

#### Q35. You're working on a site that uses an old version of jQuery, and you want to update to a newer version. What's the most efficient way to do so?

- [ ] Install the newer version of jQuery, go through each script one by one, and fix what looks broken.
- [ ] Read the change notes for the newer version of jQuery, fix all scripts, install the newer version, and fix anything that remains broken.
- [x] Install the newer version of jQuery as well as its Migrate plugin, fix all warnings, and uninstall the Migrate plugin.
- [ ] Install the newer version of jQuery at the same time, and use `jQuery.noConflict()` on pages that need the older version.

#### Q36. Let's say you have a page with just one link on it. How can you change the anchor tag so it links to example.com?

- [ ] `$('a').attribute('href', 'http://www.example.com')`
- [x] `$('a').attr('href', 'http://www.example.com')`
- [ ] `$('a').data('href', 'http://www.example.com')`
- [ ] `$('a').href('http://www.example.com')`

#### Q37. What does `$()` mean in jQuery?

- [x] It is an alias to the main core method of jQuery itself—the same as writing jQuery().
- [ ] It is a utility function that selects the first element from the document.
- [ ] It is a shorter way to write `document.getElementById()`.
- [ ] It is a utility function that selects the last element from the document.

#### Q38. Along with DOM traversal and manipulation, jQuery offers several general-purpose helper functions that fill in some JavaScript gaps, especially before ES2015. Which is NOT a jQuery utility function?

- [ ] `jQuery.each`, a general purpose iterator for looping over arrays or objects
- [ ] `jQuery.isNumeric`, which can check whether its argument is, or looks like, a number
- [ ] `jQuery.extend`, which can merge objects and make complete deep copies of objects
- [x] `jQuery.isMobile`, which can tell whether the user is using a mobile browser

#### Q39. Given this set of checkboxes, how can you select the ones that have the phrase "sun" as part of the value?

```html
<input type="checkbox" name="artists[]" value="sun-ra" />
<input type="checkbox" name="artists[]" value="otis-redding" />
<input type="checkbox" name="artists[]" value="captain-beefheart" />
<input type="checkbox" name="artists[]" value="king-sunny-ade" />
<input type="checkbox" name="artists[]" value="weather-report" />
```

- [ ] `$('checkbox').val(/sun/);`
- [x] `$('input[value*="sun"]');`
- [ ] `$('input[value|="sun"]');`
- [ ] `$('input:checkbox').attr('value', '*sun*');`

#### Q40. How can you get an AJAX request to go through without triggering any of jQuery's AJAX events?

- [ ] Set the type option to "none".
- [ ] Set the processData option to false.
- [ ] Set a success callback that returns false.
- [x] Set the option "global" to false.

#### Q41. How do you change the current value of a text field with the class `.form-item` to "555-1212"?

- [ ] `$.val('.form-item', '555-1212');`
- [x] `$('.form-item').val('555-1212');`
- [ ] `$('.form-item').data('value', '555-1212');`
- [ ] `$('.form-item').set('value', '555-1212');`

#### Q42. How would you fire a callback when any AJAX request on a page has completed?

- [ ] `$('body').ajaxComplete(function() { console.count('An AJAX request completed'); });`
- [ ] `$(document).on('ajax-complete', function() { console.count('An AJAX request completed'); });`
- [ ] `$('body').on('ajaxComplete', function() { console.count('An AJAX request completed'); });`
- [x] `$(document).ajaxComplete(function() { console.count('An AJAX request completed'); });`

#### Q43. Given this set of checkboxes, how can you select the one with the value "blimp"?

```html
<input type="checkbox" name="songs[]" value="satisfaction" />
<input type="checkbox" name="songs[]" value="respect" />
<input type="checkbox" name="songs[]" value="blimp" />
<input type="checkbox" name="songs[]" value="saturn" />
<input type="checkbox" name="songs[]" value="penguins" />
```

- [x] `$('input[value="blimp"]');`
- [ ] `$('input[value!="blimp"]');`
- [ ] `$('checkbox').val('blimp');`
- [ ] `$('input:checkbox').attr('value', 'blimp');`

#### Q44. Given this snippet of HTML and jQuery code, what does the jQuery do?

```html
<ul class="menu">
  <li><a href="#" class="active">Home</a></li>
  <li><a href="#">Page 2</a></li>
</ul>
<ul class="active submenu">
  <li><a href="#">Subpage 1</a></li>
  <li><a href="#">Subpage 2</a></li>
</ul>
```

```js
var m = $('.menu'),
  sm = $('.submenu');
m.add(sm);
m.css('font-weight', 'bold');
```

- [ ] It makes all the menu items bold.
- [ ] It throws an exception on line 3.
- [x] It makes the first set of menu items, not the second, bold.
- [ ] It makes the second set of menu items, not the first, bold.

#### Q45. You want to take a block of type and animate it to a larger size with jQuery. The following HTML and JavaScript behaves strangely. What is the issue?

```html
<div id="type" style="font: 1em/1.5 helvetica, arial, sans-serif; background: #ffc; padding: 0">
  Animate me!
</div>
```

```js
$('#type').animate(
  {
    fontSize: '+=1em',
  },
  3000,
);
```

- [ ] jQuery does not support ems and will make the type 1 pixel larger instead of 1 em larger.
- [ ] jQuery cannot override CSS in a style attribute, so the font size will not change.
- [ ] The font size was set with a shorthand property, so jQuery will not animate the font size at all.
- [x] The font size was set with a shorthand property, so jQuery will start the animation from 0 instead of from 1 em.

#### Q46. When using the `clone()` function to duplicate an element, what is one of the main concerns your code needs to watch out for?

- [ ] The `clone()` function may ignore data attributes on the original elements.
- [x] The `clone()` function may result in elements with duplicate ID attributes.
- [ ] The `clone()` function may remove CSS classes from the cloned elements.
- [ ] The `clone()` function may not respect the attribute order of the original elements.

#### Q47. When incorporating a plugin into a project, what are the important steps for basic installation and usage?

- [x] The jQuery script tag must come first, followed by the plugin, followed by your custom scripts, all preferably at or near the bottom of the page.
- [ ] Your custom scripts must appear first in the document `<head>`, followed by jQuery, followed by the plugin.
- [ ] The jQuery script tag and the plugin script tag must appear in the document `<head>`, and your custom scripts can follow anywhere on the page.
- [ ] The jQuery script tag must appear in the document `<head>`, but the plugin and your custom scripts can appear anywhere else in any order.

#### Q48. These two script tags show different ways of using jQuery's `ready()` method. What is true about both approaches?

```js
<script>
  $(function() {
    // The rest of my code goes here
  });
</script>

<script>
  jQuery(document).ready(function($) {
    // The rest of my code goes here
  });
</script>
```

- [x] The code inside them can manipulate the DOM safely, knowing the browser has loaded it fully.
- [ ] The code inside them can manipulate images on the page safely, knowing they have fully downloaded to the browser.
- [ ] The code inside them will be run exactly once per user session.
- [ ] The code inside them is not aware of the DOM.

#### Q49. Which describes how jQuery makes working with the DOM faster?

- [ ] jQuery optimizes the DOM in a background thread, making updates faster.
- [ ] jQuery avoids using the DOM at all.
- [ ] jQuery uses a virtual DOM that batches updates, making inserts and deletes faster.
- [x] jQuery code to perform DOM manipulation is shorter and easier to write, but does not make DOM operations faster.

#### Q50. There are some issues with this snippet of jQuery. First, it is manipulating CSS directly, rather than manipulating classes and leaving the CSS in stylesheets. What else in this code is best to avoid?

```js
$('.item').css('background-color', 'red');
// some other code here
var firstSubItem = $('.item').find('.sub-item').get(0);
// some other code here too
$('.item').parents('.navigation').css('font-weight', 'bold');
```

- [ ] The `.css()` method accepts only an object, not two separate arguments. This will trigger an exception that should be caught.
- [ ] The `$('.item')` selection is being made several times. This should be cached in a variable for (however slightly) better performance and easier maintainability.
- [x] The call to `.parents()` is in an inefficient place.
- [ ] All the calls to `$('.item')` should be chained together as a single executable line for better performance.

#### Q51. Which choice is an example of statement chaining?

- [ ] `var $p = $('p'); console.log($p.length);`
- [x] `$('p').find('a').children('li');`
- [ ] `$('p > a > li');`
- [ ] `$('p'); $('a'); $('li');`

#### Q52. How can you ensure that some code executes only when a class `active` appears on an element?

- [ ] `$('.element').attr('class', 'active')`
- [ ] `$('.element').with('.active')`
- [x] `$('.element').hasClass('active')`
- [ ] `$('.active').then()`

#### Q53. jQuery has a main function for handling AJAX, and several shorthand function including `load()` that make calling that main function easier. Given this HTML snippet, how can you insert only the second snippet from the source.html file (`div#one`) into the `#load-me` div on-demand via AJAX?

```html
<div id="load-me">This area will be replaced with AJAX loaded content.</div>

<div id="one">
  <h1>First Piece</h1>

  <p>Lorem ipsum duis maximus quam condimentum dolor eleifend scelerisque.</p>
</div>

<div id="two">
  <h1>Second Piece</h1>

  <p>Lorem ipsum proin facilisis augue in risus interdum ornare.</p>
</div>
```

- [ ] `$('#load-me').get('source.html#one');`
- [ ] `$('#load-me').get('source.html #one');`
- [x] `$('#load-me').load('source.html #one');`
- [ ] `$('#load-me').load('source.html', '#one');`

#### Q54. Given this HTML list and subsequent two lines of jQuery, what is the difference in the behavior of `.closest()` and `.parents()`?

```html
<ul class="items" id="main-menu">
  <li>
    Item 1
    <ul id="sub-menu">
      <li class="leaf">Sub Item 1</li>
      <li>Sub Item 2</li>
    </ul>
  </li>
</ul>
```

```js
$('.leaf').closest('.items');
$('.leaf').parents('.items');
```

- [x] `.closest()` returns `.leaf` and `#main-menu`; `.parents()` returns `#main-menu` and `#sub-menu`.
- [ ] `.closest()` returns `.leaf` and `#sub-menu`; `.parents()` returns `#main-menu` and `#sub-menu`.
- [ ] `.closest()` returns only `#main-menu`; `.parents()` returns `#main-menu` and `#sub-menu`.
- [ ] `.closest()` returns only `#sub-menu`; `.parents()` returns `#main-menu` and `#sub-menu`.

#### Q55. What does this line of code do?

```js
$('ul > li:first-child');
```

- [x] selects the first list item inside all unordered lists on the page
- [ ] selects the first list item inside the first unordered list on the page
- [ ] selects the first element inside any list items on the page
- [ ] creates a predefined CSS selector that can be reused later

#### Q56. Below is a list of items that you want to be clickable and an event handler function. How can you assign the event handler to every item in the list in a way that is most performant, and also that ensures that the handler is called even if more items are added to the list programmatically?

```html
<ul class="clickable-list">
  <li>First Item</li>
  <li>Second Item</li>
  <li>Third Item</li>
  <li>Fourth Item</li>
  <li>Fifth Item</li>
</ul>
```

```js
function listResponder(evt) {
  console.log('You clicked a list item that says', evt.target.innerText);
}
```

- [ ] `$('.clickable-list').click(listResponder);`
- [x] `$('.clickable-list').on('click', 'li', listResponder);`
- [ ] `$('.clickable-list').on('click, append', listResponder);`
- [ ] `$('.clickable-list').each(function() { $(this).click(listResponder); });`

#### Q57. What is the difference between $('p').find('a') and $('p').children('a')?

- [ ] `find() traverses only one level down, whereas children() selects anything inside the original element`
- [ ] `$('p').find('a') finds all paragraphs inside links, whereas $('p').children('a') finds links within paragraph tags`
- [ ] `.find() always searches the entire DOM tree, regardless of the original selection .children() searches only the immediate childern of an element`
- [x] `children() traverses only one level down, whereas find() selects anything inside the original element`

[Source: https://api.jquery.com/find/](https://api.jquery.com/find/)

**Explanation**:`Given a jQuery object that represents a set of DOM elements, the .find() method allows us to search through the descendants of these elements in the DOM tree and construct a new jQuery object from the matching elements. The .find() and .children() methods are similar, except that the latter only travels a single level down the DOM tree.`

#### Q58. Consider the following markup, used to lay out three balls on the page, all hidden. How can you select the green ball, make it faded in over the course of three seconds, and log a console message when the animation has finished?

```html
<div class="balls">
  <div class="ball ball--red" style="display: none"></div>
  <div class="ball ball--green" style="display: none"></div>
  <div class="ball ball--blue" style="display: none"></div>
</div>
```

- [x] A

```JavaScript
$('.ball--green').fadeIn(3000, function(){
    console.log("Animation is done!");
});
```

- [ ] B

```JavaScript
$('.ball--green').fade('in',3000).done(function(){
    console.log("Animation is done!");
});
```

- [ ] C

```JavaScript
$('.ball--green').fadeIn(3).console().log("Animation is done!");
```

- [ ] D

```JavaScript
$('.ball--green').fadeIn("3s", function(){
    console.log("Animation is done!");
});
```

[Source: jQuery Docs: fadeIn](https://api.jquery.com/fadeIn/)

`Durations are given in milliseconds; higher values indicate slower animations, not faster ones. The strings 'fast' and 'slow' can be supplied to indicate durations of 200 and 600 milliseconds, respectively. If any other string is supplied, or if the duration parameter is omitted, the default duration of 400 milliseconds is used.`

#### Q59. Why might you use custom events instead of shared helper functions? For example

```JavaScript
$(document).on('myCustomEvent', function(){
    // act on my custom event
});

//and later...
$(document).trigger('myCustomEvent');
```

- [ ] `Custom events are at least an order of magnitude faster than helper functions`
- [x] `Custom events can be listened for and acted upon across one or more scripts without needing to keep helper functions in scope`
- [ ] `Handler functions for custom events are less likely to be mangled by minification and obfuscation build tools`
- [ ] `It is easier to write documentation for custom events than it is for helper functions`

[Source: learn.jquery.com](https://learn.jquery.com/events/introduction-to-custom-events/)

`Instead of focusing on the element that triggers an action, custom events put the spotlight on the element being acted upon. This brings a bevy of benefits, including: Behaviors of the target element can easily be triggered by different elements using the same code. Behaviors can be triggered across multiple, similar, target elements at once. Behaviors are more clearly associated with the target element in code, making code easier to read and maintain.`

#### Q60. In the HTML and JavaScript below, the animations will all fire at once. How can you make them fire in sequence instead?

```html
<div id="element-1" class="animel"></div>
<div id="element-2" class="animel"></div>
<div id="element-3" class="animel"></div>

$('#element-1').animate({ top: '+=100' }); $('#element-2').animate({ top: '+=100' });
$('#element-3').animate({ top: '+=100' });
```

- [ ] A

```JavaScript
$('#element-1').animate({ top: '+=100' })
    .pushStack('#element-2')
    .animate({ top: '+=100' })
    .pushStack('#element-3').animate({ top: '+=100' })
```

- [x] B

```JavaScript
$('#element-1').animate({ top: '+=100' }, function() {
    $('#element-2').animate({ top: '+=100' }, function() {
        $('#element-3').animate({ top: '+=100' });
    })
});
```

- [ ] C

```JavaScript
$('#element-1').animate({ top: '+=100' })
    .add('#element-2').animate({ top: '+=100' })
    .add('#element-3').animate({ top: '+=100' })
```

- [ ] D

```JavaScript
$('#element-1').animate({ top: '+=100' }, {queue: 'custom'});
$('#element-2').animate({ top: '+=100' }, {queue: 'custom'});
$('#element-3').animate({ top: '+=100' }, {queue: 'custom'});
$('custom').dequeue();
```

[Source: jQuery Docs: animate](https://api.jquery.com/animate/)

`the .animate() method can take in a function to call once the animation is complete, called once per matched element. Which is called the complete option for the animate method`

#### Q61. Given this checkbox, how can you determine whether a user has selected or cleared the checkbox?

`<input type="checkbox" id="same-address" checked>`

- [ ] by checking the value of `$('#same-address').val()`
- [x] by checking the value of `$('#same-address').prop('checked')`
- [ ] by checking the value of `$('#same-address').attr('checked')`
- [ ] by checking the value of `$('#same-address').checked`

#### Q62. In some projects, jQuery is not included as a file with an obvious version number (if it has been run through a minifier or other code bundler, for example). How can you detect programmatically what version of jQuery is active?

- [ ] `jQuery.version()`
- [ ] `jQuery.jquery`
- [ ] `jQuery.prototype.version`
- [x] `jQuery.fn.jquery`

#### Q63. Given this snippet of HTML, how can you get the value of the text field using jQuery?

`<input type="text" class="form-control" id="firstName" placeholder="" value="" required="">`

- [ ] `$('input[type=text]').val()`
- [ ] `$('.form-control').val()`
- [x] `all of these answers`
- [ ] `$('#firstName').val()`

`all the listed selectors will target the text field since it has a type=text, a class=form-control, and an id=firstName`

#### Q64. Which property of the jQuery event object references the DOM object that dispatched an event?

- [x] target
- [ ] self
- [ ] source
- [ ] object

[Source: jQuery Docs: event.target](https://api.jquery.com/event.target/)

`The target property can be the element that registered for the event or a descendant of it. It is often useful to compare event.target to this in order to determine if the event is being handled due to event bubbling.`

#### Q65. You want to write a plugin that creates a new traversal function—such as parent() and children()—and behaves like the ones jQuery includes out of the box. It needs to correctly modify the list of selections jQuery tracks internally, build up a list of additional items, and return the merged collection. What do you need to return on the last line of the function in order for this plugin to work correctly?

```JavaScript
$.fn.myTraverse = function() {
   // ... setup

   var additionalItems = [ /* some additional items for jQuery */ ];

   return // return what?
}
```

- [ ] `return this.append(additionalItems);`
- [ ] `return additionalItems.appendTo(this);`
- [x] `return this.pushStack(additionalItems);`
- [ ] `return this.add(additionalItems);`

[Source: jQuery Docs](https://api.jquery.com/pushStack/)

`When you call pushStack() off of the current collection, it will take the given collection and associate it to the current collection such that calling the end() method (after the plugin exits) will return the programmer to the current collection.`

[Extra Reading: bennadel.com](https://www.bennadel.com/blog/1739-using-pushstack-in-jquery-plugins-to-create-new-collections.htm)

#### Q66. Given this snippet of HTML and jQuery code, what will the result look like?

```html
<ul class="items">
  <li class="active">Item 1</li>
  <li>Item 2</li>
  <li>
    Item 3
    <ul>
      <li>Sub Item 1</li>
      <li>Sub Item 2</li>
    </ul>
  </li>
</ul>
```

`$('.items').find('.active').nextAll().addClass('after-active');`

- [x] A

```html
<ul class="items">
  <li class="active">Item 1</li>
  <li class="after-active">Item 2</li>
  <li class="after-active">
    Item 3
    <ul>
      <li>Sub Item 1</li>
      <li>Sub Item 2</li>
    </ul>
  </li>
</ul>
```

- [ ] B

```html
<ul class="items">
  <li class="active">Item 1</li>
  <li class="after-active">Item 2</li>
  <li class="after-active">
    Item 3
    <ul class="after-active">
      <li>Sub Item 1</li>
      <li>Sub Item 2</li>
    </ul>
  </li>
</ul>
```

- [ ] C

```html
<ul class="items">
  <li class="active">Item 1</li>
  <li class="after-active">Item 2</li>
  <li class="after-active">
    Item 3
    <ul>
      <li class="after-active">Sub Item 1</li>
      <li class="after-active">Sub Item 2</li>
    </ul>
  </li>
</ul>
```

- [ ] D

```html
<ul class="items">
  <li class="active">Item 1</li>
  <li class="after-active">Item 2</li>
  <li class="after-active">
    Item 3
    <ul class="after-active">
      <li class="after-active">Sub Item 1</li>
      <li class="after-active">Sub Item 2</li>
    </ul>
  </li>
</ul>
```

[Source: jQuery Docs](https://api.jquery.com/nextall/)

**.nextAll([selector]) method**
`Gets all following siblings of each element in the set of matched elements, optionally filtered by a selector.`

#### Q67. You have an element with a series of code (not CSS) animations applied to it that could be triggered by code you control, or other code elsewhere (such as plugins). How can you fire some code when all those animations have completed?

- [ ] A

```js
$('#element').on('animationend', function () {
  console.log('Finally, everything is done!');
});
```

- [ ] B

```js
$('#element')
  .on('promise')
  .then(function () {
    console.log('Finally, everything is done!');
  });
```

- [ ] C

```js
$('#element')
  .promise()
  .catch(function () {
    console.log('Finally, everything is done!');
  });
```

- [ ] D

```js
$('#element')
  .promise()
  .then(function () {
    console.log('Finally, everything is done!');
  });
```

1. [Source: HTMLElement: animationend event | MDN ](https://developer.mozilla.org/en-US/docs/Web/API/HTMLElement/animationend_event)
2. [Example: Stackoverflow](https://stackoverflow.com/questions/49580666/check-if-an-css-animation-is-completed-with-jquery-or-js)

#### Q68. HTML5 data attributes allow you to create valid custom attributes to store arbitrary data within DOM elements. jQuery has an API to interface with custom data such as the series of quotes below. How can you mark the second quote as your favorite?

```html
<div class="quotes">
  <blockquote data-favorite="false">A quote</blockquote>
  <blockquote data-favorite="false">A favorite quote</blockquote>
  <blockquote data-favorite="false">A quote</blockquote>
  <blockquote data-favorite="false">A quote</blockquote>
</div>
```

- [ ] `$('blockquote'):second().attr('favorite', true);`
- [x] `$('blockquote:nth-child(2)').data('favorite', true);`
- [ ] `$('blockquote').second().data('favorite', true);`
- [ ] `$('blockquote:nth-child(2)').attr('favorite', true);`

1. [Source: .data() | jQuery API Documentation](https://api.jquery.com/data/)
2. [Source: :nth-child() | MDN Docs](https://developer.mozilla.org/en-US/docs/Web/CSS/:nth-child)

#### Q69. jQuery can create event handlers that execute exactly once. How is this done?

- [ ] `$('button').click(function() { console.log('this will only happen once'); }, false);`
- [ ] `$('button').on('click', function() { console.log('this will only happen once'); }).off('click');`
- [ ] `$('button').once('click', function() { console.log('this will only happen once'); });`
- [x] `$('button').one('click', function() { console.log('this will only happen once'); });`

[Source: .one() | jQuery API Documentation](https://api.jquery.com/one/)

#### Q70. You want to implement the behavior of an effect like `slideDown()` manually using `animate()`. What is one critical point you need to remember?

- [ ] `slideDown()` requires animating the background color; doing so with `animate()` requires the jQuery Color plugin.
- [x] `slideDown()` includes toggling visibility automatically. `animate()` does not automatically set any properties.
- [ ] `slideDown()` requires the element to have a height set in pixels. `animate()` does not.
- [ ] Effects created with `animate()` must be run over at least 100 milliseconds, where `slideDown()` can run as quickly as 50ms.

[Source: .slideDown() | jQuery API Documentation](https://api.jquery.com/slidedown/)

[Source: .animate() | jQuery API Documentation](https://api.jquery.com/animate/)\

#### Q71. What is the main difference between the `contents()` and `children()` functions?

- [ ] They both return the content of selected nodes, but `children()` also includes text and comment nodes.
- [ ] The `contents()` function only includes text nodes of the selected elements.
- [ ] The `children()` function only includes text nodes of the selected elements.
- [x] They both return the content of selected nodes, but `contents()` also includes text and comment nodes.

1. [Source: .children() | jQuery API Documentation](https://api.jquery.com/children/)
2. [Source: .contents() | jQuery API Documentation](https://api.jquery.com/contents/)

#### Q72. If your JavaScript project involves a lot of DOM manipulation, but no AJAX or animation, which version of jQuery should you use?

- [ ] jQuery 3 compressed
- [ ] jQuery 3 slim
- [ ] jQuery 2
- [x] None of these - jQuery requires AJAX

#### Q73. The `.ready()` function is one of the most basic parts of jQuery, but jQuery also provides a mechanism for executing code when both one or more Promises have resolved and the DOM is ready. Which code snippet accomplishes this?

- [ ] A

```js
$(function({
    getData : $.get('http://httpbin.org/get'),
    delayedData : $.get('http://httpbin.org/delay/3')
})  {
    //DOM is ready, getData and delayedData are available
});
```

- [ ] B

```js
$($.get('http://httpbin.org/get'), $.get('http://httpbin.org/delay/3')).then(function (
  getData,
  delayedData,
) {
  //DOM is ready, getData and delayedData are available
});
```

- [ ] C

```js
$.when($.get('http://httpbin.org/get'), $.get('http://httpbin.org/delay/3')).then(function (
  getData,
  delayedData,
) {
  //DOM is ready, getData and delayedData are available
});
```

- [x] D

```js
$.ready($.get('http://httpbin.org/get'), $.get('http://httpbin.org/delay/3')).then(function (
  getData,
  delayedData,
) {
  //DOM is ready, getData and delayedData are available
});
```

#### Q74. You want to take an element and any event handlers that go with it out of the DOM to do some work—without the changes affecting the rest of the page—and then move it somewhere else in the DOM, like right after the opening tag. What should go on the first line of this code snippet?

```js
// what goes here?
// ... do some other hidden work on $example
$example.prependTo(document.body);
```

- [ ] `var $example = $('#example').remove();`
- [ ] `var $example = $('#example').clone();`
- [x] `var $example = $('#example').detach();`
- [ ] `var $example = $('#example').addBack().empty();`

https://api.jquery.com/detach/

#### Q75. Review the HTML below. You want to select the first item in the list and fade it out, then select the subsequent items up to (but not including) the active item, and fade them out halfway. How can you set up a single chain to do this?

```html
<ul class="items">
  <li>Item 1</li>
  <li>Item 2</li>
  <li>Item 3</li>
  <li class="active">Item 4</li>
  <li>Item 5</li>
  <li>Item 6</li>
</ul>
```

- [x] A

```js
$('.items > li').first().fadeOut().nextUntil('.active').fadeTo('fast', 0.5);
```

- [ ] B

```js
$('.items').children(':first-child').fadeOut().filter('.active').fadeTo('fast', 0.5);
```

- [ ] C

```js
$('.items > li').first().fadeOut().nextAll('.active').fadeOut(50);
```

- [ ] D

```js
$('.items').find('li:first-child').fadeOut().next('.active').fadeTo('fast', 0.5);
```

1. https://api.jquery.com/fadeTo/
2. https://api.jquery.com/fadeOut/
3. https://api.jquery.com/nextUntil/

#### Q76. What is a particular performance concern when dealing with event handlers, and how can you cope with it?

- [ ] Finding which element an event occurred on is expensive. Assign most events to document.body and use .is() to act on the element of interest.
- [x] Some events, such as mousemove and scroll, happen a lot on a typical page. Debounce or throttle their handlers to make sure the handlers are not called more than you actually need.
- [ ] Listening for an event that does not exist can create serious memory leaks. Be careful to spell event names correctly to avoid consuming too much memory.
- [ ] DOM elements with an ID wil fire events more efficiently than with classes. Always use IDs instead of classes where possible.

#### Q77. What is the purpose of the jQuery.fx.off global property?

- [ ] It turns off animations that are used to provide motion effect, but appearance effects remain enabled.
- [ ] It causes animation effects that are triggered via functions to instead be executed using CSS.
- [x] It globally disables all animations. When animations are run, all animation methods will immediately set elements to their final state when called, rather than displaying an effect.
- [ ] It globally disables animations that are triggered by CSS class changes.

[Source: jQuery.fx.off Property](https://www.w3schools.com/jquery/prop_jquery_fx_off.asp)

#### Q78. When you use custom Jquery selection extensions, such as :animated, on a page with lots of DOM elements, you can run into performance issues. What is the best practice for managing those issues?

- [ ] Select `$(document.body)` first, then use .filter with the custom extension.
- [ ] Use the custom extension with `.has()`.
- [ ] Start with the custom extension, then use `.find` with a selector that exists in CSS to limit the selection.
- [ ] Start with a selection that exists in CSS, then refine the selection using `.filter()` with the custom extension.

