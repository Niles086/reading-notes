# Passing Functions as Props

React Docs - lists and keys){:target=”_blank”}

1. What does .map() return? The .map() method in JavaScript returns a new array created by applying a provided function to each element in the original array.
2. If I want to loop through an array and display each value in JSX, how do I do that in React? In React, you can use the .map() method to loop through an array and create JSX elements for each item. Here's an example:

                const myArray = [1, 2, 3, 4];

                const jsxElements = myArray.map((item) => <p key={item}>{item}</p>);

                // Then, you can render jsxElements in your component

3. Each list item needs a unique ____. Each list item in React needs a unique key. The key is a special attribute that helps React identify which items have changed, been added, or been removed. It should be a unique identifier for each item in the array.
4. What is the purpose of a key? The purpose of a key in React is to help the framework identify which items in a list have changed, been added, or been removed. When rendering lists of components, React uses the key to efficiently update the virtual DOM. The key should be a stable identifier and should be unique within the list of elements. It helps React optimize the rendering process and improve performance when dealing with dynamic lists.

The Spread Operator

1. What is the spread operator? The spread operator (...) is a JavaScript syntax introduced in ECMAScript 6 (ES6). It allows an iterable, like an array or string, to be expanded or spread into individual elements.
2. List 4 things that the spread operator can do.
   
                        a. Copying Arrays:

                        javascript
                        Copy code
                        const originalArray = [1, 2, 3];
                        const newArray = [...originalArray];
                        b. Combining Arrays:

                        javascript
                        Copy code
                        const array1 = [1, 2, 3];
                        const array2 = [4, 5, 6];
                        const combinedArray = [...array1, ...array2];
                        c. Adding Elements to an Array:

                        javascript
                        Copy code
                        const originalArray = [1, 2, 3];
                        const newArray = [...originalArray, 4];
                        d. Copying Objects (Shallow Copy):

                        javascript
                        Copy code
                        const originalObject = { key1: 'value1', key2: 'value2' };
                        const newObject = { ...originalObject };

3. Give an example of using the spread operator to combine two arrays.
   
        const array1 = [1, 2, 3];
        const array2 = [4, 5, 6];
        const combinedArray = [...array1, ...array2];
        console.log(combinedArray); // Output: [1, 2, 3, 4, 5, 6]

4. Give an example of using the spread operator to add a new item to an array.
   
                    const originalArray = [1, 2, 3];
                    const newArray = [...originalArray, 4];
                    console.log(newArray); // Output: [1, 2, 3, 4]

5. Give an example of using the spread operator to combine two objects into one.
   
   const object1 = { key1: 'value1', key2: 'value2' };
const object2 = { key3: 'value3', key4: 'value4' };
const combinedObject = { ...object1, ...object2 };
console.log(combinedObject);
// Output: { key1: 'value1', key2: 'value2', key3: 'value3', key4: 'value4' }


## Videos

How to Pass Functions Between Components

1. In the video, what is the first step that the developer does to pass functions between components?
2. In your own words, what does the handleClick function do?
3. How can you pass a method from a parent component into a child component?
4. How does the child component invoke a method that was passed to it from a parent component?

## Bookmark and Review

React Tutorial through ‘Declaring a Winner’
[React Docs - Lifting State Up](https://reactjs.org/docs/lifting-state-up.html)