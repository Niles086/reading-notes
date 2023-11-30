# React and Forms

How to use Forms in React

1. What is a ‘Controlled Component’? In React, a "controlled component" refers to a form element, such as an input or textarea, whose value is controlled by the state of the React component. In a controlled component, the value of the form element is managed by React state, and any changes to the input value are handled by React through state updates.
2. Should we wait to store the users responses from the form into state when they submit the form OR should we update the state with their responses as soon as they enter them? Why.
   the decision depends on the specific needs of your application. Consider the user experience, form complexity, and any real-time feedback or validation requirements to determine the most appropriate approach for storing user responses in state.
   Form Complexity: For simple forms, real-time updates may enhance the user experience. However, for complex forms with multiple sections, it might be more logical to wait until submission to update the state.

Validation Requirements: If you need to perform validation checks on user inputs, updating state as they enter responses allows you to provide immediate feedback.

Data Consistency: If ensuring data integrity and consistency is critical, storing responses on form submission may be more suitable.
3. How do we target what the user is entering if we have an event handler on an input field?
   In a React component, if you have an event handler on an input field, you can target what the user is entering by accessing the event object and extracting the value from the input field. The most common event for handling user input in React is the onChange event.

## The Conditional (Ternary) Operator Explained

1. Why would we use a ternary operator?
   Conciseness and Readability:

Ternary operators can make code more concise, especially for simple conditional assignments or operations.
For short and straightforward conditions, a ternary operator can enhance code readability by presenting the logic in a single line.
Avoiding Redundancy:

When you need to choose between two values based on a condition, using a ternary operator can help you avoid redundant code that might be present in a traditional if-else statement.
Inline Conditions:

Ternary operators are useful for inline conditions within JSX or template literals, making it easier to embed conditional values directly in your markup or strings.
2. Rewrite the following statement using a ternary statement: console.log(x === y ? true : false);
   

            if(x===y){
            console.log(true);
            } else {
            console.log(false);
            }


## Bookmark and Review

React Bootstrap - Forms
React Docs - conditional rendering

## Things I want to know more about