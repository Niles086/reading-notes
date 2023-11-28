# State and Props

[React lifecycle](https://medium.com/@joshuablankenshipnola/react-component-lifecycle-events-cb77e670a093)

1. Based off the diagram, what happens first, the ‘render’ or the ‘componentDidMount’? Render happens first.
2. What is the very first thing to happen in the lifecycle of React? Mounting is the first thing.
3. Put the following things in the order that they happen: constructor, componentDidMount, render,  componentWillUnmount, React Updates
4. What does componentDidMount do?
  Its a lifecycle method that allows you to perform tasks that should happen after the initial render of the component. 

## Videos

[React State Vs Props](https://www.youtube.com/watch?v=IYvD9oBCuJI)

1. What types of things can you pass in the props?

* Strings, numbers, booleans: Simple values can be passed as props.
* Functions: You can pass functions as props to allow child components to communicate with parent components.
* Objects and arrays: Complex data structures can be passed as props.

2. What is the big difference between props and state?

* Props (Properties): Props are immutable (read-only) and are used to pass data from parent components to child components. They are set by the parent and cannot be changed by the child components.
* State: State is mutable (can be changed) and is used to manage the internal state of a component. It is initialized and managed within the component itself. State changes trigger re-renders.

3. When do we re-render our application?

* React components re-render when their state or props change. Changes to the state or props trigger the render method, updating the view.

4. What are some examples of things that we could store in state?

* Form data: Input values, dropdown selections, etc.
UI state: Such as whether a modal is open or closed.
Data fetched from an API: When the data needs to be displayed in the component and may change over time.
Toggle state: Whether something is expanded or collapsed.
User authentication state: To track whether a user is logged in or not.

In Closing props are for passing data from parent to child, while state is for managing internal component state. Components re-render when their state or props change, and understanding the difference is crucial for effective React development.


## Bookmark and Review

[React Docs - State and Lifecycle](https://reactjs.org/docs/state-and-lifecycle.html)
[React Docs - handling events](https://reactjs.org/docs/handling-events.html)
[React Tutorial through ‘Developer Tools’](https://reactjs.org/tutorial/tutorial.html)
[React Bootstrap Documentation](https://react-bootstrap.github.io/)
[Boootstrap Cheatsheet](https://getbootstrap.com/docs/5.0/examples/cheatsheet/)
[Bootstrap Shuffle - a class “sandbox”](https://bootstrapshuffle.com/classes)
[Netlify](https://www.netlify.com/)