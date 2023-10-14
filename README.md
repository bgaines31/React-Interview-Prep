#About React

#### <ins> What is React?
React is a front-end and open-source JavaScript library which is useful in developing user interfaces specifically for applications with a single page. It is helpful in building complex and reusable user interface(UI) components of mobile and web applications as it follows the component-based approach.
####  <ins>Major Features: 
<ul>
<li>Uses JSX/TSX which allows devs to write HTML in JS/TS
<li>Supports server-side rendering which boosts SEO
<li>Uses a Virtual DOM (Data Object Model) instead of a Real DOM to do manipulation which is cheaper
<li>One-day data flow and binding, but there are hooks that allow you to make data shareable from child to parent and between sibling nodes
<li>Huge ecosystem of libraries to choose from: React provides you with the freedom to choose the tools, libraries, and architecture for developing an application based on your requirement.

</ul>

####  <ins>Definitions:
<ul><li> <b> JSX </b>- stands for JavaScript XML and it is an XML-like syntax extension to ECMAScript. Allows for HTML to be integrated into JS/TS. Note that JSX is stricter than HTML.
<br>
Web browsers cannot read JSX directly. This is because they are built to only read regular JS objects and JSX is not a regular JavaScript object 
For a web browser to read a JSX file, the file needs to be transformed into a regular JavaScript object. For this, we use Babel
</li>
<li> <b>React Element</b> - describes what you want to see on the screen. Elements can contain other Elements in their props. Renders to the DOM using `ReactDOM.render()`. Looks like this: </li>

```HTML
 <div id=”login-btn”>Login</div>
  ``` 
<li> <b>React Component</b> - NEED DEF. Looks like this:</li>

```JSX
    const Button = ({ handleLogin }) => (
      <div id={"login-btn"} onClick={handleLogin}>
        Login
      </div>
    );
```

<li> <b>Function Component</b> - The simplest way to create a component. They are pure JS functions that accept props as the first param and returns React elements to render the output. <u>After Hooks were introduced in React 16.8, Functional components have been the recommended way to create components in React</u> Looks like this:</li>

```JSX
    function Greeting({ message }) {
  return <h1>{`Hello, ${message}`}</h1>;
}
```
<li> <b>Class Component</b> - The simplest way to create a component. They are pure JS functions that accept props as the first param and returns React elements to render the output. Looks like this:</li>

```JSX
    function Greeting({ message }) {
  return <h1>{`Hello, ${message}`}</h1>;
}
```

<li> <b>Pure Component</b> - I DONT GET IT</li>
<li><b>Virtual DOM</b> - React keeps a lightweight representation of the real DOM in the memory, and that is known as the virtual DOM. When the state of an object changes, virtual DOM changes only that object in the real DOM, rather than updating all the objects.
<br><br>
Additional info:

 React uses virtual DOM to render the view. As the name suggests, virtual DOM is a virtual representation of the real DOM. Each time the data changes in a react app, a new virtual DOM gets created. Creating a virtual DOM is much faster than rendering the UI inside the browser. Therefore, with the use of virtual DOM, the efficiency of the app improves. It is synced with the real DOM by a library such as ReactDOM. For every DOM object, there is a corresponding virtual DOM object(copy), which has the same properties. The main difference between the real DOM object and the virtual DOM object is that any changes in the virtual DOM object will not reflect on the screen directly. Consider a virtual DOM object as a blueprint of the real DOM object. Whenever a JSX element gets rendered, every virtual DOM object gets updated.
<br>
**Note- One may think updating every virtual DOM object might be inefficient, but that’s not the case. Updating the virtual DOM is much faster than updating the real DOM since we are just updating the blueprint of the real DOM.
</br>
<br>
React uses two virtual DOMs to render the user interface. One of them is used to store the current state of the objects and the other to store the previous state of the objects. Whenever the virtual DOM gets updated, react compares the two virtual DOMs and gets to know about which virtual DOM objects were updated. After knowing which objects were updated, react renders only those objects inside the real DOM instead of rendering the complete real DOM. This way, with the use of virtual DOM, react solves the problem of inefficient updating.
</li>
</br>

<li><b>useState</b>  - The useState() is a built-in React Hook that allows you for having state variables in functional components.The state is a built-in React object that is used to contain data or information about the component. The state in a component can change over time, and whenever it changes, the component re-renders.
The change in state can happen as a response to user action or system-generated events. It determines the behavior of the component and how it will render..</li>
<li><b>Keys (in a list)</b> - A key is a special string attribute that needs to be included when using lists of elements.  
<ul>
<li>Keys help react identify which elements were added, changed or removed.
<li>Keys should be given to array elements for providing a unique identity for each element. Recommended to NOT use index as key.
Without keys, React does not understand the order or uniqueness of each element.
<li>Keys are generally used for displaying a list of data coming from an API.
<li> <b>Note</b> - Keys used within arrays should be unique among siblings. They need not be globally unique.
</li>
</ul>
<li><b>Controlled component</b> - In a controlled component, the value of the input element is controlled by React. We store the state of the input element inside the code, and by using event-based callbacks, any changes made to the input element will be reflected in the code as well.
<li><b>Controlled and uncontrolled components</b> - Controlled and uncontrolled components are just different approaches to handling input from elements in react. 
<br>
When a user enters data inside the input element of a controlled component, onChange function gets triggered and inside the code, we check whether the value entered is valid or invalid. If the value is valid, we change the state and re-render the input element with the new value. Example:

```JSX
function FormValidation(props) {
let [inputValue, setInputValue] = useState("");
let updateInput = e => {
  setInputValue(e.target.value);
};
return (
  <div>
    <form>
      <input type="text" value={inputValue} onChange={updateInput} />
    </form>
  </div>
);
}
```
</li>
<li> <b>Uncontrolled component</b> - In an uncontrolled component, the value of the input element is handled by the DOM itself. Input elements inside uncontrolled components work just like normal HTML input form elements.
The state of the input element is handled by the DOM. Whenever the value of the input element is changed, event-based callbacks are not called. Basically, react does not perform any action when there are changes made to the input element. 
Whenever use enters data inside the input field, the updated data is shown directly. To access the value of the input element, we can use <b>ref</b>.

Example of an uncontrolled component:

```JSX
function FormValidation(props) {
let inputValue = React.createRef();
let handleSubmit = e => {
  alert(`Input value: ${inputValue.current.value}`);
  e.preventDefault();
};
return (
  <div>
    <form onSubmit={handleSubmit}>
      <input type="text" ref={inputValue} />
      <button type="submit">Submit</button>
    </form>
  </div>
);
}
```
</li>
<li> <b>Props</b> - The props in React are the inputs to a component of React. They can be single-valued or objects having a set of values that will be passed to components of React during creation by using a naming convention that almost looks similar to HTML-tag attributes. We can say that props are the data passed from a parent component into a child component.
<br>
Every React component accepts a single object argument called props (which stands for “properties”).  These props can be passed to a component using HTML attributes and the component accepts these props as an argument.

Using props, we can pass data from one component to another.

```JSX
function Car(props) {
let [brand, setBrand] = useState(props.brand);
}
```
 </li>
<li><b>Prop Drilling </b> - Sometimes while developing React applications, there is a need to pass data from a component that is higher in the hierarchy to a component that is deeply nested. To pass data between such components, we pass props from a source component and keep passing the prop to the next component in the hierarchy till we reach the deeply nested component.

The disadvantage of using prop drilling is that the components that should otherwise be not aware of the data have access to the data.

 </li>
<li><b> React Hooks:</b> <ul>
<li><b>What are they? </b> - React hooks were introduced in the 16.8 version of React. Previously, functional components were called stateless components. Only class components were used for state management and lifecycle methods. The need to change a functional component to a class component, whenever state management or lifecycle methods were to be used, led to the development of Hooks. example:

```JSX
function Person(props) {
// We are declaring a state variable called name.
// setName is a function to update/change the value of name
let [name, setName] = useState('');
}
```
</li>
<li><b> Hook Rules </b> - <ul>
<li>React Hooks must be called only at the top level. It is not allowed to call them inside the nested functions, loops, or conditions</li>
<li>It is allowed to call the Hooks only from the React Function Components.</li>
</ul></li><br>
<li><b>useEffect() </b> - The useEffect React Hook is used for performing the side effects in functional components. With the help of useEffect, you will inform React that your component requires something to be done after rendering the component or after a state change. The function you have passed(can be referred to as “effect”) will be remembered by React and call afterwards the performance of DOM updates is over. Using this, we can perform various calculations such as data fetching, setting up document title, manipulating DOM directly, etc, that don’t target the output value. The useEffect hook will run by default after the first render and also after each update of the component. React will guarantee that the DOM will be updated by the time when the effect has run by it.
<br><br>

The useEffect React Hook will accept 2 arguments: 
```JSX
useEffect(callback,[dependencies]);
```
Where the first argument callback represents the function having the logic of side-effect and it will be immediately executed after changes were being pushed to DOM. The second argument dependencies represent an optional array of dependencies. The useEffect() will execute the callback only if there is a change in dependencies in between renderings.

```jsx
import { useEffect } from 'react';
function WelcomeGreetings({ name }) {
 const msg = `Hi, ${name}!`;     // Calculates output
 useEffect(() => {
   document.title = `Welcome to you ${name}`;    // Side-effect!
 }, [name]);
 return <div>{msg}</div>;         // Calculates output
}
```
The above code will update the document title which is considered to be a side-effect as it will not calculate the component output directly. That is why updating of document title has been placed in a callback and provided to useEffect().

Consider you don’t want to execute document title update each time on rendering of WelcomeGreetings component and you want it to be executed only when the name prop changes then you need to supply name as a dependency to 
```JSX
 useEffect(callback, [name])
 ```
</li>
<li><b>useMemo( ) - </b></li>
<li><b>useContext():</b>
 It is used for creating common data that is to be accessed by the components hierarchy without having to pass the props down to each level.</li>
<li><b>useReducer() :</b> It is used when there is a complex state logic that is having several sub-values or when the upcoming state is dependent on the previous state. It will also enable you to optimization of component performance that will trigger deeper updates as it is permitted to pass the dispatch down instead of callbacks.</li>
<li><b>useCallback() : </b>This is useful while passing callbacks into the optimized child components and depends on the equality of reference for the prevention of unneeded renders.</li>
<li><b>useRef() : </b> It will permit creating a reference to the DOM element directly within the functional component.</li>
<li><b> </b></li>
<li><b> </b></li>
</ul> </li>
<li><b> Styling in React</b> <ul>

<li><b>Inline: </b>

```JSX
const RandomComponent = () => {
   return (
     <div>
       <h3 style={{ color: "Yellow" }}>This is a heading</h3>
       <p style={{ fontSize: "32px" }}>This is a paragraph</p>
     </div>
   );
}
```
</li>
<li><b>JS Object: </b>

```JSX
const RandomComponent = () => {
 paragraphStyles = {
   color: "Red",
   fontSize: "32px"
 };

 headingStyles = {
   color: "blue",
   fontSize: "48px"
 };
   return (
     <div>
       <h3 style={this.headingStyles}>This is a heading</h3>
       <p style={this.paragraphStyles}>This is a paragraph</p>
     </div>
   );
}
```
</li>
<li><b>CSS Stylesheet: </b>

```JSX
import './RandomComponent.css';

const RandomComponent = () => {
   return (
     <div>
       <h3 className="heading">This is a heading</h3>
       <p className="paragraph">This is a paragraph</p>
     </div>
   );
}
```
</li>
<li><b> </b></li>
</ul> </li>
<li><b> Ways to Optimize React Performance: </b>
<ul>
<li><b>Using useMemo( ) - </b> It is a React hook that is used for caching CPU-Expensive functions.
Sometimes in a React app, a CPU-Expensive function gets called repeatedly due to re-renders of a component, which can lead to slow rendering.
useMemo( ) hook can be used to cache such functions. By using useMemo( ), the CPU-Expensive function gets called only when it is needed.</li>
<li><b> Using React.PureComponent - </b> It is a base component class that checks the state and props of a component to know whether the component should be updated.
Instead of using the simple React.Component, we can use React.PureComponent to reduce the re-renders of a component unnecessarily.</li>
<li><b>Maintaining State Colocation - </b> This is a process of moving the state as close to where you need it as possible.
Sometimes in React app, we have a lot of unnecessary states inside the parent component which makes the code less readable and harder to maintain. Not to forget, having many states inside a single component leads to unnecessary re-renders for the component.
It is better to shift states which are less valuable to the parent component, to a separate component.</li>
<li><b>Lazy Loading - </b>  It is a technique used to reduce the load time of a React app. Lazy loading helps reduce the risk of web app performances to a minimum.
</li>
</ul>
</li>
<li><b>Higher Order Components - </b>A higher-order component acts as a container for other components. This helps to keep components simple and enables re-usability. They are generally used when multiple components have to use a common logic. </li>
<li><b>Phases of the React Component Lifestyle: </b>
<ul>
<li><b>Initialization: </b> During this phase, React component will prepare by setting up the default props and initial state for the upcoming tough journey.</li>
<li><b>Mounting: </b>Mounting refers to putting the elements into the browser DOM. Since React uses VirtualDOM, the entire browser DOM which has been currently rendered would not be refreshed. This phase includes the lifecycle methods <code>componentWillMount</code>
 and <code>componentDidMount</code>. 
</li>
<li><b>Updating: </b> In this phase, a component will be updated when there is a change in the state or props of a component. This phase will have lifecycle methods like <code>componentWillUpdate</code>, <code>shouldComponentUpdate</code>, <code>render</code>, and <code>componentDidUpdate </code>.</li>
<li><b>Unmounting:  </b>In this last phase of the component lifecycle, the component will be removed from the DOM or will be unmounted from the browser DOM. This phase will have the lifecycle method named <code>componentWillUnmount</code></li>
</ul>
</li>
<li><b>React Router - </b>React Router refers to the standard library used for routing in React. It permits us for building a single-page web application in React with navigation without even refreshing the page when the user navigates. It also allows to change the browser URL and will keep the user interface in sync with the URL. React Router will make use of the component structure for calling the components, using which appropriate information can be shown. Since React is a component-based framework, it’s not necessary to include and use this package. Any other compatible routing library would also work with React.</li>
<ul>
<li><b>BrowserRouter:  </b> It is a router implementation that will make use of the HTML5 history API (pushState, popstate, and event replaceState) for keeping your UI to be in sync with the URL. It is the parent component useful in storing all other components.</li>
<li><b>Routes: </b>It is a newer component that has been introduced in the React v6 and an upgrade of the component.</li>
<li><b>Route:  </b>It is considered to be a conditionally shown component and some UI will be rendered by this whenever there is a match between its path and the current URL.</li>
<li><b>Link: </b> It is useful in creating links to various routes and implementing navigation all over the application. It works similarly to the anchor tag in HTML.
</li>
</ul>
<li><b>Event - </b>An event is an action that a user or system may trigger, such as pressing a key, a mouse click, etc.

React events are named using camelCase, rather than lowercase in HTML.
With JSX, you pass a function as the event handler, rather than a string in HTML.

```JSX
<Button onClick={() => lightItUp} />
```
</li>
</ul>

####  <ins>React Redux:
<li><b>What is it? </b>Redux is an open-source, JavaScript library used to manage the application state. React uses Redux to build the user interface. It is a predictable state container for JavaScript applications and is used for the entire application’s state management.</li>
<li><b>Components of Redux </b>
<ul>
<li><b>Store: </b>Holds the state of the application.</li>
<li><b>Action: </b>The source information for the store.</li>
<li><b>Reducer: </b>Specifies how the application's state changes in response to actions sent to the store.</li>
</ul>
</li>
<li><b> </b></li>
<li><b> </b></li>
<li><b> </b></li>
<li><b> </b></li>
<li><b> </b></li>
<li><b> </b></li>
<li><b> </b></li>
<li><b> </b></li>
<li><b> </b></li>
<li><b> </b></li>
<li><b> </b></li>
<li><b> </b></li>
<li><b> </b></li>
<li><b> </b></li>
<li><b> </b></li>
<li><b> </b></li>


 
