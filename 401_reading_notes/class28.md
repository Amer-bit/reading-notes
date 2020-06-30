# Components and Props
components are like JavaScript functions. They accept arbitrary inputs (called “props”) and return React elements describing what should appear on the screen.

**NOTE: recommend naming props from the component’s own point of view rather than the context in which it is being used**

**NOTE: JavaScript expression can be passed as a prop, by surrounding it with {}.**

# Function and Class Components
The simplest way to define a component is to write a JavaScript function.We call such components “function components” because they are literally JavaScript functions.

Or we can can also use an ES6 class to define a component

Component can  DOM tags or a user-defined component. When React sees an element representing a user-defined component, it passes JSX attributes and children to this component as a single object. We call this object `props`

````function Welcome(props) {
  return <h1>Hello, {props.name}</h1>;
}

const element = <Welcome name="Sara" />;
ReactDOM.render(
  element,
  document.getElementById('root')
)
````
this code renders “Hello, Sara” on the page

**NOTE: Extracting components might seem like grunt work at first, but having a palette of reusable components pays off in larger apps. A good rule of thumb is that if a part of your UI is used several times (Button, Panel, Avatar), or is complex enough on its own (App, FeedStory, Comment), it is a good candidate to be extracted to a separate component.**

**NOTE: All React components must act like pure functions with respect to their props.**

**A pure function do not attempt to change their inputs, and always return the same result for the same inputs.**

**NOTE: In applications with many components, it’s very important to free up resources taken by the components when they are destroyed.**