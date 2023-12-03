# Putting it all together

## Reading

## [React Docs - Thinking in React](https://reactjs.org/docs/thinking-in-react.html)

1. What is the single responsibility principle and how does it apply to components?
2. What does it mean to build a ‘static’ version of your application?
3. Once you have a static application, what do you need to add?
4. What are the three questions you can ask to determine if something is state?
5. How can you identify where state needs to live?

## Answers

Single Responsibility Principle and Components:

The Single Responsibility Principle (SRP) is a software design principle that states that a component or module should have only one reason to change. Applied to components in React, it means that each component should ideally have a single responsibility or perform a single function. This makes components more modular, maintainable, and easier to understand. For example, a component responsible for rendering a button should not handle data fetching or business logic.
Building a 'Static' Version:

Building a 'static' version of an application in React refers to creating a version that renders the user interface from the data model without incorporating any interactivity. In this phase, components are created to display the UI based on the initial data, and props are used for data flow. This allows developers to establish the basic structure and appearance of the application before introducing dynamic behavior.
Adding to the Static Application:

Once a static version of the application is in place, the next step involves adding interactivity and dynamic behavior. This includes incorporating state to manage data that changes over time, responding to user input, and updating the UI accordingly. The static version serves as a foundation, and developers build upon it to create a fully functional and responsive application.
Three Questions to Determine State:

To determine if something is state in a React application, you can ask the following three questions:
Does it remain unchanged over time? If yes, it isn't state.
Is it passed in from a parent via props? If yes, it isn't state.
Can you compute it based on existing state or props in your component? If yes, it definitely isn't state.
Identifying Where State Should Live:

To identify where state should live in a React application, you can follow these steps:
Identify every component that renders something based on that state.
Find the closest common parent component—a component above them all in the hierarchy.
Decide where the state should live based on the identified common parent. It can be directly in the common parent, in some component above the common parent, or in a new component created solely for holding the state.


## [Higher-Order Functions](https://eloquentjavascript.net/05_higher_order.html#h_xxCc98lOBK)

1. What is a “higher-order function”?
2. Explore the greaterThan function as defined in the reading. In your own words, what is line 2 of this function doing?
3. Explain how either map or reduce operates, with regards to higher-order functions.

## Answers2

A higher-order function is a function that either takes one or more functions as arguments or returns a function as its result. In other words, it operates on functions, treating them as first-class citizens in the programming language. Higher-order functions enable the abstraction of actions, allowing for more flexible and modular code.

This function takes a single argument n and returns another function that, when called with an argument m, checks whether m is greater than n. It essentially creates a function that can be customized to check if a given value is greater than the specified threshold n.

Explanation of Line 2 (return m => m > n;):
This line defines an arrow function that takes a parameter m and returns the result of the comparison m > n. It utilizes the fact that functions in JavaScript can be defined inline and returned as values. So, greaterThan returns a function that captures the value of n from the outer scope and can be later invoked with a different value (m) to perform the comparison.

Map or Reduce as Higher-Order Functions:
Both map and reduce are higher-order functions in JavaScript that operate on arrays.

Map:

map applies a provided function to each element of an array and returns a new array with the results. It takes a function as an argument, which is applied to each element, transforming the original elements into a new set of values.

reduce combines the elements of an array into a single value. It takes a function as an argument that defines the reduction operation. This function typically has an accumulator that accumulates the result and an element that represents each item in the array.

## Things I want to know more about